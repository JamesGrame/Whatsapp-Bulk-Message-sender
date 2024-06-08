# WhatsApp Bulk Message Sender

This project allows you to send bulk WhatsApp messages using a list of contacts and product links stored in an Excel file. The script reads the Excel file, extracts the phone numbers and product links, and sends the messages automatically using the `pywhatkit` library.

## Prerequisites

Before you can run the script, you need to have the following:

1. Python 3.x installed on your machine.
2. The required Python libraries installed:
    - pandas
    - pywhatkit
    - openpyxl (for reading Excel files)

## Installation

1. Clone the repository:

2. Navigate to the project directory:

3. Install the required Python libraries:
    ```sh
    pip install pandas pywhatkit openpyxl
    ```

## Usage

1. Prepare your Excel file (`data.xlsx`) with the following columns:
    - `WhatsApp Number(with country code)`: The recipient's phone number, including the country code (e.g., +1234567890).
    - `Product link`: The message or product link to be sent.

2. Place the `data.xlsx` in the project directory.

3. Run the script:
    ```sh
    python main.py
    ```

## Note

- Ensure that you have a stable internet connection while running the script.
- WhatsApp Web needs to be logged in on your default browser for `pywhatkit` to work.
- The script waits for 3 seconds before sending the next message to avoid any potential issues with WhatsApp's message sending limits.
