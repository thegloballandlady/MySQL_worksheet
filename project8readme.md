# MYSQL PROJECT_8
---

[QUESTION](#question)

[MY ANSWER](#my-answer)

[DATA SOURCE](#data-source) 

### QUESTION 
---
Social Media Addiction can be a crippling disease affecting millions every year.

We need to identify people who may fall into that category.

Write a query to find the people who spent a higher than average amount of time on social media.

Provide just their first names alphabetically so we can reach out to them individually.

user_id	media_time_minutes (dataset 1)
1	0
2	200
3	250
4	15
5	500
6	45
7	450
8	1000
9	300
10	60

user_id	first_name (dataset 2)
1	John
2	Janice
3	Michael
4	Molly
5	Adam
6	Amanda
7	Chris
8	Christine
9	Bella
10	Brian



### MY ANSWER 
---
```SQL
SELECT first_name
  from users 
  where user_id IN (SELECT user_id
        FROM user_time
        WHERE MEDIA_TIME_MINUTES > (SELECT AVG(MEDIA_TIME_MINUTES) 
                            FROM user_time))
  ORDER BY FIRST_NAME 
;
```

### DATA SOURCE 
---
Analyst Builder
do check for [AlextheAnalyst](https://github.com/alextheanalyst) on Youtube 


#### highlight
---
This project requires the following filters:

1. Calculate the avg media time

2. Create subqueries

3. Count by firstname in ascending order

