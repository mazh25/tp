# Ma Zhiheng’s Project Portfolio Page

## Project: FitnessOne

**FitnessOne** is a desktop fitness management application designed for coaches to manage their athletes’ training sessions, exercises, and calorie intake. It provides a Command Line Interface (CLI) for efficient command input and a JavaFX-based Graphical User Interface (GUI) for better user interaction. The project is written in Java and has around 10 kLoC.

---

## Summary of Contributions

### New Features Implemented

#### 1. Implemented view commands (`viewSession`, `viewAthlete`, `viewExercise`) and calorie intake management (`intake`)

**What it does:**  
These commands allow users to conveniently view detailed information about specific sessions, athletes, or exercises, and manage the athletes’ daily calorie intake through the `intake` command.  
The feature provides a clear interface for coaches to monitor athletes’ progress and balance their calorie consumption and expenditure.

**Justification:**  
These view and intake features significantly improve the usability of FitnessOne. They provide coaches with an intuitive and efficient way to check relevant information and record nutritional intake, which are essential functions for any professional fitness management system.

**Highlights:**  
Implementing these commands required integrating with multiple core components (`Athlete`, `Session`, and `Exercise`) and designing a new data class `CaloriesIntake` that parallels existing classes such as `Exercise` and `Session`. This demanded careful coordination of model updates and command parsing logic.

**Credits:**  
The command structure and parser design were inspired by the architecture of AddressBook-Level3. All other logic and data modeling were independently implemented.

---

### Core Code Contributions

- Designed and implemented the `CaloriesIntake` class as a new core component in the data model, supporting tracking and updating of calorie intake per athlete.
- Integrated calorie management logic into `Coach` and storage modules for persistent data handling.
- Developed `ViewSessionCommand`, `ViewAthleteCommand`, and `ViewExerciseCommand`, ensuring consistency with the existing `List` and `Add` command framework.
- Added validation and error handling logic to ensure robustness against invalid command parameters.
- **Wrote comprehensive JUnit tests** for all implemented commands (`viewSession`, `viewAthlete`, `viewExercise`, and `intake`) and for the new `CaloriesIntake` class, ensuring high reliability and correctness of command execution.

---

### Documentation Contributions

**User Guide (UG):**
- Authored and refined documentation for `viewSession`, `viewAthlete`, `viewExercise`, and `intake` commands.
- Ensured consistent style and formatting across all command descriptions.

**Developer Guide (DG):**
- Wrote implementation details, purpose, step-by-step logic, and error handling sections for the following commands:  
  `NewAthlete`, `NewExercise`, `NewSession`, `UndoExercise`, `UndoSession`, `UpdateSession`, `ViewAthlete`, `ViewExercise`, and `ViewSessions`.
- Created sequence diagrams and described internal control flow for these commands to help new developers understand the architecture.

---

### Project Management

- Contributed code through multiple pull requests and participated actively in team discussions.
- Maintained close coordination with other members to ensure consistent data model integration.

---

### Community

- Reviewed peers’ pull requests and provided feedback on command design consistency.
- Participated in code discussions and documentation alignment.

---

### Tools

- Utilized GitHub and IntelliJ IDEA for version control and collaborative development.
- Followed the project’s Gradle-based build system and JavaFX UI framework setup.
- Applied **JUnit 5** testing framework for automated testing and regression verification.

---

### Code Contributed

View my code contributions on **RepoSense**: [link to be inserted]
