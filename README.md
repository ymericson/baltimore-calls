
### Baltimore City Police Emergency and Non-Emergency 911 Calls for Service, 2015-2018

### Summary
This notebook will analyze Baltimore's 911 police calls for service data to observe trends, and predict 911 calls using spatial analysis.

### Introduction

Baltimore, MD is known for its violent crime rate, including annual robbery and homicide rates that rank above the national average. Although overall reported crime has dropped significantly since the early 1990s, homicide rates remain high and especially concentrated in poverty areas. Despite the population of Baltimore metropolitan area having shrunk over decades, its per-capita homicide record remain one of the highest in the country.

Violent crime spiked in 2015 after the death of Freddie Gray on April 19, leading to a sudden spike in civil unrest and rioting from late April to early May. Crime rates in Baltimore reached one of the highest peaks that year; 2015's tally of 344 homicides, nearly 90 percent of which were the result of shooting, was the most since 1993.

### Data and Methods

Baltimore 911 call data was be obtained from [Open Baltimore](https://data.baltimorecity.gov/Public-Safety/911-Police-Calls-for-Service/xviu-ezkt). The calls dates range from January 1st, 2015 to present. There are 3.6 million rows as of July 1st, 2018, each row representing an individual call. Data is automatically refreshed multiple times a day.

The data contains the following fields:

* recordId: Int variable, record identifier
* callDateTime: Floating timestamp, YYYY-MM-DD HH:MM:SS
* priority: String variable, priority of call
* district: String variable, quadrant of Baltimore	
* description: String variable, description of the emergency call
* callNumber: String variable, call identifier
* incidentLocation: String variable, location of incident 	
* location: String variable, location of call

### Limitationa

**Reporting**: The 911 calls do not account for all crimes tha occured in Baltimore, since some are not reported. However, it is a big dataset and we are able to observe several trends over time.

**Categorization**: Calls that had descriptions 'no voice' or 'other' accounted for almost 30% of all calls. Some categories may overlap, such as 'common assault' and 'investigate' calls.

**Priority**: The standard for which calls are low or high priority were unclear, with a single category of calls having different levels of priority.
