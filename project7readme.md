# MYSQL PROJECT_7
---

[QUESTION](#question)

[MY ANSWER](#my-answer)

[DATA SOURCE](#data-source) 

### QUESTION 
---
Data was input incorrectly into the database. The ID was combined with the First Name.

Write a query to separate the ID and First Name into two separate columns.

id
12345Johnny
93829Sally
20391Larry
29324Valerie



### MY ANSWER 
---
```SQL
SELECT
  substring (id,1,5) as id_fixed,
 substring(id,6) as first_name
  FROM bad_data 
  ;
```

### DATA SOURCE 
---
Analyst Builder
do check for [AlextheAnalyst](https://github.com/alextheanalyst) on Youtube 

#### highlight
This project requires the following filters:

1.filter to get id knowing they are 5 character long


