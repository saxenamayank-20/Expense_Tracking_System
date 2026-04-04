# 💰 Expense Tracking System

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.120.0-green.svg)](https://fastapi.tiangolo.com/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.51.0-red.svg)](https://streamlit.io/)
[![MySQL](https://img.shields.io/badge/MySQL-Connector-orange.svg)](https://dev.mysql.com/doc/connector-python/en/)

A modern, user-friendly expense tracking application built with **FastAPI** for the backend and **Streamlit** for the frontend. Track your expenses, analyze spending patterns, and manage your finances effortlessly!

## ✨ Features

- 📊 **Expense Management**: Add, update, and delete expenses with ease
- 📈 **Analytics Dashboard**: Visualize spending patterns with interactive charts
- 🗂️ **Category-based Tracking**: Organize expenses by categories
- 📅 **Date Range Filtering**: Analyze expenses over specific time periods
- 💾 **MySQL Database**: Robust data storage with persistent records
- 🚀 **FastAPI Backend**: High-performance REST API
- 🎨 **Streamlit Frontend**: Beautiful, responsive web interface
- 🔐 **User Authentication**: Secure user management system

## 🏗️ Project Structure

```
Expense_Tracking_System/
├── backend/
│   ├── __init__.py
│   ├── database_helper.py    # Database operations
│   ├── logging_setup.py      # Logging configuration
│   └── server.py             # FastAPI server
├── frontend/
│   ├── app.py                # Main Streamlit app
│   ├── add_update_ui.py      # Add/Update expense interface
│   └── analytics_ui.py       # Analytics dashboard
├── testing/
│   ├── __init__.py
│   └── backend/
│       ├── __init__.py
│       └── test_database_helper.py
├── requirements.txt          # Python dependencies
└── README.md
```

## 🚀 Quick Start

### Prerequisites

- Python 3.8 or higher
- MySQL Server
- Git

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/saxenamayank-20/Expense-Tracking-System.git
   cd Expense-Tracking-System
   ```

2. **Create a virtual environment** (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up MySQL database**:
   - Create a new MySQL database
   - Update database connection settings in `backend/database_helper.py`

### Running the Application

1. **Start the FastAPI backend**:
   ```bash
   uvicorn backend.server:app --reload
   ```
   The API will be available at `http://localhost:8000`

2. **Start the Streamlit frontend**:
   ```bash
   streamlit run frontend/app.py
   ```
   The app will open in your browser at `http://localhost:8501`

## 📖 Usage

### Adding Expenses
- Navigate to the "Add/Update" tab
- Enter expense details: amount, category, notes, and date
- Click "Add Expense" to save

### Viewing Analytics
- Switch to the "Analytics" tab
- View spending summaries and charts
- Filter by date range or category

### API Endpoints
- `GET /expenses` - Retrieve all expenses
- `POST /expenses` - Add a new expense
- `PUT /expenses/{id}` - Update an expense
- `DELETE /expenses/{id}` - Delete an expense
- `GET /analytics` - Get spending analytics

## 🧪 Testing

Run the test suite:
```bash
python -m pytest testing/
```

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

⭐ **Star this repo** if you find it helpful!