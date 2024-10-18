# Spring Boot Mail Sender Application

This project demonstrates how to send a simple email using Spring Boot and Gmail's SMTP server.

# Requirements

- Java 8 or higher
- Maven
- Gmail account with "Less secure apps" enabled (or app password for two-factor authentication)

# Steps: 

# Option 1 : Enable "Less secure apps" (For accounts without two-factor authentication)
```bash
Note: Google is phasing out the "Less secure apps" feature, so it's recommended to use two-factor authentication with an app-specific password if possible.
```
- Login to your Google Account:
- Go to Google Account and sign in with your credentials.
- Go to Security Settings:
- Click on "Security" from the left-hand navigation menu.
- Scroll to "Less secure app access":
- In the "Less secure app access" section, click Turn on access (not recommended).
- Turn ON the setting:
- Click the switch to turn ON the less secure app access.
  
# Option 2: Use an App-Specific Password (For accounts with two-factor authentication)
- If your Gmail account has two-factor authentication enabled, you will need to generate an app-specific password.
- Login to your Google Account:
- Go to Google Account and sign in with your credentials.
- Enable Two-Factor Authentication (if not already enabled):
- In the Security section, under "Signing in to Google", ensure that 2-Step Verification is turned on. If it is not, click 2-Step Verification and follow the steps to enable it.
- Generate an App Password:
- After enabling 2-Step Verification, go back to the Security section.
- Under "Signing in to Google", click on App passwords.
- Create an App Password:
- You may be prompted to re-enter your Google account password.
- In the App passwords section, select Mail as the app and Other as the device. Name it something like "Spring Boot App".
- Click Generate.
- Google will generate a 16-character password. Copy this password.
- Use this 16-character password in your Spring Boot application as the value for the spring.mail.password property in your environment variables.

# clone repository

```bash
https://github.com/Prathamesh-Jagtap/SpringBoot-MailSender.git
cd SpringBoot-MailSender
```

# Build and Run the Project

```bash
mvn clean install
mvn spring-boot:run
```

# Test the endpoints using Postman/OpenAPI

