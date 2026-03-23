# 🚀 DevDaily

**DevDaily** is a high-performance, disciplined growth tracker built with Flutter. Designed for software engineers, it bridges the gap between technical preparation (DSA, System Design, Interviews) and personal consistency (Communication, Mindfulness, Naam Jaap).

---

## ✨ Key Features

- **Activity Logging:** Categorized tracking for DSA, Interview Prep, and Habits.
- **Data Visualization:** Beautiful progress insights using `fl_chart`.
- **Offline First:** Lightning-fast local persistence with Isar NoSQL database.
- **Reactive UI:** Instant state synchronization across screens using Riverpod.

## 🏗 Architecture & Tech Stack

This project follows **Feature-First Clean Architecture**, ensuring the code is scalable, testable, and maintainable.

* **Framework:** Flutter (Material 3)
* **State Management:** `Riverpod 2.x` (AsyncNotifier)
* **Local Database:** `Isar` (NoSQL)
* **Navigation:** `GoRouter` (Declarative Routing)
* **Code Generation:** `build_runner`, `isar_generator`



## 📂 Project Structure

The project is organized by features to keep the codebase decoupled:

```text
lib/
├── core/               # Global constants, themes, and shared utilities
├── routes/             # App routing logic (GoRouter)
└── features/           # Independent feature modules
    ├── home/           # Dashboard and Analytics
    │   ├── model/
    │   ├── notifiers/
    │   └── presentation/
    └── tasks/          # Task management and History
        ├── model/
        ├── repository/
        ├── provider/
        └── presentation/