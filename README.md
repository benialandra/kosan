# Kosan Management System

This project is a web-based application built with Google Apps Script, designed to help manage "kosan" (boarding houses or rental rooms). It provides an administrative interface, a dashboard, and specific views for room management.

## Features

*   **Dashboard View:** Overview of key information and statistics.
*   **Admin View:** Administrative functions for managing the system.
*   **Kamar (Room) View:** Specific interface for managing individual rooms or units.
*   **Google Apps Script Integration:** Leverages Google's ecosystem for backend logic, data storage (e.g., Google Sheets, Google Forms), and deployment.
*   **Web UI:** Interactive user interface built with HTML and JavaScript.

## Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

*   Node.js and npm (or yarn) installed.
*   `clasp` (Command Line Apps Script Project) installed globally:
    ```bashz
    npm install -g @google/clasp
    ```
*   A Google Cloud Project with the Google Apps Script API enabled.

### Deployment

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/your-repository.git
    cd your-repository
    ```
2.  **Login to `clasp`:**
    ```bash
    clasp login
    ```
    This will open a browser window for you to authenticate with your Google account.
3.  **Link to an existing Apps Script project or create a new one:**
    If you have an existing Apps Script project you want to link, use:
    ```bash
    clasp clone <Script ID>
    ```
    Alternatively, to create a new project:
    ```bash
    clasp create --title "Kosan Management" --type webapp
    ```
    This will create a new Google Apps Script project and generate a `.clasp.json` file.
4.  **Push the code to Apps Script:**
    ```bash
    clasp push
    ```
    This command uploads all local files (`Code.js`, `AdminView.html`, etc.) to your Google Apps Script project.
5.  **Deploy as a Web App:**
    *   Go to your Apps Script project online (script.google.com).
    *   Click `Deploy` -> `New deployment`.
    *   Select `Web app` as the type.
    *   Configure access (e.g., "Anyone," "Anyone, even anonymous").
    *   Click `Deploy` and authorize the necessary permissions.
    *   Copy the Web App URL.

## Usage

Once deployed, access the application through the Web App URL obtained during deployment.

*   **`Index.html`**: The main entry point of the web application.
*   **`DashboardView.html`**: Displays key metrics and an overview.
*   **`AdminView.html`**: Provides tools for administrators.
*   **`KamarView.html`**: Allows management of individual rooms.
*   **`Code.js`**: Contains the Google Apps Script backend logic.
*   **`Javascript.html`**: Likely contains shared JavaScript functions or libraries used by other HTML templates.

## Technologies Used

*   Google Apps Script
*   HTML
*   JavaScript
*   clasp (Command Line Apps Script Project)

## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.

---
**Note:** The `.clasp.json` and `appsscript.json` files are crucial for `clasp` to manage your Google Apps Script project. Do not modify them unless you understand their purpose.
