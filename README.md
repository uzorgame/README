# Sudoku Uzor: Professional Flutter Showcase

This repository serves as a professional showcase for **Sudoku Uzor**, a fully-featured Sudoku game developed and published to the Google Play Store by Nahreba Mykhailo in **2 months**.

The project demonstrates a mature, production-ready approach to mobile development, focusing on performance, monetization, and clean architecture.

<br />

<p align="center">
  <a href="https://play.google.com/store/apps/details?id=com.sudoku.uzor">
    <img alt="Get it on Google Play" src="https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png" width="250"/>
  </a>
</p>

<br />

##  Key Features and UX/UI

* **Robust Game Modes:** Implemented multiple game logics including Classic, Daily Challenges, Battle, and Championship modes.
* **Adaptive Design:** Utilizes `LayoutScale` and custom adaptive layouts to ensure a seamless experience on compact phones and large tablets.
* **Performance-Driven UX:** Features custom animations, gradient use, haptic feedback, and instant user feedback (Combo toasts) for enhanced UX.
* **Localization & Customization:** Full support for locale switching, theme switching (Dark/Light), and dynamic font scaling.

---

##  Architecture and Engineering Solutions

### Core Stack
* **Framework:** Flutter, Dart
* **State Management:** `Provider` (using `MultiProvider` for structured global state aggregation).
* **Monetization & Tracking:** `Firebase Analytics` and `Google Mobile Ads`.

### Advanced Solutions
1.  **Performance Optimization (Isolates):**
    * Implemented asynchronous game state serialization (save/load) using `compute` Isolates to prevent UI thread blocking (`jank`) during heavy I/O operations.
2.  **Effective Monetization Strategy (Ad Service):**
    * Designed a specialized service for `Rewarded Ads` that proactively **pre-caches** inventory, handles complex **retry logic** with back-off, and properly manages ad showing based on the app's life cycle (background/foreground) to maximize fill rate and minimize `Ad_failed` errors.
3.  **Complex State Management:**
    * `ComboController` and other game logic controllers handle sequential, time-sensitive, and overlay-dependent scenarios cleanly, demonstrating high-level state control without duplication.

---

##  Code Quality & Professional Audit

The project underwent an AI-powered code quality analysis, providing an objective assessment of the development level.

> ### **Developer Level: Strong Middle (on the path to Senior)**
>
> **Summary:** The solution reflects an experienced developer's approach. Skills include building complex business logic, integrating external services, designing a reactive UI, and optimizing performance.
>
> **Key Strengths:** Effective use of `compute` Isolates, clean life-cycle management (ChangeNotifier, StatefulWidget), and proactive resource handling (e.g., ad pre-loading).
>
> **Growth Areas (Focus for Senior):** Recommended next steps include implementing automated behavioral tests and standardizing configuration/secrets management (Ad IDs, keys) outside of the codebase.

---

##  Source Code Access Policy

As **Sudoku Uzor** is a published, commercial product, the source code is maintained in a private repository to protect intellectual property.

I am prepared to **provide a live code walkthrough** during a technical interview to showcase the architecture and discuss the logic behind key services (Ad Service, State Controller, Serialization) in detail.

---

##  Contact

**Nahreba Mykhailo**

* **LinkedIn:** ---
* **Website:** https://uzorgame.github.io/
* **Email:** NagrebaMM@gmail.com
* **Telegram:** @uzormn
