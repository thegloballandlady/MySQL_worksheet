# MYSQL PROJECT_4
---

[QUESTION](#question)

[MY ANSWER](#my-answer)

[DATA SOURCE](#data-source) 

### QUESTION 
---
After about 10,000 miles, Electric bike batteries begin to degrade and need to be replaced.

Write a query to determine the amount of bikes that currently need to be replaced.


bike_id	miles
120320	15842
120321	15027
120322	6657
120323	22431
120324	14427
120325	6868
120326	9341
120327	17345
120328	14668
120329	11322
120330	22363
120331	4939
120332	915
120333	6380




### MY ANSWER 
---
```SQL
SELECT COUNT (BIKE_ID)
  FROM bikes
  WHERE MILES >10000
  ;
```

### DATA SOURCE 
---
Analyst Builder
do check for [AlextheAnalyst](https://github.com/alextheanalyst) on Youtube 

#### highlight
This project requires the following filters
1. Filter down on miles >10,000
2.  Count on bike_id


