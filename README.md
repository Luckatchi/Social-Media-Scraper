# Web-Scraper
This script automates the process of searching for social media profiles on Instagram and Facebook based on specific keywords and location. It uses web scraping tools to fetch search results from Google, processes the results to extract valid social media profile links, and saves the links in Excel files for further analysis.

Main Features:
Automated Search Query Generation:

Dynamically generates Google search queries based on given keywords and a specific location.
Supports both Instagram and Facebook search filters.
Web Scraping:

Uses Selenium for browser automation and BeautifulSoup to parse search result pages.
Rotates User-Agent strings to minimize detection.
Handling reCAPTCHA:

Detects reCAPTCHA challenges and alerts the user with a sound notification.
Waits and retries the scraping process if a CAPTCHA is detected.
Excel File Output:

Extracted links are saved in separate Excel files for Instagram and Facebook.
Links are color-coded: Green for Instagram and Yellow for Facebook.
Randomized Delays:

Introduces random delays between requests to simulate human behavior and reduce the risk of being blocked by search engines.
Requirements to Run the Script
1. Software Requirements
Python 3.7 or higher.
A browser driver compatible with Chrome (e.g., ChromeDriver).
2. Python Libraries
The following libraries are required:

Selenium: For web automation.
Install via pip install selenium
BeautifulSoup (bs4): For parsing HTML content.
Install via pip install beautifulsoup4
openpyxl: For working with Excel files.
Install via pip install openpyxl
pygame: For sound playback during reCAPTCHA detection.
Install via pip install pygame
3. Additional Files
chromedriver.exe: The ChromeDriver executable that matches your browser version.

Place it in an accessible directory and update its path in the script (C:/Users/hassa/Desktop/python/chromedriver.exe).
alert.mp3: An audio file that plays when reCAPTCHA is detected.

4. Internet Connection
A stable internet connection is needed since the script accesses Google Search, Instagram, and Facebook.

Steps to Run the Script
Install Dependencies: Ensure all the required Python libraries are installed using the commands above.

Configure ChromeDriver:

Download ChromeDriver from https://chromedriver.chromium.org/ and place it in the specified directory.
Verify that the ChromeDriver version matches your installed version of Google Chrome.
Place the alert.mp3 File:

Place an audio file named alert.mp3 in the same directory as the script.
Run the Script: Execute the script in a terminal or IDE:

bash
Copier le code
python script_name.py
Enter Keywords and Location: Modify the keywords and location variables in the script to specify the profiles you're searching for.

Output:

Two Excel files will be generated:
instagram_links.xlsx: Contains all Instagram profile links found.
facebook_links.xlsx: Contains all Facebook profile links found.
Links will be color-coded for easier identification.
Disclaimer
This script is for educational purposes and must comply with the terms of service of the websites being accessed (Google, Instagram, Facebook). Misuse of this script for unauthorized scraping may result in IP bans or legal consequences.
