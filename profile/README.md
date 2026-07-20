# Mobile Programming HWs

Coursework projects for the Mobile Programming course at Sharif University of Technology.

These repositories are small mobile programming projects with runnable code, screenshots, setup notes, and focused implementation details. I keep them as course work and as a place to clean up older projects over time.

Project hub: [mobile-programming-hws.github.io](https://mobile-programming-hws.github.io/)

## Projects

| Repo | App | Main Idea |
| --- | --- | --- |
| [HW1](https://github.com/Mobile-Programming-HWs/HW1) | Terminator | Course browser and weekly schedule planner |
| [HW2](https://github.com/Mobile-Programming-HWs/HW2) | Quiz of Kings | Trivia game with local users and scores |
| [Project](https://github.com/Mobile-Programming-HWs/Project) | MicroMaster | Course and homework management app |
| [Swift](https://github.com/Mobile-Programming-HWs/Swift) | Crypto Tracker | Swift cryptocurrency tracker with terminal and SwiftUI flows |
| [mobile-programming-hws.github.io](https://github.com/Mobile-Programming-HWs/mobile-programming-hws.github.io) | Project site | GitHub Pages hub with screenshots and source links |
| [.github](https://github.com/Mobile-Programming-HWs/.github) | Org profile | Public profile and repo overview |

## HW1: Terminator

[Terminator](https://github.com/Mobile-Programming-HWs/HW1) is an Android app for browsing Sharif course data and building a weekly class plan.

- Loads bundled JSON course data from the app resources.
- Groups courses by department.
- Supports search by course name, instructor, number, or id.
- Shows course details, class time, exam time, units, and capacity.
- Checks duplicate courses, class conflicts, and exam conflicts.
- Saves selected courses locally.

<p>
  <a href="https://github.com/Mobile-Programming-HWs/HW1">
    <img src="https://raw.githubusercontent.com/Mobile-Programming-HWs/HW1/main/docs/screenshots/course-list.png" width="190" alt="Terminator course list">
  </a>
  <a href="https://github.com/Mobile-Programming-HWs/HW1">
    <img src="https://raw.githubusercontent.com/Mobile-Programming-HWs/HW1/main/docs/screenshots/weekly-chart.png" width="190" alt="Terminator weekly chart">
  </a>
  <a href="https://github.com/Mobile-Programming-HWs/HW1">
    <img src="https://raw.githubusercontent.com/Mobile-Programming-HWs/HW1/main/docs/screenshots/course-details.png" width="190" alt="Terminator course details">
  </a>
</p>

## HW2: Quiz of Kings

[Quiz of Kings](https://github.com/Mobile-Programming-HWs/HW2) is a multiple-choice trivia app with local accounts, settings, and a scoreboard.

- Registers and logs in local users.
- Stores user settings and scores with Room.
- Fetches live questions from Open Trivia DB.
- Falls back to cached questions when needed.
- Tracks score, progress, category, difficulty, and question count.
- Includes profile, settings, navigation drawer, and scoreboard screens.

<p>
  <a href="https://github.com/Mobile-Programming-HWs/HW2">
    <img src="https://raw.githubusercontent.com/Mobile-Programming-HWs/HW2/main/docs/screenshots/game.png" width="180" alt="Quiz of Kings game screen">
  </a>
  <a href="https://github.com/Mobile-Programming-HWs/HW2">
    <img src="https://raw.githubusercontent.com/Mobile-Programming-HWs/HW2/main/docs/screenshots/question.png" width="180" alt="Quiz of Kings question screen">
  </a>
  <a href="https://github.com/Mobile-Programming-HWs/HW2">
    <img src="https://raw.githubusercontent.com/Mobile-Programming-HWs/HW2/main/docs/screenshots/scoreboard.png" width="180" alt="Quiz of Kings scoreboard">
  </a>
</p>

## Project: MicroMaster

[MicroMaster](https://github.com/Mobile-Programming-HWs/Project) is the final project app for managing courses, homework, and user roles.

- Registers teachers, TAs, and students.
- Lets teachers create courses and add homework links.
- Lets students enroll in courses.
- Lets TAs request course access.
- Stores users, courses, enrollments, TA records, and homework links in Room.
- Shows profile data, course counts, homework counts, and homework file status.

<p>
  <a href="https://github.com/Mobile-Programming-HWs/Project">
    <img src="https://raw.githubusercontent.com/Mobile-Programming-HWs/Project/main/docs/screenshots/courses.png" width="170" alt="MicroMaster course list">
  </a>
  <a href="https://github.com/Mobile-Programming-HWs/Project">
    <img src="https://raw.githubusercontent.com/Mobile-Programming-HWs/Project/main/docs/screenshots/course-detail.png" width="170" alt="MicroMaster course detail">
  </a>
  <a href="https://github.com/Mobile-Programming-HWs/Project">
    <img src="https://raw.githubusercontent.com/Mobile-Programming-HWs/Project/main/docs/screenshots/profile.png" width="170" alt="MicroMaster profile">
  </a>
</p>

## Swift: Crypto Tracker

[Crypto Tracker](https://github.com/Mobile-Programming-HWs/Swift) is a Swift cryptocurrency tracker with a terminal app and a SwiftUI playground.

- Lists default cryptocurrencies with today's price.
- Opens a detail flow by id, name, or symbol.
- Shows daily price history for a selected date range.
- Shows first, last, low, high, average, and change.
- Prints a selected price range as CSV.
- Adds and deletes cryptocurrencies with validation.
- Includes a profile tab and username editing.
- Includes the assignment PDF, sample session, screenshots, and tests.

<p>
  <a href="https://github.com/Mobile-Programming-HWs/Swift">
    <img src="https://raw.githubusercontent.com/Mobile-Programming-HWs/Swift/main/docs/screenshots/terminal-home.svg" width="210" alt="Crypto Tracker terminal home">
  </a>
  <a href="https://github.com/Mobile-Programming-HWs/Swift">
    <img src="https://raw.githubusercontent.com/Mobile-Programming-HWs/Swift/main/docs/screenshots/terminal-history.svg" width="210" alt="Crypto Tracker price history">
  </a>
  <a href="https://github.com/Mobile-Programming-HWs/Swift">
    <img src="https://raw.githubusercontent.com/Mobile-Programming-HWs/Swift/main/docs/screenshots/swiftui-preview.svg" width="210" alt="Crypto Tracker SwiftUI preview">
  </a>
</p>

## Setup

The Android apps use:

- Android Studio
- JDK 17
- Android SDK Platform 32
- A local Android emulator or Android device

Build any app from its repo folder:

```powershell
.\gradlew.bat :app:assembleDebug
```

Install a debug build on a running emulator:

```powershell
adb devices
.\gradlew.bat :app:installDebug
```

The Swift project uses:

- Swift 5.9 or newer
- Xcode or Swift Playgrounds for the SwiftUI playground

Run the Swift terminal app from its repo folder:

```powershell
swift run crypto-tracker
```

Run Swift tests:

```powershell
swift test
```

## Repo Notes

- Each project has its own README with setup steps, screenshots, and implementation notes.
- The screenshots are stored under `docs/screenshots` in each project repo.
- The Android apps are course projects, so the package names and older dependency choices are kept conservative unless a change is needed.
- The GitHub Pages site links the public repos and shows a browsable project overview.
