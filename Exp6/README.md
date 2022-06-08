# Poisson Process

# Aim: 
To find the probability of that (i) exactly 4 customers arrive (ii) more than 4 customers arrive (iii) fewer than 4 customers. Given that the customers arrive at a bank according to a Poisson process with mean rate of 3 per minute during a time interval of 2 min.
# Software required:  

Python

# Theory:

The Poisson process is one of the most widely-used counting processes. It is usually used in scenarios where we are counting the occurrences of certain events that appear to happen at a certain rate, but completely at random (without a certain structure). For example, suppose that from historical data, we know that earthquakes occur in a certain area with a rate of 2 per month. Other than this information, the timings of earthquakes seem to be completely random. Thus, we conclude that the Poisson process might be a good model for earthquakes. In practice, the Poisson process or its extensions have been used to model.

1. The number of car accidents at a site or in an area
2. The location of users in a wireless network
3. The requests for individual documents on a web server

 
# Procedure:

![image](https://user-images.githubusercontent.com/104613195/172528169-f26bdf76-f357-4c48-b806-a0a80da21cac.png)

# Program:
```
# Developed by: Y Chethan
# Register Number: 212220230008

import numpy as np
import math

l=3
t=2
def p(x):
    return ((math.exp(-l*t))*((l*t)**x))/(math.factorial(x))

print("The Probability that exactly 4 customers arrive is ",p(4))

sum=0
for i in range(0,5):
    sum+=p(i)
print("The Probability that more than 4 customers arrive is ",1-sum)

sum_1=0
for i in range(0,4):
    sum_1+=p(i)
print("The Probability that fewer than 4 customers arrive is ",sum_1)
```
# Output: 
![image](https://user-images.githubusercontent.com/75234991/172535141-deb6f33b-29f0-43cb-9363-90d54cafa518.png)
![image](https://user-images.githubusercontent.com/75234991/172535153-a389a74f-feaf-4ff1-95df-9406e16b9133.png)
![image](https://user-images.githubusercontent.com/75234991/172535148-a1356501-e23f-4c47-bacf-c3bf59338601.png)

# Result:
Thus, the python program to find the probabilities for the given poisson process has been implemented.
