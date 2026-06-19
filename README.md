# Phishing Website Detection Chrome Extension

## Overview

Phishing Website Detection is a Chrome Extension developed to identify potentially malicious websites and alert users before they interact with suspicious pages.

The extension combines blacklist-based detection and rule-based URL analysis to detect phishing attempts in real time.

## Features

* Detects phishing websites using a blacklist of known malicious domains.
* Analyzes URLs using heuristic rules.
* Warns users when suspicious websites are detected.
* Automatically scans every website loaded in the browser.
* Lightweight and easy to use.

## Detection Techniques

### 1. Blacklist-Based Detection

The extension checks whether the current website domain exists in a blacklist of known phishing domains.

### 2. Rule-Based Detection

The extension evaluates URLs using the following indicators:

* Excessively long URLs
* Presence of '@' symbols
* Suspicious keywords such as:

  * login
  * verify
  * update
  * bank
  * secure
* Usage of HTTP instead of HTTPS

When multiple suspicious indicators are detected, the extension displays a warning message to the user.

## Technologies Used

* JavaScript
* HTML
* CSS
* Chrome Extension API
* Python

## Project Structure

phishing-website-detection/

├── manifest.json

├── background.js

├── content.js

├── popup.html

├── style.css

├── blacklist.json

├── online-valid.csv

└── extract.py

## How It Works

1. User opens a website.
2. The content script sends the current URL to the background service worker.
3. The extension checks whether the domain exists in the blacklist.
4. If not blacklisted, rule-based analysis is performed.
5. If suspicious patterns are found, a warning message is displayed.

## Installation

1. Download or clone this repository.
2. Open Google Chrome.
3. Navigate to:

chrome://extensions

4. Enable Developer Mode.
5. Click "Load unpacked".
6. Select the project folder.
7. Start browsing.

## Future Improvements

* Machine Learning based phishing detection
* Website reputation checking APIs
* Visual phishing page analysis
* Better popup dashboard
* Risk scoring system
* Detailed threat reports

## Author

Sahithya
