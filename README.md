BudgetBuddy
BudgetBuddy is a Python-based web app designed for the HackSphere High School Community Finance Hackathon to help low-income families manage budgets and reduce financial stress. Built with Flask, SQLite, scikit-learn, and Matplotlib, it offers an AI-powered Smart Budget Planner, Expense Tracker, Community Resources, and an Expense Risk Forecaster, prioritizing accessibility for users with limited financial literacy. This app empowers families to achieve financial stability through simple, community-focused tools.
Features

Smart Budget Planner: Users input income (e.g., daily wages) and expenses (e.g., rent). A linear regression model (scikit-learn) suggests a weekly budget, prioritizing essentials.
Expense Tracker: Log daily expenses via a form, with spending trends visualized in a Matplotlib bar chart.
Community Resources: Select a location from a dropdown to access links to local aid programs (e.g., food banks).
Expense Risk Forecaster: An AI model predicts budget overruns based on spending patterns, suggesting cost-saving tips (e.g., "Cook at home").

Tech Stack

Language: Python
Web Framework: Flask (frontend and backend)
Database: SQLite (stores budgets and expenses)
AI: scikit-learn (linear regression for budgeting and risk forecasting)
Visualization: Matplotlib (spending charts)
Styling: Bootstrap (mobile-responsive, accessible UI)

Prerequisites

Python 3.8 or higher
pip (Python package manager)
A web browser (e.g., Chrome, Firefox)
Optional: REPL.it or VS Code for development

Setup Instructions

Clone or Download the Project

Download the project files or clone the repository (if hosted).
Ensure the following files are present:
app.py: Main Flask app
model.py: AI model logic
templates/: HTML templates (budget.html, tracker.html, resources.html)
static/: CSS and chart images




Install Dependencies

Open a terminal in the project directory.
Run:pip install flask sqlite3 scikit-learn matplotlib numpy




Initialize the Database

The app automatically creates a data.db SQLite file on first run to store expenses.


Run the App

In the terminal, navigate to the project directory and run:python app.py


Open a browser and go to http://localhost:5000 (or the URL provided by REPL.it).


Test the App

Navigate to the Budget Planner, enter sample income (e.g., $100) and expenses (e.g., $50 rent).
Log expenses in the Expense Tracker and view the spending chart.
Select a location in Community Resources to see aid links.
Check the Expense Risk Forecaster for budget alerts.



File Structure
budgetbuddy/
├── app.py              # Main Flask app with routes
├── model.py            # AI model (linear regression)
├── data.db             # SQLite database (auto-generated)
├── templates/          # HTML templates
│   ├── budget.html
│   ├── tracker.html
│   └── resources.html
├── static/             # CSS and chart images
│   ├── style.css
│   └── chart.png
└── README.md           # This file

Usage

Budget Planner: Enter weekly income and expenses to get a suggested budget.
Expense Tracker: Log daily expenses (e.g., $5 for food) and view a chart of spending by category.
Community Resources: Choose a location to access financial aid links.
Risk Forecaster: Receive alerts if spending risks exceeding your budget, with tips to save.

Hackathon Context
BudgetBuddy was built for the HackSphere High School Community Finance Hackathon (deadline: May 11, 2025). It addresses the challenge of developing a Python-based finance app that strengthens communities. The app tackles financial stress in low-income families, incorporates AI for risk management, and ensures accessibility, aligning with the hackathon’s goals.
Troubleshooting

Flask not found: Ensure dependencies are installed (pip install flask).
Chart not displaying: Verify Matplotlib saved chart.png to static/.
Database errors: Check data.db permissions or reinitialize with init_db() in app.py.
AI predictions off: Ensure sample data in model.py is valid.

Team

Developed by [Your Team Name] for HackSphere 2025.
Roles: [List roles, e.g., frontend, AI, database, or leave blank if solo].

License
This project is for educational purposes and submitted to the HackSphere Hackathon. No formal license is applied.
![Screenshot 2025-05-08 171752](https://github.com/user-attachments/assets/1ddfe780-ab99-4961-9d19-bebd0954574c)
