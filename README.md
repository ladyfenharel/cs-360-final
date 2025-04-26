# 📅 Event Manager Android App

## 📝 Project Summary

The Event Manager app is an Android application developed to help users create, track, and manage personal events. The app addresses a common user need: staying organized and receiving timely reminders about upcoming commitments. It includes an optional SMS notification feature, which sends alerts about new events directly to the user's phone.

## 🎯 User Needs & UI Design

This app was designed to support users who need a quick and simple way to manage their event schedules without the complexity of full calendar integration. The app prioritizes:

- Easy event creation
- Editing and deleting existing events
- Visual organization of events through a responsive grid layout
- Optional SMS notifications to serve as timely reminders

To meet these needs, the user interface includes:
- A dashboard with a clean, user-friendly grid layout using RecyclerView
- An event creation dialog for fast input of event details (name, date, time)
- An edit dialog allowing in-place updates of existing events
- Permission handling for SMS messaging, keeping user privacy in mind

The UI is centered on simplicity and usability. All buttons and inputs are clearly labeled, and the layout adapts well to different screen sizes, ensuring an accessible experience for all users.

## 💻 Development Approach

Development was broken into modular components to maintain clean architecture. Key strategies included:

- Separation of concerns: The database logic was abstracted into a helper class (EventDatabaseHelper) to keep the UI code manageable.
- EventAdapter with RecyclerView: This pattern allowed efficient rendering of dynamic event lists.
- PermissionHelper: A separate class for SMS permission logic improved code readability and maintainability.
- Testing with Android Emulator: Simulated permission grants and denials to verify conditional behavior.

These strategies helped produce reusable, scalable components that can easily be applied to future mobile projects.

✅ Testing & Quality Assurance

Thorough testing was performed using the Android Emulator to simulate different user actions, including:

[x] Granting or denying SMS permissions

[x] Creating, editing, and deleting events

[x] Verifying database persistence

[x] Ensuring the app UI remains functional regardless of permission status

Testing revealed the importance of defensive coding and fail-safe design, ensuring the app remained stable even when optional features like SMS were disabled by the user.

## 🚀 Full Development Lifecycle & Challenges

From planning through to deployment, the app followed a structured design and build process. One key challenge was ensuring the app would function properly with or without SMS permissions. This required conditional logic and robust error handling to maintain a smooth experience for all users.

Another area that required innovation was designing an intuitive event editing interface. The use of AlertDialog for in-place editing provided a lightweight solution that felt seamless to users.

## 🏆 Key Accomplishment

A standout success was the integration of SQLite database functionality with full CRUD (Create, Read, Update, Delete) operations tied into the RecyclerView UI. This demonstrated advanced knowledge of Android components, lifecycle management, and data handling, all wrapped in a responsive and user-centered interface.

