# Scraping Central Weather Bureau data with Python
  Knowing that I was learning web scraping with Python, one of my friends asked me to scrape weather data from Central Weather Bureau for him. 

  As a web scraping rookie, I didn’t know it was a dynamic website and used BeautifulSoup. What I could get was merely framework of the website. I tried to find a solution on Stack Overflow and came across Selenium, which was initially used for automating the tests carried out on web browsers. 
  
I installed Selenium, downloaded ChromeDriver, and gave it a try. This time I successfully scraped temperature data but couldn’t crawl humidity and precipitation data. After inspecting the source code, I realized I had to click on the humidity button and precipitation button to load the data. While I was testing my code, the error:    Element is not clickable at point (x, y). Other element would receive the click     will occur every now and then, so I tried JavaScriptExecutor and the problem was solved.

  I used pandas to turn the weather data into a csv file (data → dictionary → data frame → csv). Lastly, I added a date and time row to the csv file and proudly showed the result to my friend.
