---
title: "Machine Learning during Covid-19"
datePublished: Fri Jun 28 2024 14:40:26 GMT+0000 (Coordinated Universal Time)
cuid: clxysvt6t000209kz84wdejgh
slug: machine-learning-during-covid-19
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1719585954995/53f047ba-8cc0-41c9-8c16-0c4ab42a85ff.jpeg
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1719585440980/c315bf21-e56d-4725-8ad2-796bd73d6556.jpeg
tags: ai, data-science, machine-learning, covid-19

---

**Note**: I published this article on LinkedIn 4 years ago.

In the time of COVID-19, almost all aspects of our lives are affected, some being slightly resilient and others being heavily hit. Even the weather forecast are going to be affected by corona while weather is not. The reason for that is the dependencies of the weather forecasting models on the [data collected by aircraft](https://www.accuweather.com/en/severe-weather/coronavirus-canceled-flights-could-affect-weather-forecasting-at-exactly-the-wrong-time/711234) e.g., Wind speed, Wind direction, Air pressure, Air temperature together with Temporal and Spatial information. As per [ECMWF](https://www.ecmwf.int/), The data collected by aircraft is [second only to satellite data](https://www.ecmwf.int/en/about/media-centre/news/2020/drop-aircraft-observations-could-have-impact-weather-forecasts) in terms of their significance for weather predictions. Now due to the very heavy reduction in air traffic the weather forecast accuracy will be slightly impacted but the impact will still be [statistically significant](https://www.aljazeera.com/news/2020/03/weather-predictions-affected-coronavirus-outbreak-200326104501955.html).

A lot of work is already happening to cope with COVID-19 pandemic. I see a lot of articles on the internet about how Machine Learning or AI could be used to combat Corona Virus e.g., Forecasting models to predict the outbreak, Computer Vision models to better screen the existence of Corona infection in the X-ray/CT-scan images.

However, I do not see much contribution in the direction of modeling the impact of corona virus on businesses. This is obvious that majority of the businesses are affected by the pandemic but the question is how can we forecast the demand or sales given the corona pandemic in a particular region. The answer to this question becomes even more interesting for the companies who are currently using ML models for the forecasting of their business. How could the models running in production incorporate the COVID-19 related data to model the impact on business and adjust the forecasts accordingly? Here at Continental, we are running a number of forecasting models to predict a number of things e.g., Demand, Revenue, Sales, Raw material requirements.

I could think of couple of strategies which I am planning to test if they help to adapt the behavior of our forecasting models:

A very naive approach could be just to add a binary feature which could emphasize on the time-period when an outlier event e.g., COVID-19 took place which of course could be different for different regions. Perhaps a step a forward approach could be to also add the actual effect of this event (COVID-19) hence the model not only learns when the event happened but also how the event evolved within that period e.g., daily new cases, daily recovered cases, daily deaths due to COVID-19. This also depends upon the aggregation level (forecast step size) of the data. I could also think of adding a data set e.g., employment data, stock data which could exhibit the impact of COVID-19, and we use this effect from aforementioned data sets as a feature to learn the behavior. Of course, the semantics of such a data set should be close to the business we are forecasting. I wrote this post to start a discussion around this topic to brainstorm on the ideas we can use to combat with the adverse effect on our respective businesses. We can already see the impact of COVID-19 on the employment e.g., In the US alone, [16 million jobs are already gone](https://www.theguardian.com/business/2020/apr/09/us-unemployment-filings-coronavirus) while more than 6.6 million alone in the week of 9th April, 2020. I hope that companies will quickly develop resilience to the impact and leave minimal impact on employment. In the meantime, we continue to contribute!

Looking forward to your ideas/comments on modeling the impact of COVID-19 in our ML models.