# Hadoop-MapReduce-Census-Report-
This project is to design a map program and a reduce program to solve the given census problem. The most important aspects of this design is to identify the key value pairs to be output by the mapper and worked by the reducer.


One of the advantages of cloud computing framework and the use of Map/Reduce paradigm is its ability to deal with very large data sets and one-time computations with a reasonable response time. This is done by using as many processors as needed. Typically, the map/reduce paradigm is used for these types of problems in contrast to the RDBMS approach which is better suited for storing, managing, and manipulating this data. Hadoop is a widely used open source map/reduce platform. Hadoop Map/Reduce is a software framework for writing applications which process vast amounts of data in parallel on large clusters. In this project, you will use the US census dataset and develop a program to compute a number of demographic statistics using Hadoop map/reduce paradigm. Please use the following links for a better understanding of Hadoop and Map/Reduce.
Dataset: consist of US census data for years 2009 to 2013.
i. Dataset size: 8 GB (two files and can be downloaded using the link given below)
ii. Coverage: all of US
iii. Large number of characteristics per person

Column No.
Attribute name
Description
0
SERIALNO
Unique identifier. Eg. 200900000001-201399999999 the first four digits represents year. There are five years – 2009, 2010, 2011, 2012, 2013
5
STATE
State Code; 1. Alabama/AL, 2. Alaska/AK 4. Arizona/AZ,
5. Arkansas/AR, 6. California/CA, 8. Colorado/CO,
9. Connecticut/CT, 10. Delaware/DE, 11. District of Columbia/DC, 12. Florida/FL, 13. Georgia/GA, 15. Hawaii/HI, 16. Idaho/ID, 17. Illinois/IL, 18. Indiana/IN,
19. Iowa/IA, 20. Kansas/KS, 21. Kentucky/KY,
22. Louisiana/LA, 23. Maine/ME, 24. Maryland/MD,
25. Massachusetts/MA, 26. Michigan/MI,
27. Minnesota/MN, 28. Mississippi/MS, 29. Missouri/MO, 30. Montana/MT, 31. Nebraska/NE, 32. Nevada/NV,
33. New Hampshire/NH, 34. New Jersey/NJ, 35. New Mexico/NM, 36. New York/NY, 37. North Carolina/NC,
38. North Dakota/ND, 39. Ohio/OH, 40. Oklahoma/OK, 41.Oregon/OR, 42. Pennsylvania/PA, 44. Rhode Island/RI, 45. South Carolina/SC, 46. South Dakota/SD,
47. Tennessee/TN, 48. Texas/TX, 49. Utah/UT,
50. Vermont/VT, 51. Virginia/VA, 53. Washington/WA,
54. West Virginia/WV, 55. Wisconsin/WI, 56. Wyoming/WY, 72. Puerto Rico/PR
The codes are not in sequence.
7
PWGTP
Person's weight; 1 to 9999 weight of person (in kilogram)
8
AGEP
Age; 00. Under 1 year, 01-99. 1 to 99 years
9
CIT
Citizenship status; 1. Born in the U.S., 2. Born in Puerto Rico, Guam, the U.S. Virgin Islands, .or the Northern Marianas, 3. Born abroad of American parent(s), 4. U.S. citizen by naturalization, 5. Not a citizen of the U.S.
The codes are in sequence.
69
SEX
Sex; Code is 1. Male, 2. Female
72
WAGP
Wages or salary income past 12 months;
bbbbbb. N/A (less than 15 years old) [Ignore],
000000. None [Ignore],
000001-999999. $1 to 999999
97
RAC1P
Recoded detailed race code; 1. White alone, 2. Black or African American alone, 3. American Indian alone, 4. Alaska Native alone, 5. American Indian and Alaska Native tribes specified; or American .Indian or Alaska Native, not specified and no other races, 6. Asian alone, 7. Native Hawaiian and Other Pacific Islander alone, 8. Some Other Race alone, 9. Two or More Races
The codes are in sequence.

There are 295 attributes. All the attributes are comma separated. The above table provides description of few attributes needed for your project. Use the appropriate attribute to solve the problem. You can ignore rest of the attributes. Also, Ignore null values.
The above data set can be downloaded from (right click on the link below). Contains 2 files each about 4GB.

Problem Specification:
i. we need to compute the weight trend over a few years for different states along genders using the given data. we need to develop a map/reduce solution.
For each of the following states, calculate average weight of males and females for each year and plot on a graph with year as the X-axis and avg. weight as the Y-axis. Note that this can be done for all states as well as in other ways. I have chosen 7 states to compare these trends: I) California, ii) Colorado, iii) North Dakota, iv) Texas, v) New York, vi) Maine, and vii) Florida.
ii) If we end up doing this project using different numbers of mappers and reducers, we can also visualize and understand the response time improvements when we use more number of mappers and reducers (divide and conquer)

