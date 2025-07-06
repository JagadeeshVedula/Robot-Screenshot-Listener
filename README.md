# Expense Statement App

This project is an Android application designed to read messages containing transaction details and sort expenses for the month into a formatted statement. It utilizes Python for the backend logic.

## Project Structure

```
expense-statement-app
├── src
│   ├── main.py               # Entry point of the application
│   ├── message_reader.py      # Handles reading and filtering messages
│   ├── expense_parser.py      # Parses and sorts expense details
│   └── statement_generator.py  # Generates and saves the expense statement
├── requirements.txt           # Lists project dependencies
└── README.md                  # Project documentation
```

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/expense-statement-app.git
   cd expense-statement-app
   ```

2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

## Usage

1. Run the application:
   ```
   python src/main.py
   ```

2. The application will fetch messages from your device, filter for transaction details, parse the expenses, and generate a monthly statement.

## Contributing

Feel free to submit issues or pull requests if you have suggestions or improvements for the project.

## License

This project is licensed under the MIT License. See the LICENSE file for details.