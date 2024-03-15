# MinorProject-1.1
# SQL Injection Scanner

This is a simple SQL injection scanner built with Python and Flask, designed to identify potential SQL injection vulnerabilities in web applications.

## Features

- Detects various types of SQL injection attacks, including:
  - Generic SQL Injection
  - Error Based Injection
  - Union Select Injection
  - Authentication Bypass Injection

- Uses a database to store and manage SQL injection payloads for testing.

## Setup

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/cyb3rcr4t0712/sql-injection-scanner.git```

2. **Install Dependencies:**

```pip install -r requirements.txt```

3. **Configure Database:**
- Choose a database management system (SQLite, MySQL, PostgreSQL, etc.).
- Set up a database and configure the connection in `app.py`.

4. **Run the Application:**
   ``python app.py``

## Usage

1. **Scan URLs for SQL Injection:**
- Send POST requests to `/scan` endpoint with JSON payload containing the URL to scan.
- Example:
  ```json
  {
      "url": "http://example.com/page.php?id=1"
  }
  ```

2. **View Results:**
- The scanner will return a JSON response containing any detected SQL injection vulnerabilities.

## Contributing

Contributions are welcome! If you'd like to improve this project, please fork the repository and submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Disclaimer

This tool is for educational and testing purposes only. Use it responsibly and only on systems you have permission to test.

