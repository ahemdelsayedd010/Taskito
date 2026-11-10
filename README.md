# 📝 Taskito

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white" alt="Platform" />
  <img src="https://img.shields.io/badge/Language-Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white" alt="Language" />
  <img src="https://img.shields.io/badge/UI-Jetpack%20Compose%20%2B%20Material3-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white" alt="UI" />
  <img src="https://img.shields.io/badge/Architecture-MVVM-FF6F00?style=for-the-badge" alt="Architecture" />
  <img src="https://img.shields.io/badge/Database-Room-00599C?style=for-the-badge&logo=sqlite&logoColor=white" alt="Database" />
  <img src="https://img.shields.io/badge/Min%20SDK-24-success?style=for-the-badge" alt="Min SDK" />
</p>

**Taskito** is a sleek, modern Android productivity application built with Kotlin, Jetpack Compose, Material Design 3, and Room Database. It helps users organize daily tasks, set priorities and deadlines, track productivity habits, and analyze completion metrics with intuitive charts and insights.

---

## 📱 App Preview & Screenshots

<div align="center">
  <table>
    <tr>
      <td align="center" width="33%">
        <b>📅 Calendar & Task List</b><br/><br/>
        <img src="screenshots/task_list_calendar.jpeg" width="100%" alt="Task List & Calendar Screen" />
      </td>
      <td align="center" width="33%">
        <b>➕ Add New Task</b><br/><br/>
        <img src="screenshots/add_task.jpeg" width="100%" alt="Add Task Screen" />
      </td>
      <td align="center" width="33%">
        <b>📊 Analytics & Insights</b><br/><br/>
        <img src="screenshots/analytics_insights.jpeg" width="100%" alt="Analytics & Insights Screen" />
      </td>
    </tr>
  </table>
</div>

---

## ✨ Features

- **📅 Interactive Calendar & Day View:** Browse and manage tasks for any selected date on the calendar.
- **⚡ Swipe-to-Delete with Undo:** Easily delete tasks with a left swipe and restore them instantly with Snackbar Undo.
- **🏷️ Priority & Color Tagging:** Assign priority levels (High, Medium, Low) and custom color tags to structure your workflow.
- **🎯 Task Deadlines:** Select task due dates using a Material Date Picker dialog.
- **📊 Productivity Insights & Analytics (Compose):**
  - **Completion Rate Gauge:** Real-time percentage indicator of finished vs. pending tasks.
  - **Streak & Overdue Counter:** Track active streaks and monitor overdue obligations.
  - **Weekly Activity Chart:** Custom Compose bar graph showing daily completion activity (Mon–Sun).
  - **Priority Breakdown:** Visual distribution bar of high, medium, and low priority tasks.
- **💾 Offline First:** Persistent data storage using Room DB and Kotlin Flow for real-time UI updates.

---

## 🛠️ Tech Stack & Architecture

- **Language:** 100% [Kotlin](https://kotlinlang.org/)
- **UI Framework:** [Jetpack Compose](https://developer.android.com/jetpack/compose) & Material Design 3 XML Views
- **Architecture:** MVVM (Model-View-ViewModel) + Unidirectional Data Flow
- **Local Database:** [Room Database](https://developer.android.com/training/data-storage/room) with KSP
- **Asynchronous Programming:** Kotlin Coroutines & `StateFlow`
- **Navigation:** AndroidX Jetpack Navigation Component
- **Build System:** Gradle KTS with Version Catalog (`libs.versions.toml`), AGP 9.4+

---

## 📁 Repository Structure

```
Taskito2/
├── app/
│   ├── src/main/java/com/example/taskito/
│   │   ├── analytics/        # Jetpack Compose Insights & Charts
│   │   ├── db/               # Room Database, DAO & App Database
│   │   ├── model/            # Data Models (Task) & Repository
│   │   ├── view/             # Fragments, Host, AddTask & Adapters
│   │   └── viewmodel/        # TaskViewModel & Factory
│   └── src/main/res/         # XML layouts, navigation graph & drawables
├── screenshots/              # High-resolution app preview screenshots
└── README.md
```

