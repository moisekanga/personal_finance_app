# Personal Finance Dashboard

A simple yet powerful personal finance dashboard built with Streamlit that helps you track, categorize, and visualize your expenses.

![Personal Finance Dashboard](https://streamlit.io/images/brand/streamlit-logo-secondary-colormark-darktext.png)

## Features

- **CSV Import**: Easily import your bank statements in CSV format
- **Expense Categorization**: Automatically categorize your expenses based on transaction details
- **Visual Analytics**: View your spending patterns with interactive charts
- **Custom Categories**: Create and manage custom expense categories
- **Expense Tracking**: Track both debits (expenses) and credits (income)

## Demo

Upload your bank statement CSV file and instantly see your finances visualized with charts and breakdowns by category.

## Getting Started

### Prerequisites

- Python 3.7 or higher
- pip (Python package installer)

### Installation

1. **Clone the repository**

```bash
git clone https://github.com/yourusername/personal_finance_app.git
cd personal_finance_app
```

2. **Install required packages**

```bash
pip install -r requirements.txt
```
If there's no requirements.txt file, install the necessary packages:

```bash
pip install streamlit pandas plotly
```

### Usage

1. **Run the application**

```bash
streamlit run main.py
```

2. **Upload your bank statement**

- Use the file uploader to import your bank statement CSV file
- For testing, you can use the sample bank statements provided:
  - `sample_bank_statement_usd.csv` (USD currency)

3. **Categorize your expenses**

- The app will attempt to automatically categorize your expenses
- You can add new categories and manually assign transactions to categories
- Save your changes to improve future automatic categorization

4. **Analyze your finances**

- View the expense breakdown by category
- See total credits (income) and debits (expenses)
- Analyze spending patterns with interactive charts

## CSV File Format

Your bank statement CSV should have the following columns:
- `Date`: Transaction date (format: DD MMM YYYY, e.g., "15 Jan 2023")
- `Details`: Transaction description
- `Amount`: Transaction amount (can include commas for thousands)
- `Currency`: Currency code (USD, EUR, etc.)
- `Debit/Credit`: Whether the transaction is a "Debit" or "Credit"
- `Status`: Transaction status (e.g., "SETTLED", "REVERSED")

Example:
```
Date,Details,Amount,Currency,Debit/Credit,Status,
15 Jan 2023,Salary Deposit,"5,250.00",USD,Credit,SETTLED,
18 Jan 2023,AMAZON.COM,"89.99",USD,Debit,SETTLED,
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the Unlicense - see the [LICENSE](LICENSE) file for details.