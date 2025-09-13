# Universal Medical Card (Showcase)

A web-based platform for creating, managing, and sharing a universal digital medical card. This application is designed to provide users with a centralized and easily accessible way to store their critical medical information.

## Status 

In Development. The full source code for this project is hosted in a private repository.

## Features

*   **User Authentication:** Secure registration and login system for users.
*   **Profile Management:** Create and manage detailed medical profiles.
*   **Dynamic QR Codes:** Generate a QR code for each profile to allow for quick access to public-facing medical information.
*   **FHIR Integration:** Leverages the FHIR standard for healthcare data interoperability.
*   **Internationalization:** Support for multiple languages (English and Spanish).
*   **File Uploads:** Attach and store medical documents and exam results.
*   **Responsive Design:** Accessible on both desktop and mobile devices.

## Tech Stack


*   **Backend:** ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54), Flask
*   **Database:** Google Firestore
*   **Frontend:** HTML, CSS, JavaScript, Jinja2
*   **Deployment:** ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white), ![Google App Engine](https://img.shields.io/badge/Google_Cloud-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white) 
*   **Libraries:**
    *   Firebase Admin SDK
    *   Flask-WTF & WTForms
    *   Pillow
    *   PyMuPDF
    *   qrcode

## Getting Started

Follow these instructions to get a local copy of the project up and running for development and testing purposes.

### Prerequisites

*   Python 3.10+
*   `pip` for package management
*   A Google Cloud Platform project with Firestore enabled.
*   Firebase Admin SDK credentials.

### Installation

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/your-username/universal-medical-card.git
    cd universal-medical-card
    ```

2.  **Create and activate a virtual environment:**
    ```sh
    python -m venv venv
    source venv/bin/activate
    # On Windows, use: venv\Scripts\activate
    ```

3.  **Install the required dependencies:**
    ```sh
    pip install -r requirements.txt
    ```

4.  **Set up environment variables:**
    Create a `.env` file in the project root and add the necessary configuration. This typically includes your Firebase credentials.
    ```
    FLASK_APP=run.py
    FLASK_ENV=development
    SECRET_KEY='a_very_secret_key'

    # Firebase Credentials
    GOOGLE_APPLICATION_CREDENTIALS='path/to/your/firebase-credentials.json'
    ```

### Running the Application

1.  **Run the Flask development server:**
    ```sh
    flask run
    ```
    Or directly using python:
    ```sh
    python run.py
    ```

2.  **Access the application:**
    Open your web browser and navigate to `http://127.0.0.1:5000` or the address shown in your terminal.

## Usage

Once the application is running, you can:
*   Register for a new account.
*   Log in and create your medical profile.
*   Add personal details, emergency contacts, allergies, and medical conditions.
*   Upload relevant medical documents.
*   Share your profile via the generated QR code.

