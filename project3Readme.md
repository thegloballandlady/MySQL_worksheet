# MYSQL PROJECT_3
---

[QUESTION](#question)

[MY ANSWER](#my-answer)

[DATA SOURCE](#data-source) 

### QUESTION 
---
I love chocolate and only want delicious baked goods that have chocolate in them!

Write a Query to return bakery items that contain the word "Chocolate".

product_name
Double Chocolate Doughnut
Sweet Loaf
Croissant
Chocolate Banana Muffin
Glazed Doughnut
Cinnamon Roll
Cheese Danish
Peanut Butter Chocolate Pound Cake
Fruit Tart


### MY ANSWER 
---
```SQL
SELECT * 
  FROM bakery_items 
  where product_name like "%Chocolate%"
  ;
```

### DATA SOURCE 
---
Analyst Builder
do check for [AlextheAnalyst](https://github.com/alextheanalyst) on Youtube 

#### highlight
This project requires the following filters
1. To use the where statement
2. To use the like statement % also
