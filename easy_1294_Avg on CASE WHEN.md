<img src="https://github.com/leizhangg/SQL_leetcode_challenge/blob/main/img/1294-1.png">
<img src="https://github.com/leizhangg/SQL_leetcode_challenge/blob/main/img/1294_2.png">
<img src="https://github.com/leizhangg/SQL_leetcode_challenge/blob/main/img/1294_3.png">
<img src="https://github.com/leizhangg/SQL_leetcode_challenge/blob/main/img/1294_4.png">

### Solution:

When working with AVG (), the return type will be determined by the fist data type.    
Therefore, here the weather_state is int, the average of weather state will also be int. 
For example, 15.2 will be converted to 15, which will lead to error when using CASE WHEN
So, in order to make sure the data type is decimal, we could either use CAST (column AS DECIMAL()), 
or times the data with decimal point, thus it will become decimal. 

<img src="https://github.com/leizhangg/SQL_leetcode_challenge/blob/main/img/1294_solution_1.png">
<img src="https://github.com/leizhangg/SQL_leetcode_challenge/blob/main/img/1294_solution_2.png">
