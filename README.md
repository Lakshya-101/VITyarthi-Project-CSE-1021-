# VITyarthi-Project-CSE-1021
VITyarthi Project - 

Project Title - Finance Expense management app

Overview of The Project:-

The Finance Expense Management App is a lightweight, fully offline Python desktop application designed specifically for college students to track and manage daily expenses effectively. Built with Tkinter, it features a clean tabbed interface allowing users to add expenses, filter and view records, generate basic analytics, visualize spending trends with an embedded line chart which utilizes mathplotlib, and export/import data via CSV. All data is stored in memory using pandas, requiring no internet or database. It promotes financial awareness through simplicity, speed, and portability—ideal for students on a budget.

Features:-

- **Add Expense**  
  User-friendly form to record expenses with automatic validation:  
  - Date (YYYY-MM-DD format)  
  - Amount (numeric only)  
  - Predefined categories: Food, Transportation, Entertainment, Utilities, Other  
  - Optional description  
  Instant feedback via success/error message boxes and automatic field clearing after submission.

- **View Expenses**  
  Interactive, sortable table displaying all recorded expenses with:  
  - Real-time filtering by category (including “All”) and custom date range  
  - Vertical scrollbar for large datasets  
  - Dynamic total summary showing the sum of filtered expenses (e.g., “Total Expenses: $342.50”)  
  Category dropdown and date fields auto-populate with existing data when the tab is selected.

- **Analytics**  
  One-click generation of key financial insights:  
  - Total and average expense amounts  
  - Detailed breakdown of spending by category (e.g., Food: $180.00)  
  Results displayed in a clear, readable text area.

- **Graphical Visualization**  
  Embedded line chart showing daily expense trends over time:  
  - Automatically groups expenses by date  
  - Uses markers and grid for readability  
  - Properly formatted date axis with rotation for clarity  
  Chart updates instantly on button press and replaces any previous graph.

- **Export/Import via CSV**  
  Full data persistence:  
  - Export all expenses to a standard CSV file (with column headers)  
  - Import previously saved CSV files to restore or merge data  
  Strict validation ensures imported files have the exact required columns (Date, Amount, Category, Description).

- **Additional Highlights**  
  - Completely offline — no internet, accounts, or databases required  
  - Input validation and helpful error messages throughout  
  - Responsive tabbed interface with automatic UI updates  
  - Lightweight single-file design for easy distribution and use

