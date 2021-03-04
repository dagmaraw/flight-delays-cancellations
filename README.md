### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>

There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python.  The code should run with no issues using Python versions 3.*.

## Project Motivation<a name="motivation"></a>

The goal of this project was to practice creating data visualizations. To that end, exploratory visualizations were created to help pose questions. A segment of these visualizations were chosen and polished into explanatory visualizations, which are presented in a slideshow.

The dataset in this project includes almost 7.5 million domestic flights throughout 2019. It includes flights details such as time of departure/arrival, origin/destination airports, carriers, and delay times/cancellations. This project includes analysis of arrival delays and cancellations, but the investigation focuses on characteristics of only cancelled flights. 

I look at the following:

1. Distribution of arrival delay times and a categorical distribution of delays and cancellations
2. Distribution of cancellation causes
3. Cancellation cause vs. season
4. Cancellation cause vs. season by airport

## File Descriptions <a name="files"></a>

There are two Jupyter notebooks in the respository. exploration_flights.ipynb is exploratory in creating visualizations to pose and answer the questions above. slide_deck_flights.ipynb is used to create the slide deck presentation including the final visualizations. 

The data is found in the /data folder. It consists of 7,434,871 (after cleaning) US flights in 2019 (all months). Many flight details, including delays/cancellations including cause, origin/destination, airline, and times are included. I removed some columns that I knew I wouldn't use, such as flight number.

The published slideshow is slide_deck_flights.slides.html. output_toggle.tpl is a template file used with nbconvert to export the slide deck. All the data required to run the exploratory notebook in in the data folder, and includes one .csv file for each month of flights in 2019. This data was downloaded from [here](https://www.transtats.bts.gov/DL_SelectFields.asp?Table_ID=236).

Note: The slides (slide_deck_flights.slides.html) are not viewable through GitHub. The easiest way to view html files is to download the repo (click green link labeled "code" on [main repo page](https://github.com/dagmaraw/flight-delays-cancellations) and choose "Download ZIP"). The file can then be opened from the download.

## Results<a name="results"></a>

The main findings can be viewed by opening slide_deck_flights.slides.html.

I was interested in finding trends relating to flight delays and cancellations. I started with many univariate explorations. I found that delays had a unimodal distribution with the peak actually 10 minutes *early*, but with a long tail to the higher delay values. I put the delay values into bins, including cancellations, which was 2% of all flights.

I found that winter was the busiest flight season. I also found the airlines and airports that had the most flights that year. Looking at hour of flight departure, the 6 o'clock hour was the most popular time for flights. The remainder of the flights waved, with other peaks at noon and 5pm. Most flight were between 5am and 11pm. Majority of flights cancellations were due to weather. Delay was roughly even between days of the week and seasons, but increased as scheduled departure time increased from 5am to 7pm. At that hour, the trend reversed, but went down again after midnight. Cancellations showed a similar trend with departure hour.

I found that ATL airport had the highest percentage of on-time flights, and the lowest percentage of cancellations out of the top 6 airports explored. The cancellations due to weather had a clear majority in the winter season. The other seasons had closer margins, but only spring did not have weather as the leading cause of cancellations. Looking at this trend for 6 of the highest-trafficked airports, we find that LAX is the only airport for which weather was not the leading cancellation cause for any season. Besides that, carrier cancellations surpassed weather as the top cause only at ATL in spring and fall, and at CLT in the fall. Adding departure time to that analysis, I found that NAS cancellations were responsible for more cancellations of flights that departed in the afternoon than the morning.

I found that of the 2% total flights cancelled in 2019, the majority were due to weather. In fact, weather  was the leading cause of flight cancellations for all seasons except Spring. Weather caused by far the majority of cancellations in winter (December, January, February). If we look at this trend for 6 of the highest-trafficked airports, we find that LAX is the only airport for which weather was not the leading cancellation cause for any season. Besides that, carrier cancellations surpassed weather as the top cause only at ATL in spring and fall, and at CLT in the fall. It was surprising to learn that location of destination of airport (cold vs. temperate climate) is not a very good predictor of weather-related cancellations.

## Licensing, Authors, Acknowledgements<a name="licensing"></a>

This project was done as part of Udacity's Data Analyst Nanodegree program. Credit to Bureau of Transportation Statistics for the data. output_toggle.tpl was take from [this page](https://github.com/damianavila/blog/blob/master/posts/hide-the-input-cells-from-your-ipython-slides.ipynb).
