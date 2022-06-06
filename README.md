# NTU-ceiba-web-crawler

This repository is about a web crawler to download and upload from a system called <b>NTU Ceiba</b>.

<b>NTU Ceiba</b> is a course management system built by my alma mater National Taiwan University. I was a teaching assistant and it's been irritable to download hundreds of students' homework and upload grades once a time every week from this management system.

## Crawler System
There are two parts of this web crawler system
1. <b>NTU Ceiba Crawler-Download</b>: Download all homework files to our local path, and print those students' name whose homework is missing.
2. <b>NTU Ceiba Crawler-Upload</b>: After grading homework scores and save as a CSV file, then update those scores to the management system.

## Requirements & Tutorial
### Selenium
All systems are built under Python 3 using <b>Selenium Browser</b>. <b>Selenium</b> is an umbrella project for a range of tools and libraries that enable and support the automation of web browsers.

Visit [Selenium](https://www.selenium.dev/documentation/)

### WebDriver
Selenium Browser is to emulate user interaction with browsers, therefore it requires us to download WebDriver for nevigating to web pages, in this repository, we use [ChromeDriver](https://chromedriver.chromium.org/).

Simply download from the mainpage of <b>ChromeDriver</b> which suited to the version of Chrome you used.

```python
from selenium import webdriver

driver = webdriver.Chrome("ChromeDriver_path")
driver.get("website_link_to_crawl")
driver.quit()
```
