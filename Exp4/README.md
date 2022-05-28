# Correlation and Regression for Data Analysis
# Aim: 

To analyse given data using coefficient of correlation and regression line.
![image](https://user-images.githubusercontent.com/104613195/168224136-d6b64e64-7d3d-4775-9337-c8f96fe41f2d.png)


# Software required:  

Python

# Theory:

Correlation describes the strength of an association between two variables, and is completely symmetrical, the correlation between A and B is the same as the correlation between B and A. However, if the two variables are related it means that when one changes by a certain amount the other changes on an average by a certain amount.  

If y represents the dependent variable and x the independent variable, this relationship is described as the regression of y on x. The relationship can be represented by a simple equation called the regression equation. The regression equation representing how much y changes with any given change of x can be used to construct a regression line on a scatter diagram, and in the simplest case this is assumed to be a straight line.

<br><br><br><br><br><br><br><br><br><br>

# Procedure:

![image](https://user-images.githubusercontent.com/104613195/168225866-ac8f6610-bdc3-4ac2-a24e-2b24ba08e189.png)

# Program:
```
# Developed by: Y Chethan
# Register Number: 212220230008

import numpy as np
import math
import matplotlib.pyplot as plt
def f(x):
    return ymean+byx*(x-xmean)

x=[25,28,35,32,31,36,29,38,34,32]
y=[43,46,49,41,36,32,31,30,33,39]

sx=0
sy=0
sxy=0
sx2=0
sy2=0
for i in range(0,10):
    sx=sx+x[i]
    sy=sy+y[i]    
    sxy=sxy+x[i]*y[i]
    sx2=sx2+x[i]**2
    sy2=sy2+y[i]**2
N=10
r=(N*sxy-sx*sy)/(math.sqrt(N*sx2-sx**2)*math.sqrt(N*sy2-sy**2))
print("The Correlation Coefficient is %0.3f"%r)

byx=(N*sxy-sx*sy)/(N*sx2-sx**2)
xmean=sx/N
ymean=sy/N
print("The regression line Y on X is ::: Y = %0.3f + (%0.3f) * (X - %0.3f)"%(ymean,byx,xmean))

plt.scatter(x,y)
def reg(x):
    return ymean+byx*(x-xmean)
x1=np.linspace(20,40,101)
y1=reg(x1)
plt.plot(x1,y1,'y')
plt.xlabel("X")
plt.ylabel("Y")
plt.title("Regression Line")
plt.legend(["Regression line","Data points"],loc=3)
plt.show()
```
# Output:

<img width="244" alt="image" src="https://user-images.githubusercontent.com/75234991/170812582-71cde67c-2a25-47d1-98ef-9cba3b9108b7.png">

<img width="432" alt="image" src="https://user-images.githubusercontent.com/75234991/170812588-41823daf-eb1e-430c-a810-9d3841d2ddc2.png">

![image](https://user-images.githubusercontent.com/75234991/170812591-c3d847e4-2c85-4ccb-b805-04036c564bd3.png)

<br><br><br>

# Result:
Thus, given data is analysed using coefficient of correlation and regression line.
