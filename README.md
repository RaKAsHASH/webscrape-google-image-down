# Google Image Scraper

## Overview
This Python script allows users to search and download images directly from Google Images by providing a search query and specifying the number of images to download. It uses the `requests` library to fetch the data and `BeautifulSoup` for HTML parsing.

## Features
- **Custom Search**: Specify the type of images to download.
- **Download Control**: Set the number of images to fetch and save.
- **Folder Management**: Automatically creates a folder to store the downloaded images.

## Requirements
- Python 3.x
- The following Python libraries:
  - `requests`
  - `bs4` (BeautifulSoup)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/RaKAsHASH/google-image-scraper.git
   cd google-image-scraper
2. Install the required libraries:
   ```bash
   pip install requests beautifulsoup4

## Usage
1. Run the script:
   ```bash
   python scraper.py
2. Enter the type of images you want to download (e.g., "cats" or "landscapes").
3. Specify the number of images to download.

## How It Works
1. The script sends a search request to Google Images with the user-specified query.
2. It parses the HTML response to extract image links using BeautifulSoup.
3. Downloads the specified number of images and saves them in the Images_1 folder.

## Code Explanation

### Main Components
- **User Agent Setup**: Mimics a browser to avoid being blocked by Google.
- **Image Download Logic**: Extracts image links from the HTML and downloads them using requests.
### Key Functions
`main()`: Initializes the folder and starts the download process. <br/>
`download_images()`: Handles the search query, fetches image links, and downloads them.

## Example
- **Input**:
  ```bash
  Enter images type you want to download: puppies
  Enter the number of images you want: 5
- **Output**:
  ```bash
  Found 5 images
  Start downloading...
  Download Completed!

## Notes

- **User Agent**: Update the User-Agent string if it becomes outdated or blocked.
- **Google Restrictions**: Google might block repeated or excessive requests. Use responsibly.
- **Image Quality**: The quality of downloaded images depends on Google's provided links.




