# statement.md

### Problem Statement:-

College students typically operate on tight and irregular budgets sourced from pocket money, part-time jobs, or scholarships. Frequent small expenditures on food, transportation, entertainment, and utilities often go untracked, leading to overspending, confusion about where money disappears, and financial stress toward the end of each month. Many existing expense-tracking solutions are either overly complex, advertisement-heavy, subscription-based, or require constant internet access, making them impractical for students who need a simple, private, and instantly accessible tool. This project addresses the clear need for a lightweight, completely offline, and user-friendly expense manager tailored specifically to the daily financial realities and limited technical setup of college students.

### Scope of the project:-

The project delivers a fully functional, standalone, offline desktop expense tracking application built as a single Python script. It provides college students with an easy-to-use tool to record, manage, and understand their daily spending without requiring internet access, user accounts, or external databases.

**In-Scope Features:**
- Add, view, filter, and analyze expenses via an intuitive tabbed GUI
- Support for Date, Amount, Category (Food, Transportation, Entertainment, Utilities, Other), and Description
- Real-time filtering by category and custom date range with total calculation
- Basic analytics: total spent, average expense, and category-wise breakdown
- Embedded line chart visualizing daily spending trends
- Full data export and import using standard CSV format for persistence across sessions
- Comprehensive input validation and user-friendly error handling

**Technical Scope:**
- Built using only Tkinter (standard library), pandas, and Matplotlib
- Single-file implementation (no additional modules or configuration files)
- In-memory storage using pandas DataFrame
- Cross-platform compatibility (Windows, macOS, Linux)

**Out of Scope:**
- Cloud synchronization or multi-device access
- User authentication or multiple profiles
- Advanced budgeting, forecasting, or recurring expenses
- Mobile or web versions
- Database storage (SQLite, etc.)
- Currency conversion or receipt scanning

### Target Users:-

**Primary Audience:** 
College and university students managing limited and irregular budgets (pocket money, part-time earnings, scholarships).
**Secondary Audience:** 
High school students, fresh graduates, or anyone seeking a simple, private, and completely free expense tracker.
Beginner Python learners looking for a clean, well-structured, real-world Tkinter + pandas + Matplotlib project to study or modify.

