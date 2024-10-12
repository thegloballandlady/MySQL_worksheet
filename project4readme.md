# MYSQL PROJECT_4
---

[QUESTION](#question)

[MY ANSWER](#my-answer)

[DATA SOURCE](#data-source) 

### QUESTION 
---
A Computer store is offering a 25% discount for all new customers over the age of 65 or customers that spend more than $200 on their first purchase.

The owner wants to know how many customers received that discount since they started the promotion.

Write a query to see how many customers received that discount.
customer_id	age	total_purchase
1001	72	1053
1002	86	826
1003	37	713
1004	61	923
1005	50	90
1006	45	1057
1007	39	673
1008	69	952
1009	29	874
1010	23	524
1011	81	496
1012	62	384
1013	80	1059
1014	99	1071
1015	75	1015



### MY ANSWER 
---
```SQL
SELECT COUNT (CUSTOMER_ID)
  FROM customers
  WHERE AGE >65
  OR TOTAL_PURCHASE > 200
  ;
```

### DATA SOURCE 
---
Analyst Builder
do check for [AlextheAnalyst](https://github.com/alextheanalyst) on Youtube 

#### highlight
This project requires the following filters
1. Filter on those older than 65 and with total purchase above 200
2. Do a count on customer id
