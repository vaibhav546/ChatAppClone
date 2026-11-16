# ChatApp Clone – Real-Time Android Messaging App

A real-time chat application for Android, built with **Kotlin, Jetpack Compose and Firebase** as part of the *Mobile App Development* module of my MSc Computer Science at Teesside University (2024).

Users can sign up, log in, chat in real time, share a status with images, and manage their profile. The project also includes a review of the **social, legal, ethical and security considerations** of building a messaging app.

---

## Features

- **Sign up and login.** Accounts are created with name, email, phone number and password, using Firebase Authentication.
- **Real-time chat.** Send and receive messages instantly, add new contacts and start conversations.
- **Status page.** Post and update a status, including images.
- **Profile management.** View and edit name, photo and phone number, and save the changes to the database.
- **Navigation.** Splash screen, Back and Logout buttons, and a simple page flow.

## Screenshots

| Login | Chat | Status | Profile |
|-------|------|--------|---------|
| ![Login](screenshots/login.png) | ![Chat](screenshots/chat.png) | ![Status](screenshots/status.png) | ![Profile](screenshots/profile.png) |

## Tech Stack

| Area | Tool |
|------|------|
| Language and UI | Kotlin, Jetpack Compose |
| Backend and database | Firebase Authentication, Firebase Realtime Database, Firebase Storage |
| IDE | Android Studio 2023.1.1 (build tools 29.0.2) |
| Project management | Trello (Kanban board) |
| Version control | Git and GitHub |

## Data Design

User data is stored in Firebase as structured JSON. Each user record holds the profile fields (name, email, phone, photo URL, status), and messages are stored per conversation with sender, receiver, text and timestamp. The app reads and writes these records in real time, much like running SELECT and UPDATE queries on a relational database.

## Privacy, Ethics and Security

- **Privacy.** Users control their own profile information, and data is stored in Firebase rather than on the device.
- **Security.** Email-based authentication and Firebase access rules and encryption protect accounts and data.
- **Legal.** The design follows basic data-protection principles (GDPR) to prevent misuse of personal data.
- **Social.** The report discusses digital well-being and the need for content moderation in messaging platforms.

## Development Process

I used an **Agile Kanban** approach. Tasks were tracked on a Trello board with To Do, In Progress, Testing and Done columns, and limits on work in progress kept the workflow steady.

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/vaibhav546/ChatAppClone.git
   ```
2. Open the project in **Android Studio**.
3. Create a Firebase project, enable **Authentication (Email/Password)** and **Realtime Database**, and add your own `google-services.json` to the `app/` folder.
4. Build and run the app on an emulator or an Android device.

## Known Limitations and Next Steps

- Some screens need UI and usability improvements, for example the splash-screen logo sizing.
- Planned: message read receipts, push notifications, end-to-end encryption, and content-moderation tools.

## What I Learned

- Building declarative UIs with Jetpack Compose, a new framework for me
- Connecting a front-end to a cloud backend (Firebase)
- Planning a project with Kanban, and thinking through the ethics and security of user data

## Author

**Vaibhav Bhalani** · MSc Computer Science, Teesside University
[LinkedIn](https://linkedin.com/in/vaibhavbhalani)
