# Journalism 2050 - Instagram Scraper

A Python-based Instagram profile scraper using Instaloader to collect follower statistics and profile information.

## Features

- Scrape Instagram profile data including followers, following, posts count
- Rate limiting to avoid API restrictions
- Caching system to avoid re-fetching already collected data
- Export data to CSV and JSON formats

## Requirements

- Python 3.x
- pandas
- instaloader

## Installation

```bash
pip install pandas instaloader
```

## Usage

1. Prepare a `data.csv` file with a `social.instagram` column containing Instagram usernames
2. Run the notebook `scrapingInsta.ipynb`
3. Data will be cached in `instagram_cache.csv`

## Files

- `scrapingInsta.ipynb` - Main scraping notebook
- `data.csv` - Input data with Instagram usernames
- `instagram_cache.csv` - Cached Instagram profile data
- `TwitterScraper/` - Twitter scraping utilities

## Notes

- The script includes automatic rate limiting (8-second delays) to avoid Instagram's API restrictions
- Cached data is reused to minimize API calls
- If you encounter 401 errors, increase the delay or wait before retrying
