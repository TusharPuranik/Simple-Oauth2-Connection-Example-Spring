# Hello World OAuth2 Client in Spring for Google API

This project demonstrates a simple "Hello World" application built using Spring that utilizes OAuth2 client to connect to Google API services. The application authenticates with Google using OAuth2 and retrieves basic user information.

## Features:
- Connects to Google API services using OAuth2 client in Spring.
- Retrieves basic user information from the authenticated Google account.

## Prerequisites:
- Java JDK 8 or higher installed.
- Gradle build tool.

## Steps to Run the Project:
1. Clone the repository from GitHub.
2. Open a terminal/command prompt and navigate to the project's root directory.
3. Build the project using Gradle: `./gradlew build`
4. Run the application: `./gradlew bootRun`

## Steps to Create Credentials for Google API:
1. Go to the [Google Developers Console](https://console.developers.google.com/).
2. Create a new project or select an existing one.
3. In the left navigation menu, click on "Credentials".
4. Click the "Create Credentials" button and choose "OAuth client ID".
5. Select "Web Application" as the application type.
6. Enter a name for the OAuth client (e.g., "My Hello World App").
7. Under "Authorized Redirect URIs", add the redirect URI for your local development environment (e.g., http://localhost:8080/login/oauth2/code/google).
8. Click the "Create" button.
9. Once the credentials are created, you'll see your Client ID and Client Secret.
10. Copy the Client ID and Client Secret and update your Spring application's configuration with these values.

## Configuring the Project with Google API Credentials:
1. Open the `application.properties` file in the `src/main/resources` directory.
2. Replace `<YOUR_CLIENT_ID>` and `<YOUR_CLIENT_SECRET>` with your actual Google API Client ID and Client Secret, respectively.

## Usage:
1. Run the application.
2. Access the application in your web browser at `http://localhost:8080`.
3. Click the "Login with Google" button to authenticate with Google.
4. Upon successful authentication, the application will display basic user information retrieved from the Google account in the console.
