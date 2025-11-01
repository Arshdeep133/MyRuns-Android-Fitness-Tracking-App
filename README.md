# MyRuns Android Application

The **MyRuns Android Application** is a comprehensive fitness tracking app designed to record, visualize, and manage users’ physical activities. It allows users to create personal profiles, log exercises, and analyze their workout data over time. The application was developed incrementally through multiple stages, each focusing on key components such as user interface design, profile management, database implementation, and activity tracking.

---

## 📱 Overview

**MyRuns** enables users to:
- Create and manage personal profiles with name, email, phone, gender, and major.
- Capture or select a profile photo from the camera or gallery.
- Record physical activities (e.g., walking, running, cycling) manually or automatically.
- View, edit, and delete exercise history.
- Store and display activity data in human-readable formats.
- Switch between metric and imperial units seamlessly.
- Navigate through a tabbed interface for different app sections (Start, History, Settings).

This project emphasizes Android development fundamentals including activity lifecycles, fragments, intents, data persistence, threading, and UI design with XML and Kotlin.

---

## 🧩 Application Structure

The project is composed of several key components that work together as one complete system:

### 1. **User Profile Management**
- Users can enter personal details such as name, email, phone number, gender, and major.
- Profile images can be captured via camera or selected from the gallery.
- Profile data is saved locally and automatically reloaded when the app restarts.

### 2. **User Interface & Navigation**
- The main screen features a tabbed interface with three fragments:
  - **Start Tab:** Allows users to begin a new activity or enter data manually.
  - **History Tab:** Displays a list of previously recorded exercises.
  - **Settings Tab:** Provides access to personal profile and unit preferences.
- UI states are preserved during screen rotations to ensure smooth user experience.

### 3. **Database Integration**
- All exercise entries are stored using **Room Database** for persistent local data storage.
- Users can add, view, and delete exercise entries efficiently.
- A background thread is used for database operations to ensure smooth performance.
- Distances and speeds are automatically converted to match the user’s selected measurement unit (Metric or Imperial).

---

## 🧰 Technologies Used

- **Language:** Kotlin  
- **UI Design:** XML (Android Layouts)  
- **Architecture:** MVVM (Model–View–ViewModel)  
- **Database:** Room (SQLite)  
- **Threading:** Kotlin Coroutines  
- **Navigation:** Fragments and TabLayout with ViewPager  
- **Lifecycle Management:** ViewModel, LiveData  
- **Image Handling:** Camera Intent and Gallery Picker  
- **Logging & Debugging:** Logcat, `Log.d()` and `println()` for debugging  
- **Build System:** Gradle  
- **IDE:** Android Studio  

---

## ⚙️ Key Functionalities

- Persistent storage of user data and exercise logs  
- Thread-safe database operations  
- Intuitive UI navigation using fragments and tabs  
- Dynamic unit conversion for distances and speeds  
- Camera and gallery integration for profile images  
- Real-time state management during configuration changes  
- Error handling through logging and crash analysis via Logcat  

---

## 🧪 Development Notes

During development:
- UI design variations across Android versions were expected, and focus remained on **functionality** rather than appearance.
- Some features such as map visualization were designed for later stages but can be extended easily.
- The project was tested for stability under **normal usage conditions** (i.e., when permissions are granted and inputs are valid).  
- Crashes due to unexpected or invalid user behavior (e.g., denying permissions) were not penalized but addressed when possible.

---

## 🚀 Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/MyRuns.git
