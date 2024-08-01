# Google API Token Generator

This project helps to generate a token that will be used for calling Google APIs and services.

## Setup

### Create a Virtual Environment
Creating a virtual environment is a good practice to manage dependencies.
```sh
python3 -m venv venv
```
To activate the virtual environment:
```sh
source venv/bin/activate
```

### Install the Required Packages
Install the necessary packages using:
```sh
pip install -r requirements.txt
```

### Google OAuth Credentials
You need to obtain Google OAuth credentials and save them under `data/input/credentials.json`. Follow these steps:

1. Go to the [Google Cloud Console](https://console.cloud.google.com/).
2. Create a new project or select an existing project.
3. Navigate to the **Credentials** section.
4. Click on **Create Credentials** and select **OAuth 2.0 Client IDs**.
5. Configure the consent screen and download the credentials JSON file.
6. Place the downloaded `credentials.json` file in the `data/input/` directory.

### Enable Required APIs
Enable the Gmail and Calendar APIs in the Google Cloud Console:

1. Go to the [API Library](https://console.cloud.google.com/apis/library).
2. Search for **Gmail API** and **Google Calendar API**.
3. Enable both APIs for your project.

### Accessing the Credentials
For a step-by-step guide on accessing and setting up the `credentials.json` file, refer to this [video tutorial](https://drive.google.com/file/d/1n8N0ry0xDiXk1txhAgt-8KzdZQUUuou5/view).

## Running the Application

### Generating Google API Token
To generate the Google API token, run the following command:
```sh
python -m src.token_generator
```

The above script will generate the token and store it as data/input/token.json
