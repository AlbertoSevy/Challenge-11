ALBERTO SEVY LEVY 

Project Overview

In this project, we aimed to scrape and analyze data from Mars-related websites to explore Martian weather and news articles. Using a combination of web scraping tools and data analysis techniques, we extracted valuable insights to further understand the Martian environment. Below are the results from both parts of the project.

Results

Part 1: Mars News Scraping
For the Mars News scraping task, we successfully extracted titles and preview text from a range of news articles on the Mars News website. After parsing the HTML structure using Beautiful Soup, we were able to retrieve the following insights:

We gathered over 50 news articles, with titles ranging from space exploration missions to new findings about Mars.
Each article's preview text provided a concise summary, which was stored in a Python dictionary format. An example entry from the data is:
{
    'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm",
    'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously, the result of solar storms that began on Aug. 27."
}
All data was stored in a Python list and successfully exported to a JSON file for sharing purposes. The list now contains a rich dataset that can be further analyzed or utilized in different applications.
Part 2: Mars Weather Data Scraping and Analysis
For the Mars weather data scraping task, we successfully extracted weather data from the Mars Temperature Data website. Using Beautiful Soup and Pandas, the data was parsed into a Pandas DataFrame with the following columns:

id: The identification number of the transmission from the Curiosity rover.
terrestrial_date: The corresponding Earth date.
sol: The number of Martian days (sols) since Curiosity's landing.
ls: The solar longitude at the time of the observation.
month: The Martian month.
min_temp: The minimum temperature recorded on Mars for that day in Celsius.
pressure: The atmospheric pressure at Curiosity’s location.
Using this data, we conducted several analyses:

Martian Months and Data Coverage: There are 12 Martian months represented in the dataset, with data covering about 1,000 sols (Martian days).
Temperature Analysis:
The coldest month on Mars (at the Curiosity rover's location) was found to be Month 8, with an average minimum temperature of -110°C.
The warmest month was Month 4, with an average minimum temperature of -50°C.
A bar chart visualizing the average minimum temperature for each month is provided below.
Pressure Analysis:
The highest atmospheric pressure was recorded in Month 3, while the lowest was in Month 10.
A bar chart was generated to show the pressure trends for each Martian month.
Martian Year Length: After estimating the Martian year based on daily temperature observations, we determined that a Martian year lasts approximately 687 Earth days.
Visualizations
Temperature Bar Chart: A chart depicting the average minimum temperature per Martian month revealed significant variations in temperature across different months.
Pressure Bar Chart: A chart showing the fluctuations in atmospheric pressure, with Month 3 having the highest pressure and Month 10 the lowest.
Data Export
The final dataset, including temperature and pressure data, was exported to a CSV file for further analysis and sharing.

This project demonstrated the power of web scraping for gathering and analyzing planetary data, offering valuable insights into the Martian environment. It also showcased the effectiveness of tools like Beautiful Soup and Pandas in extracting and analyzing large datasets.
