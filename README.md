# Budget Tracker - Personal Finance Management

[![Python](https://img.shields.io/badge/Python-3.6+-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Active-brightgreen.svg)](https://github.com/ShubhG7/Budget-Tracker---Personal-Finance-Management)

A comprehensive desktop application built with Python for personal finance management. Track your budgets, manage expenses, and visualize your spending patterns through an intuitive graphical interface.

## 🚀 Features

- **User Authentication**: Secure login and registration system
- **Budget Management**: Set and track monthly budgets with dates
- **Expense Tracking**: Record individual expenses with categories and dates
- **Data Visualization**: Interactive pie charts showing spending vs. remaining budget
- **Data Management**: Sort, filter, and delete financial records
- **User Isolation**: Separate data storage for each user account
- **Real-time Validation**: Prevents overspending beyond budget limits

## 📋 Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Technology Stack](#technology-stack)
- [Database Schema](#database-schema)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)

## 🛠️ Installation

### Prerequisites

- Python 3.6 or higher
- pip package manager

### Dependencies

Install the required packages:

```bash
pip install tkcalendar
pip install matplotlib
```

### Setup

1. Clone the repository:
```bash
git clone https://github.com/ShubhG7/Budget-Tracker---Personal-Finance-Management.git
cd Budget-Tracker---Personal-Finance-Management
```

2. Run the application:
```bash
python BudTracker.py
```

## 🎯 Usage

### Getting Started

1. **Launch the Application**: Run `python BudTracker.py`
2. **Create Account**: Click "Create Account" to register a new user
3. **Login**: Use your credentials to access the application
4. **Navigate Tabs**: Use the three main tabs for different functions

### Budget Management

- **Add Budget**: Enter amount and select date, then click "Add Amount"
- **View Budgets**: See all budget entries in the sortable table
- **Delete Entries**: Remove individual or all budget entries
- **Sort Data**: Click column headers to sort by amount or date

### Expense Tracking

- **Record Expenses**: Add item name, cost, and date
- **Budget Validation**: System prevents overspending
- **View History**: Track all expenses in chronological order
- **Manage Data**: Delete specific expenses or clear all data

### Data Visualization

- **Generate Graphs**: Click "Graph It!" to create pie charts
- **Analyze Spending**: Visual representation of budget vs. expenses
- **Color Coding**: Red for spent money, gold for remaining budget

## ✨ Features

### User Interface
- **Tabbed Interface**: Organized into Budget, Expense, and Graph sections
- **Responsive Design**: Clean, intuitive layout with proper spacing
- **Data Tables**: Sortable tables with real-time updates
- **Form Validation**: Input validation and error handling

### Security
- **User Authentication**: Password-protected accounts
- **Data Isolation**: Separate storage for each user
- **Session Management**: Secure login/logout functionality

### Data Management
- **Real-time Updates**: Immediate table refresh after changes
- **Sorting Options**: Multiple sorting criteria for better organization
- **Bulk Operations**: Delete individual entries or clear all data
- **Data Persistence**: SQLite database for reliable storage

## 🏗️ Technology Stack

- **Backend**: Python 3.6+
- **GUI Framework**: Tkinter
- **Database**: SQLite3
- **Data Visualization**: Matplotlib
- **Date Handling**: tkcalendar
- **Enhanced UI**: tkinter.ttk

## 🗄️ Database Schema

The application uses SQLite with three main tables:

### Users Table
```sql
CREATE TABLE user (
    username TEXT NOT NULL,
    password TEXT NOT NULL
);
```

### Budget Table
```sql
CREATE TABLE budget (
    username TEXT NOT NULL,
    amount INT NOT NULL,
    date TEXT NOT NULL
);
```

### Expenses Table
```sql
CREATE TABLE expenses (
    username TEXT NOT NULL,
    cost INT NOT NULL,
    date TEXT NOT NULL,
    item TEXT NOT NULL
);
```

## 📱 Screenshots

*Screenshots will be added here to showcase the application interface*

## 🔧 Project Structure

```
Budget-Tracker---Personal-Finance-Management/
├── BudTracker.py          # Main application file
├── db.db                  # SQLite database
├── README.md              # This file
└── requirements.txt       # Python dependencies
```

## 🚧 Future Enhancements

- [ ] Export functionality (PDF/Excel reports)
- [ ] Expense categorization system
- [ ] Recurring expense scheduling
- [ ] Budget alerts and notifications
- [ ] Data backup and restore
- [ ] Advanced analytics and forecasting
- [ ] Mobile app companion
- [ ] Cloud synchronization

## 🤝 Contributing

We welcome contributions! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

### How to Contribute

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


---

⭐ **Star this repository if you find it helpful!**

🔗 **Connect with us**: [GitHub](https://github.com/ShubhG7) | [Project Link](https://github.com/ShubhG7/Budget-Tracker---Personal-Finance-Management) 
