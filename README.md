Sample output on Google Collab

![Docker Containerization Screenshot](screenshot2.png)


# Ollama Setup

This project sets up the Ollama API server and integrates it with a simple Question-Answer (QA) component using the `lightrag` library.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The Ollama API server is configured to serve the `llama3.1:8b` model. This project demonstrates how to set up the server, pull the model, and use a QA component to generate responses based on user input.

## Installation

### Prerequisites

- Python 3.x
- Git for Windows
- `pip` package manager
- Chocolatey (for installing Curl)

### Steps

1. **Clone the Repository:**
    ```sh
    git clone https://github.com/<username>/ollama-setup.git
    cd ollama-setup
    ```

2. **Install Required Packages:** (For Windows) 
    - Open Command Prompt or PowerShell as Administrator and run the following commands:
    ```sh
    choco install curl
    curl -fsSL https://ollama.com/install.sh -o install.sh
    bash install.sh
    pip install -U lightrag[ollama]
    ```

## Usage

1. **Run the Script:**
    - Open Command Prompt or PowerShell in the project directory and run:
    ```sh
    python ollama_setup.py
    ```

2. **Interact with the QA Component:**

    The script initializes the Ollama API server and pulls the `llama3.1:8b` model. It sets up a simple QA component to generate responses based on user input.

3. **Example:**

    When prompted, enter a question like:

    ```
    How do you born?
    ```

    The component will generate and display an answer.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.


## I made additional step on the proces to set up the environment in docker containerization and later deploy it on OpenWebUi and access Ollama from Your Phone using NGROK


![Docker Containerization Screenshot](screenshot3.png)

![NGROK Screenshot](screenshot4.png)

![User Interface on OpenWebui Screenshot](screenshot1.png)