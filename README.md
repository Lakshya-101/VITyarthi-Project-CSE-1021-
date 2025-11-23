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

Technologies/Tools Used:-

- **Python 3.13.9** – Core programming language  
- **Tkinter** – Standard Python GUI library for building the desktop interface, including ttk for modern-styled widgets and themed components.  
- **pandas** – Powerful data analysis library used for in-memory storage, manipulation, filtering, grouping, and aggregation of expense records via DataFrames.  
- **Matplotlib** – Industry-standard plotting library for generating the embedded daily expense trend line chart.  
- **FigureCanvasTkAgg** (from matplotlib.backends.backend_tkagg) – Backend that seamlessly integrates Matplotlib figures into the Tkinter window.  
- **datetime & matplotlib.dates** – For robust date parsing, validation, and proper axis formatting in graphs.  
- **tkinter.messagebox & filedialog** – Built-in dialogs for user feedback (success/error messages) and native file save/open operations during CSV export/import.

### Steps to Install & Run the Project:-

1. **Install Python 3**  
   Ensure Python 3.7 or higher is installed on your system.  
   Download from: https://www.python.org/downloads/

2. **Install Required Libraries**  
   Open a terminal/command prompt and run:  

         pip install pandas matplotlib
   
   (Tkinter is included with standard Python installations.)

4. **Save the Source Code**  
   Copy the complete provided code into a new file named `Finances_manager.py`  
   (or any name ending in `.py`).

5. **Run the Application**  
   In the terminal/command prompt, navigate to the folder containing the file and execute:  
   
   python Finances_manager.py
   
   Alternatively, double-click the file if your system is configured to run `.py` files with Python.

The application window (titled "Finance Expense Management App") will launch immediately, sized at 800×600 pixels. No additional configuration or internet connection is required.

**Note**: Data is stored in memory during the session. Use the "Export to CSV" feature before closing to save your expenses permanently.

### Instructions for Testing:-
Follow these steps to thoroughly verify all functionalities of the application:

1. **Basic Expense Addition**
    Open the "Add Expense" tab.
    Enter a valid date (e.g., 07-11-2025), amount (e.g., 15.50), select a category (e.g., Food), and add a description.
    Click "Add Expense" → Confirm success message and cleared fields.

2.**Input Validation**
    Try invalid inputs: wrong date format (e.g., 2025-11-07), non-numeric amount (e.g., abc), or no category selected.
    Expected: Clear error messages appear via pop-up.

3.**View & Filter Expenses**
    Switch to "View Expenses" tab → Click "Apply Filters".
    Table should display all added entries with correct total at the bottom.
    
4.**Test filtering:**
    Select a specific category → Only matching rows appear.
    Set a narrow date range → Only expenses within that period are shown.

5.**Analytics**
      Add 5–10 expenses across different dates and categories.
      Go to "Analytics" tab → Click "Generate Analytics".
      Verify: Total, average, and category breakdown are accurate.

6.**Graph Generation**
      In "Analytics" tab, click "Generate Graph".
      A line chart should appear showing daily totals with properly labeled and rotated dates.

7.**Data Persistence (Export/Import)**
    Go to "Export/Import" → Click "Export to CSV" → Save the file.
    Close and restart the app (data should be gone).
    Click "Import from CSV" → Select the saved file → Data should reload completely.
    Test invalid CSV (wrong columns or format) → Error message should appear.

Edge Cases
Start the app with no expenses → All tabs should handle empty state gracefully.
Add expenses on the same date → Graph and analytics should aggregate correctly.
