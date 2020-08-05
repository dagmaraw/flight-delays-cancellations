# flight-delays-cancellations

# US Flight Delay and Cancellation Trends in 2019
## by Dagmara Namasivayam


## Dataset

The data consists of 7,434,871 (after cleaning) US flights in 2019 (all months). Many flight details, including delays/cancellations including cause, origin/destination, airline, and times are included. I removed some columns that I knew I wouldn't use, such as flight number.


## Summary of Findings

I was interested in finding trends relating to flight delays and cancellations. I started with many univariate explorations. I found that delays had a unimodal distribution with the peak actually 10 minutes *early*, but with a long tail to the higher delay values. I put the delay values into bins, including cancellations, which was 2% of all flights.

I found that winter was the busiest flight season. I also found the airlines and airports that had the most flights that year. Looking at hour of flight departure, the 6 o'clock hour was the most popular time for flights. The remainder of the flights waved, with other peaks at noon and 5pm. Most flight were between 5am and 11pm. Majority of flights cancellations were due to weather. Delay was roughly even between days of the week and seasons, but increased as scheduled departure time increased from 5am to 7pm. At that hour, the trend reversed, but went down again after midnight. Cancellations showed a similar trend with departure hour.

I found that ATL airport had the highest percentage of on-time flights, and the lowest percentage of cancellations out of the top 6 airports explored. The cancellations due to weather had a clear majority in the winter season. The other seasons had closer margins, but only spring did not have weather as the leading cause of cancellations. Looking at this trend for 6 of the highest-trafficked airports, we find that LAX is the only airport for which weather was not the leading cancellation cause for any season. Besides that, carrier cancellations surpassed weather as the top cause only at ATL in spring and fall, and at CLT in the fall. Adding departure time to that analysis, I found that NAS cancellations were responsible for more cancellations of flights that departed in the afternoon than the morning.


## Key Insights for Presentation

I found that of the 2% total flights cancelled in 2019, the majority were due to weather. In fact, weather  was the leading cause of flight cancellations for all seasons except Spring. Weather caused by far the majority of cancellations in winter (December, January, February). If we look at this trend for 6 of the highest-trafficked airports, we find that LAX is the only airport for which weather was not the leading cancellation cause for any season. Besides that, carrier cancellations surpassed weather as the top cause only at ATL in spring and fall, and at CLT in the fall. It was surprising to learn that location of destination of airport (cold vs. temperate climate) is not a very good predictor of weather-related cancellations.