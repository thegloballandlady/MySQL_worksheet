# MYSQL PROJECT_6
---

[QUESTION](#question)

[MY ANSWER](#my-answer)

[DATA SOURCE](#data-source) 

### QUESTION 
---
Often when you're working with customer information you'll want to sell that data to a third party. Sometimes it is illegal to give away sensitive information such as a full name.

Here you are given a table that contains a customer ID and their full name.

Return the customer ID with only the first name of each customer.


customer_id	full_name
1001	John McGary
1002	Sally Sue
1003	Jenny McBlue
1004	Craig Johnson
1005	Henry Hue
1006	Alex Freebird


### MY ANSWER 
---
```SQL
SELECT CUSTOMER_ID,
   SUBSTRING_INDEX (FULL_NAME, " ", 1) AS FIRST_NAME
  FROM customers
  ;
```

### DATA SOURCE 
---
Analyst Builder
do check for [AlextheAnalyst](https://github.com/alextheanalyst) on Youtube 

#### highlight
This project requires the following filters:

1.Sunstring index

2.We are return thecustomer id with just the first name


