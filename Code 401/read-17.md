# Web Scraping

Web scraping is a technique to automatically access and extract large amounts of information from a website, which can save a huge amount of time and effort. In this article, we will go through an easy example of how to automate downloading hundreds of files from the New York MTA. This is a great exercise for web scraping beginners who are looking to understand how to web scrape. Web scraping can be slightly intimidating, so this tutorial will break down the process of how to go about the process.

---
## Important notes about web scraping
- Read through the website’s Terms and Conditions to understand how you can legally use the data. Most sites prohibit you from using the data for commercial purposes.
- Make sure you are not downloading data at too rapid a rate because this may break the website. You may potentially be blocked from the site as well.

---
## Web Scraping best practices to follow to scrape without getting blocked
- Respect Robots.txt
- Make the crawling slower, do not slam the server, treat websites nicely
- Do not follow the same crawling pattern
- Make requests through Proxies and rotate them as needed
- Rotate User Agents and corresponding HTTP Request Headers between requests
- Use a headless browser like Puppeteer, Selenium or Playwright
- Beware of Honey Pot Traps
- Check if Website is Changing Layouts
- Avoid scraping data behind a login
- Use Captcha Solving Services

---
## Techniques
1. ***Human copy-and-paste*** The simplest form of web scraping is manually copying and pasting data from a web page into a text file or spreadsheet. Sometimes even the best web-scraping technology cannot replace a human’s manual examination and copy-and-paste, and sometimes this may be the only workable solution when the websites for scraping explicitly set up barriers to prevent machine automation.

2. ***Text pattern matching*** A simple yet powerful approach to extract information from web pages can be based on the UNIX grep command or regular expression-matching facilities of programming languages (for instance Perl or Python).

3. ***HTTP programmin*** Static and dynamic web pages can be retrieved by posting HTTP requests to the remote web server using socket programming.

4. ***HTML parsing*** Many websites have large collections of pages generated dynamically from an underlying structured source like a database. Data of the same category are typically encoded into similar pages by a common script or template. In data mining, a program that detects such templates in a particular information source, extracts its content and translates it into a relational form, is called a wrapper.

5. ***DOM parsing*** By embedding a full-fledged web browser, such as the Internet Explorer or the Mozilla browser control, programs can retrieve the dynamic content generated by client-side scripts. These browser controls also parse web pages into a DOM tree, based on which programs can retrieve parts of the pages. Languages such as Xpath can be used to parse the resulting DOM tree.

6. ***Vertical aggregation*** There are several companies that have developed vertical specific harvesting platforms. These platforms create and monitor a multitude of “bots” for specific verticals with no “man in the loop” (no direct human involvement), and no work related to a specific target site. The preparation involves establishing the knowledge base for the entire vertical and then the platform creates the bots automatically.

7. ***Semantic annotation recognizing*** The pages being scraped may embrace metadata or semantic markups and annotations, which can be used to locate specific data snippets.

8. ***Computer vision web-page analysis*** There are efforts using machine learning and computer vision that attempt to identify and extract information from web pages by interpreting pages visually as a human being might.
---

## How can websites detect and block web scraping ?
Websites can use different mechanisms to detect a scraper/spider from a normal user

Unusual traffic/high download rate especially from a single client/or IP address within a short time span.

Repetitive tasks performed on the website in the same browsing pattern – based on an assumption that a human user won’t perform the same repetitive tasks all the time.

Checking if you are real browser – A simple check is to try and execute JavaScript. Smarter tools can go a lot more and check your Graphic cards and CPUs to make sure you are coming from real browser.

Detection through honeypots – these honeypots are usually links which aren’t visible to a normal user but only to a spider. When a scraper/spider tries to access the link, the alarms are tripped.

![Web Scraping](https://www.promptcloud.com/wp-content/uploads/2020/05/Web-Scraping.jpeg)


---
#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>