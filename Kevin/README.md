# Michigan's Economy During the COVID-19 Pandemic

## Overview

This project tasked us with determining a situation in which we could use pandas and the Python programming language to present a real world situation with real world data. We decided to analyze the COVID-19 pandemic and its affect that it has had upon the Michigan Economy. Throughout this project, we used many different sources of information, both through API's and data downloaded to my computer.

## Data
The local data is data downloaded from the Department of Labor and Opportunity Insights Economic Tracker. The Opportunity Insights Economic Tracker data is located at tracktherecovery.org and references paper at this link https://opportunityinsights.org/wp-content/uploads/2020/05/tracker_paper.pdf.

We are currently using 3 different API's in this project; Bureau of Labor Statistics' Public API, COVID Tracking's API, and Googles Geocoding API.

## Presentation 
Google Slides presentation for this project can be found at: https://docs.google.com/presentation/d/1iVt6A2sdKbQmUp9yFeN-CnL-Qe2O55kU8VOoKw5pdn4/edit?usp=sharing. 

Presentation contains analysis of the data we gathered and all of the relevant charts and figures representing our work. 





# Notes

    - The BLS API that we used was somewhat confusing to use.
    - Needed to pre-generate series ID numbers through the BLS website and then request the API for that specific series or multiple series.
    - You also needed to define the content type in a headers parameter when sending request.get() and send data parameter as a json.dump()
    - We had to create a common 'datetime' column across two tables as a way to merge daily data. 
        - This resulted in some funky datetime.date() stuff and some string splicing.