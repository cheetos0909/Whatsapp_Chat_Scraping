# WhatsApp Chat Scraping using Pushbullet API

This script allows you to scrape and extract chat data from WhatsApp using the Pushbullet API. It fetches the chat data and saves it in an Excel file for further analysis.

## Prerequisites

Before you can use this script, you need to have the following:

- Python installed on your system.
- The required Python libraries installed. You can install them using the following command:

    ```bash
    pip install pushbullet.py
    ```

- A Pushbullet API key. You can obtain your API key from the Pushbullet website.

## Usage

1. Clone this repository or download the script `whatsapp_chat_scraper.py`.

2. Create a file named `config.py` in the same directory as the script and add your Pushbullet API key as follows:

    ```python
    API_KEY = "YOUR_PUSHBULLET_API_KEY"
    ```

3. Run the script:

    ```bash
    python whatsapp_chat_scraper.py
    ```

4. The script will fetch your WhatsApp chat data using the Pushbullet API and save it as an Excel file named `chat_with_friend.xlsx`.

## Cleaning Data

The script also cleans the raw chat data, extracting the date, time, sender's name, and message. The cleaned data is stored in the Excel file.

## File Structure

- `whatsapp_chat_scraper.py`: The main Python script for scraping WhatsApp chat data.
- `config.py`: Configuration file for storing your Pushbullet API key.
- `chat_with_friend.xlsx`: The output Excel file containing the cleaned chat data.

## Example Output

Here is an example of the cleaned chat data in the Excel file:

|    Date    |   Time  |    Name   |         Message          |
|------------|---------|-----------|--------------------------|
| 2023-10-01 | 15:30:00| Friend    | Hello, how are you?      |
| 2023-10-01 | 15:35:00| You       | I'm good, thanks!        |
| 2023-10-01 | 15:40:00| Friend    | What have you been up to?|
| ...        |   ...   |   ...     | ...                      |


## Acknowledgments

- Thanks to Pushbullet for providing the API to access chat data.
- Inspired by the need to analyze WhatsApp chat history easily.

Feel free to contribute and improve this script. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request.
