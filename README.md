# Mission-to-Mars

## Background
Robin is now ready to take on the full web-scraping and data analysis project for the mission to Mars. She’s learned to identify HTML elements on a page, identify their `id` and `class` attributes, and use this knowledge to extract information via both automated browsing with Splinter and HTML parsing with Beautiful Soup. She’s also learned to scrape various types of information. These include HTML tables and recurring elements, like multiple news articles on a webpage.

I’ll help Robin scrape, organize, analyze, and visualize the data. As I work on this Challenge, remember that I am trengthening the same core skills that I have been developing until now: collecting data, organizing and storing data, analyzing data, and then visually communicating my insights.
Web-scraping and data analysis project for the mission to Mars

## Deliverable 1: Scrape Titles and Preview Text from Mars News

Open the Jupyter Notebook in the starter code folder named `part_1_mars_news.ipynb`. You will work in this code as you follow the steps below to scrape the Mars News website.

1. Use automated browsing to visit the Mars NASA news site Links to an external site.. Inspect the page to identify which elements to scrape.

**Below is a part of the code in Jupyter and the Websraping News and Images:**

![image](https://user-images.githubusercontent.com/112348240/208799200-2910cbb6-1c31-425e-9216-6d8aa6072b07.png)

2. Create a Beautiful Soup object and use it to extract text elements from the website.

3. Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:

  - Store each `title`-and-`preview` pair in a Python dictionary. And, give each dictionary two keys: title and preview. **An example is the following:**
  
![image](https://user-images.githubusercontent.com/112348240/208800459-38ae1d87-65c9-4cf5-b8cc-6cb50d2117ee.png)

  - Store all the dictionaries in a Python list.
  - Print the list in your notebook.
  
## Deliverable 2: Scrape and Analyze Mars Weather Data
Open the Jupyter Notebook in the starter code folder named `part_2_mars_weather.ipynb.` You will work in this code as you follow the steps below to scrape and analyze Mars weather data.

1. Use automated browsing to visit the Mars Temperature Data Site Links to an external site.. Inspect the page to identify which elements to scrape. Note that the URL is `https://data-class-mars-challenge.s3.amazonaws.com/Mars/index.html`.
2. Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas `read_html` function. However, use Beautiful Soup here to continue sharpening your web scraping skills.

3. Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:

    - `id`: the identification number of a single transmission from the Curiosity rover
    - `terrestrial_date`: the date on Earth
    - `sol`: the number of elapsed sols (Martian days) since Curiosity landed on Mars
    - `ls`: the solar longitude
    - `month`: the Martian month
    - `min_temp`: the minimum temperature, in Celsius, of a single Martian day (sol)
    - `pressure`: The atmospheric pressure at Curiosity's location
    
    **Screenshot of the table**
    
    ![image](https://user-images.githubusercontent.com/112348240/208804417-73e7a353-658f-445c-a8e9-d6667c96c41a.png)

4. Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate `datetime`, `int`, or `float` data types.

![image](https://user-images.githubusercontent.com/112348240/208804527-b0ecc42d-4b89-4b97-a082-bb0a24b3fa6e.png)

5. Analyze your dataset by using Pandas functions to answer the following questions:

      1. How many months exist on Mars?

      ![image](https://user-images.githubusercontent.com/112348240/208804707-7e656b7a-bdb5-4032-aa1c-48ed432eebf1.png)

      2. How many Martian (and not Earth) days worth of data exist in the scraped dataset?
      
      ![image](https://user-images.githubusercontent.com/112348240/208804792-7bf48d72-c639-4197-8ed2-f3b9236a16e4.png)

      3. What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
          - Find the average the minimum daily temperature for all of the months.
          - Plot the results as a bar chart.
       ![image](https://user-images.githubusercontent.com/112348240/208804915-ac607696-6787-43dd-8e5f-09d2cca498ae.png)

      4. Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
          - Find the average the daily atmospheric pressure of all the months.
          - Plot the results as a bar chart.    
![image](https://user-images.githubusercontent.com/112348240/208805158-ec4b5297-7f62-4ca7-8a53-65e0f776f424.png)
      5. About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
          - Consider how many days elapse on Earth in the time that Mars circles the Sun once.
          - Visually estimate the result by plotting the daily minimum temperature.
![image](https://user-images.githubusercontent.com/112348240/208805334-6ef50e58-5c5b-488b-b1f6-9a2c65a5337e.png)

6. Export the DataFrame to a CSV file.







**The Screnshoot below shows the data Stored at MondoDB**
![Stored at MongoDB Screenshot](https://user-images.githubusercontent.com/112348240/208797202-a3262c38-2bd7-4949-9117-486b50dfbd76.png)
