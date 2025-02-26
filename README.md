# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula. 
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
4. Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
5. Use the slope m and the y -intercept to form the equation of the line.
6. Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
    import numpy as np
    import matplotlib.pyplot as plt
    x=np.array(eval(input()))
    y=np.array(eval(input()))
    print(x_mean)
    print(y_mean)
    num,denom=0,0
    for i in range(len(x)):
        num+=((x[i])-x_mean)*((y[i])-y_mean)
        denom+=((x[i])-x_mean)**2
        m=num/denom
        b=y_mean-m*x_mean
    print(m,b)
    y_predicted=m*x+b
    y_predicted
    plt.scatter(x,y,color='black')
    plt.plot(x,y_predicted,color='red')
    plt.show()
## Output:
![image](https://github.com/user-attachments/assets/e1332322-69aa-4d23-929d-7e2e5c8d12e4)


![image](https://github.com/user-attachments/assets/ed241761-597e-4744-8ec5-0b329e0bbd10)


![image](https://github.com/user-attachments/assets/7f6ee045-ebb5-4a84-8d12-467af1301782)


![image](https://github.com/user-attachments/assets/b58e6b6b-2dc9-45fa-ab09-871d15416394)


![image](https://github.com/user-attachments/assets/653f5c08-9284-4ed0-9281-992641c73c7e)


![image](https://github.com/user-attachments/assets/85826c1d-d9e6-4372-bfc5-8ded105079b7)





## Result:
 
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
