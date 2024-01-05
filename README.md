# Mars HTML Scraping

The purpose of this project is to scrape and analyze data using Splinter and HTML parsing with Beautiful Soup. In part 1 of the project i'll be scraping titles and preview text from a Mars news article. In part 2 of the project i'll scrape and analyze Mars weather data.

# Summary

1. Scrape Titles and Preview Text from Mars News

    - Use automated browsing to visit the Mars news site. Inspect the page to identify which elements to scrape.

![Alt text](<Screen Shot 2024-01-04 at 5.58.14 PM.png>)

    - Create a Beautiful Soup object and use it to extract text elements from the website.

    - Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:

        - Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview. 

        - Store all the dictionaries in a Python list.

        - Print the list in your notebook.

![Alt text](<Screen Shot 2024-01-04 at 6.04.07 PM.png>)

2. Scrape and Analyze Mars Weather Data

    - Use automated browsing to visit the Mars Temperature Data Site. Inspect the page to identify which elements to scrape. Note that the URL is https://static.bc-edx.com/data/web/mars_facts/temperature.html.

![Alt text](<Screen Shot 2024-01-04 at 6.05.53 PM.png>)

    - Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas read_html function. However, use Beautiful Soup here to continue sharpening your web scraping skills.

    - Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:

        - id: the identification number of a single transmission from the Curiosity rover

        - terrestrial_date: the date on Earth
    
        - sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
    
        - ls: the solar longitude

        - month: the Martian month
    
        - min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
    
        - pressure: The atmospheric pressure at Curiosity's location

![Alt text](<Screen Shot 2024-01-04 at 6.13.10 PM.png>)
    
    - Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.

    - Analyze your dataset by using Pandas functions to answer the following questions:

        - How many months exist on Mars?
    
        - How many Martian (and not Earth) days worth of data exist in the scraped dataset?
    
        - What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
    
            - Find the average minimum daily temperature for all of the months.
        
            - Plot the results as a bar chart.
        
        - Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question: 
    
            - Find the average daily atmospheric pressure of all the months.
        
            - Plot the results as a bar chart.
    
        - About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
    
            - Consider how many days elapse on Earth in the time that Mars circles the Sun once.
        
            - Visually estimate the result by plotting the daily minimum temperature.

![Alt text](<Screen Shot 2024-01-04 at 6.15.11 PM.png>)
        
    - Export the DataFrame to a CSV file.

![Alt text](<Screen Shot 2024-01-04 at 6.16.00 PM.png>)
