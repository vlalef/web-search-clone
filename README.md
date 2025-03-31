# Google Search Clone

This is a simple search tool developed as part of Harvard CS50's Web Programming with Python and JavaScript course. The project aims to replicate Google's search functionality while studying Flask and HTML.

## Features

- **Google Search**: Search the web using Google's search engine
- **Image Search**: Dedicated interface for searching images
- **Advanced Search**: Fine-tune your search with options for:
  - All these words
  - This exact word or phrase
  - Any of these words
  - None of these words
- **"I'm Feeling Lucky"** button that takes you directly to the first search result

## Getting Started

### Prerequisites

- Python 3.x
- Flask

### Installation

1. Clone the repository:
    ```bash
    git clone <repository-url>
    cd web-search-clone
    ```

2. Create and activate a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install Flask:
    ```bash
    pip install flask
    ```

### Running the Application Locally

1. Start the Flask development server:
    ```bash
    python app.py
    ```

2. Open your web browser and go to `http://127.0.0.1:8000` (or `http://localhost:8000`).

### Deploying the Application

To deploy the application, you can use a platform like Heroku. Here are the steps:

1. **Install the Heroku CLI**: Follow the instructions on the [Heroku CLI installation page](https://devcenter.heroku.com/articles/heroku-cli).

2. **Log in to Heroku**:
    ```bash
    heroku login
    ```

3. **Create a new Heroku app**:
    ```bash
    heroku create
    ```

4. **Add a `Procfile`**: Create a file named `Procfile` in the root directory of your project with the following content:
    ```text
    web: python app.py
    ```

5. **Commit your changes**:
    ```bash
    git add .
    git commit -m "Prepare app for Heroku deployment"
    ```

6. **Deploy to Heroku**:
    ```bash
    git push heroku main
    ```

7. **Open your deployed app**:
    ```bash
    heroku open
    ```

### Additional Notes

- Ensure that your `app.py` file is configured to run on the correct host and port for deployment.
- You may need to set up environment variables for production settings.py