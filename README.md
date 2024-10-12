# MySQL_Project 1
---

 ### QUESTION
---
Dr. Obrien has seen an uptick in heart attacks for his patients over the past few months. He has been noticing some trends across his patients and wants to get ahead of things by reaching out to current patients who are at a high risk of a heart attack.

We need to identify which clients he needs to reach out to and provide that information to Dr. Obrien.

If a patient is over the age of 50, cholesterol level of 240 or over, and weight 200 or greater, then they are at high risk of having a heart attack.

Write a query to retrieve these patients. Include all columns in your output.

As Cholesterol level is the largest indicator, order the output by Cholesterol from Highest to Lowest so he can reach out to them first.

patient_id	age	cholesterol	weight
1001	52	373	267
1002	93	235	164
1003	77	324	211
1004	65	245	216
1005	51	218	258
1006	33	195	246
1007	34	307	239
1008	49	199	213
1009	61	266	244
1010	61	257	192
1011	63	140	187
1012	31	398	175
1013	78	361	184
1014	72	365	170
1015	82	282	269

### MY_ANSWER
---
``` SELECT * 
  FROM patients 
  WHERE AGE > 50
  AND CHOLESTEROL >= 240
  AND WEIGHT >= 200
  ORDER BY CHOLESTEROL DESC
  ;


### DATA_SOURCE: ANALYST BUILDER
---
Do click to AlextheAnalyst on youtube
