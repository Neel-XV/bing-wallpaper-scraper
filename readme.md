# Bing Wallpaper Scraper 🖼️

## Overview

A powerful Python script that automates the process of downloading daily Bing wallpapers from the Bing Wallpaper Archive. This tool allows you to efficiently curate a personalized collection of high-quality wallpapers with minimal effort.

## 🌟 Features

- **Efficient Web Scraping**: Uses Selenium WebDriver to extract wallpaper URLs and metadata
- **Parallel Downloading**: Supports concurrent image downloads for faster collection
- **Robust Error Handling**: Implements retry mechanisms and comprehensive logging
- **Flexible Customization**: Easily configure download parameters via command-line arguments
- **Organized Storage**: Automatically creates month-based subdirectories for downloaded images

## 🛠️ Prerequisites

- Python 3.7+
- Firefox Browser
- pip (Python package manager)

## 📦 Dependencies

The script requires the following Python libraries:

- selenium
- webdriver_manager
- requests
- urllib3

## 🚀 Installation

1. Clone the repository:

  ```bash
  git clone https://github.com/Neel-XV/bing-wallpaper-scraper.git
  cd bing-wallpaper-scraper
  ```

2. Install required dependencies:

  ```bash
  pip install -r requirements.txt
  ```

## 💻 Usage

### Basic Usage

```bash
python bing_wallpaper_scraper.py
```

This will download wallpapers for the current month (October 2024 by default)

### Advanced Usage

```bash
# Specify a different month
python bing_wallpaper_scraper.py -m 202412

# Customize number of concurrent workers
python bing_wallpaper_scraper.py -w 5
```

### Command-Line Arguments

- `-m` or `--month`: Specify month to scrape (format: YYYYMM, default: 202410)
- `-w` or `--workers`: Number of concurrent download workers (default: 10)

## 📂 Output Structure

Downloaded wallpapers are organized as follows:

```
images/
└── 202410/
    ├── wallpaper1.jpg
    ├── wallpaper2.jpg
    └── ...
```

## ⚠️ Troubleshooting

- Ensure Firefox is installed
- Check internet connectivity
- Verify WebDriver compatibility

## 🤝 Contributing

Contributions are welcome! Please:

- Fork the repository
- Create a feature branch
- Submit a pull request

## 📄 License

[MIT License](./LICENSE)

**Happy Wallpaper Collecting!** 🖼️✨
