# MYSQL PROJECT_9
---

[QUESTION](#question)

[MY ANSWER](#my-answer)

[DATA SOURCE](#data-source) 

### QUESTION 
---
If our company hits its yearly targets, every employee receives a salary increase depending on what level you are in the company.

Give each Employee who is a level 1 a 10% increase, level 2 a 15% increase, and level 3 a 200% increase.

Include this new column in your output as "new_salary" along with your other columns.

employee_id	pay_level	salary
1001	1	75000
1002	1	85000
1003	1	60000
1004	2	95000
1005	2	95000
1006	2	85000
1007	2	105000
1008	3	300000
1009	2	105000
1010	2	95000
1011	2	115000
1012	1	85000
1013	1	75000
1014	1	60000
1015	1	75000
1016	2	85000
1017	2	105000
1018	2	95000
1019	1	75000


### MY ANSWER 
---
```SQL
SELECT employee_id,
  pay_level,
  salary,
  case
  when pay_level = 1 then salary + salary*0.10
  when pay_level =2 then salary + salary*0.15
  when pay_level =3 then salary + salary*2
  end AS new_salary
  FROM employees 
  ;

```

### DATA SOURCE 
---
Analyst Builder
do check for [AlextheAnalyst](https://github.com/alextheanalyst) on Youtube 


#### highlight
---
This project requires the following filters:

1.  Using CASE statement
   
2. Level 1 gets a 10% increase (0.10)
   
3. Level 2 gets a 15% increase (0.15)
   
4. Level 3 gets a 200% increase (2)
   
5. new column to be named "new_salary"

