```
                                                           Name: M.Srikaran
                                                           Reg no: 212223040206
```
# EX-3:Correlation and regression for data analysis
# Aim : 

To analyse given data using coeffificient of correlation and regression line
![image](https://user-images.githubusercontent.com/104613195/168224136-d6b64e64-7d3d-4775-9337-c8f96fe41f2d.png)


# Software required :  

Python

# Theory:

Correlation describes the strength of an association between two variables, and is completely symmetrical, the correlation between A and B is the same as the correlation between B and A. However, if the two variables are related it means that when one changes by a certain amount the other changes on an average by a certain amount.  

If y represents the dependent variable and x the independent variable, this relationship is described as the regression of y on x. The relationship can be represented by a simple equation called the regression equation. The regression equation representing how much y changes with any given change of x can be used to construct a regression line on a scatter diagram, and in the simplest case this is assumed to be a straight line.

# Procedure :

![image](https://user-images.githubusercontent.com/104613195/168225866-ac8f6610-bdc3-4ac2-a24e-2b24ba08e189.png)

# Program :
```
import matplotlib.pyplot as plt 
x=[int(i) for i in input().split()] 
y=[int(i) for i in input().split()]
N=len(x)
Sx=0
Sy=0
Sxy=0
Sx2=0
Sy2=0
for i in range(0,N):
    Sx=5x+x[i]
    Sy=Sy+y[i]
    Sxy=Sxy+x[i]*y[i]
    Sx2=5x2+x[i]**2
    Sy2=Sy2+y[i]**2
r=(N*Sxy-Sx*Sy)/(math.sqrt(N*Sx2-Sx**2)*math.sqrt(N*Sy2-Sy**2))
print("The Correlation coefficient is %0.3f"%r)
byx=(N*Sxy-Sx*Sy)/(N*5x2-5x**2)
xmean=Sx/N
ymean=Sy/N
print("THe Regression line Y on X is ::: y
plt.scatter(x,y)
def Reg(x):
    return ymean + byx*(x-xmean)
x=np.linspace(0,80,51)
y1=Reg(x)
plt.plot(x,y1, 'r')
plt.xlabel('x-data')
plt.ylabel('y-data')
plt.legend (['Regression Line', 'Data points'])
```

# Output 
![pro ex03](https://github.com/prideeshm/Correlation_Regression/assets/144870483/f83f5459-c86a-48f0-902f-3d896c4b89ee)

# Result
The Correlation and regression for data analysis of objects from feeder using probability distribution are calculated.
