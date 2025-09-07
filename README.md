# Smart Email Assistant 📧

A full-stack application and browser extension that simplifies email management by generating intelligent, AI-powered replies. This project combines a robust Spring AI backend with a user-friendly React frontend and a practical browser extension for direct integration with Gmail.

---

### ✨ Features

* **AI-Powered Reply Generation**: Automatically generate email replies based on the content of an original email.
* **Tone Selection**: Customize the tone of the generated reply (e.g., Professional, Casual, Friendly).
* **Seamless Gmail Integration**: A browser extension injects an "AI Reply" button directly into the Gmail compose window, allowing for instant reply generation without leaving your inbox.
* **Gemini API Integration**: Leverages Google's cutting-edge Gemini API for high-quality, context-aware reply generation.
* **User-Friendly Interface**: The React-based frontend provides a simple and intuitive experience for generating and copying replies.

---

### 💻 Technology Stack

This project is built using a modern and powerful technology stack.

#### Backend
* **Framework**: Spring Boot
* **AI Library**: Spring AI
* **LLM**: Google Gemini API
* **Build Tool**: Maven

#### Frontend
* **Framework**: React.js
* **UI Library**: Material-UI (MUI)
* **API Client**: Axios

#### Browser Extension
* **Technology**: Plain JavaScript
* **Functionality**: Utilizes a `MutationObserver` to dynamically inject a button into the Gmail UI.

---

### 🚀 Getting Started

Follow these steps to set up and run the project locally.

#### Prerequisites

* Java Development Kit (JDK) 17 or higher
* Node.js and npm
* A Google Gemini API Key

#### 1. Backend Setup

1.  Clone the repository:
    ```bash
    git clone [https://github.com/bairisai/Smart-Email-Assistant.git](https://github.com/bairisai/Smart-Email-Assistant.git)
    cd Smart-Email-Assistant
    ```
2.  Navigate to the `backend` directory.
    ```bash
    cd backend
    ```
3.  Add your Gemini API key to `src/main/resources/application.properties`.
    ```properties
    spring.ai.gemini.api-key=<YOUR_GEMINI_API_KEY>
    ```
4.  Build and run the application using Maven:
    ```bash
    ./mvnw spring-boot:run
    ```
    The backend server will start on `http://localhost:8080`.

#### 2. Frontend Setup

1.  In a new terminal, navigate to the `frontend` directory.
    ```bash
    cd frontend
    ```
2.  Install the necessary dependencies.
    ```bash
    npm install
    ```
3.  Start the React development server.
    ```bash
    npm start
    ```
    The frontend application will open in your browser at `http://localhost:5173`.

#### 3. Browser Extension Setup

1.  Open your web browser (e.g., Google Chrome).
2.  Navigate to the extensions management page.
    * Chrome: `chrome://extensions`
3.  Enable **Developer mode** in the top-right corner.
4.  Click **"Load unpacked"** and select the `extension` directory from your cloned repository.
5.  The AI Reply button will now be injected into your Gmail interface.

---

### 🗺️ Usage

#### Using the Web Application

1.  Open `http://localhost:3000` in your browser.
2.  Paste the content of an email into the text area.
3.  Select a desired tone (e.g., Professional).
4.  Click **"Generate Reply"** to get an AI-powered response.

#### Using the Gmail Extension

1.  Open Gmail in your browser.
2.  When you open or start a new email, the "AI Reply" button will appear in the compose toolbar.
3.  Click the button to automatically generate and insert a reply based on the email's content.

---
