# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.plot(x_values,y_values)
plt.show()
```
<img width="757" height="582" alt="image" src="https://github.com/user-attachments/assets/ad43a2df-9a7e-4b60-b337-f15cfcadc70a" />

```
x=[1,2,3]
y=[2,4,1]
plt.plot(x,y)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My first graph')
plt.show()
```
<img width="793" height="636" alt="image" src="https://github.com/user-attachments/assets/c36f18c8-b42c-4e49-9b59-06ffc68dc0cf" />

```
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label="line 1")
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label="line 2")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph')
plt.legend()
plt.show()
```
<img width="794" height="642" alt="image" src="https://github.com/user-attachments/assets/a47afed7-efdb-46ba-b90e-41e85bf2d10b" />

```
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue') # Added closing quote and a color 'blue'
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations')
plt.show()
```
<img width="772" height="634" alt="image" src="https://github.com/user-attachments/assets/384de83b-84f1-46f5-8bc6-911dcde36723" />

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```
<img width="802" height="591" alt="image" src="https://github.com/user-attachments/assets/24a30349-0abc-41db-8060-3c1da355b370" />

```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9375,0.895] 
oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.895] 
plt.plot(years , apples)
plt.plot(years,oranges)
plt.xlabel('Year')
plt.ylabel('Yield(tons per hectare)')
```
<img width="811" height="606" alt="image" src="https://github.com/user-attachments/assets/665f6228-752f-4784-ad18-a2ffdc410d51" />

```
plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel('Year')
plt.ylabel('Yield(tons per hectare)')
plt.title("Crop yield in Kanto")
plt.legend(['Apples','Oranges'])
```
<img width="810" height="633" alt="image" src="https://github.com/user-attachments/assets/c285ed70-800a-4a34-be2f-e58a07ce44f9" />

```
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
plt.xlabel('Year')
plt.ylabel('Yield(tons per hectare)')
```
<img width="827" height="614" alt="image" src="https://github.com/user-attachments/assets/b1dcbd63-940a-4605-a8d7-613a6d2dd110" />

```
plt.figure(figsize=(12,6))
years=range(2000,2012)
plt.plot(years,oranges,marker='o')
plt.title("Yield of oranges (tons per hectare)")
```
<img width="1265" height="680" alt="image" src="https://github.com/user-attachments/assets/53b7e61e-57d2-4c4f-937e-9d055c60481a" />

```
plt.plot(years,apples,marker='o')
plt.plot(years,oranges,marker='x')
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title("Crop Yields in kanto")
plt.legend(['Apples','Oranges'])
```
<img width="788" height="605" alt="image" src="https://github.com/user-attachments/assets/6236c753-fae9-40c1-8909-7fcf62380ec1" />

```
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.scatter(x_values,y_values,s=30,color="red")
plt.show()
```
<img width="737" height="560" alt="image" src="https://github.com/user-attachments/assets/865bdba4-395a-4ade-b93f-6532b9703da3" />

```
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
<img width="775" height="599" alt="image" src="https://github.com/user-attachments/assets/9fba66f9-5c3e-4186-9667-d516a325557e" />

```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('x axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
```
<img width="769" height="613" alt="image" src="https://github.com/user-attachments/assets/389ef655-3436-4ae8-aeb7-f18484776d83" />

```
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g*--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
```
<img width="731" height="569" alt="image" src="https://github.com/user-attachments/assets/d97b87d9-6851-45e8-a108-40ee35d9c718" />

```
import numpy as np
np.pi
```
<img width="185" height="27" alt="image" src="https://github.com/user-attachments/assets/76be02dd-69ad-4710-b1f4-9854638c4510" />

```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```
<img width="778" height="595" alt="image" src="https://github.com/user-attachments/assets/bb078d28-aa33-4244-9273-b97ba3949a6b" />

```
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
```
<img width="747" height="568" alt="image" src="https://github.com/user-attachments/assets/e5751aaf-6cee-41e3-ab0f-de6e83afad35" />

```
from scipy.interpolate import make_interp_spline
x=np.array([1,2,3,4,5,6,7,8,9,10])
y=np.array([2,4,5,7,8,8,9,10,11,12])
spl=make_interp_spline(x,y)
x_smooth=np.linspace(x.min(),x.max(),100)
y_smooth=spl(x_smooth)
plt.plot(x,y,'o',label='data')
plt.plot(x_smooth,y_smooth,'-',label='Spline')
plt.legend()
plt.show()
```
<img width="726" height="568" alt="image" src="https://github.com/user-attachments/assets/8f700898-fc6c-48a7-9960-d0d48a533e0e" />

```
values=[5,6,3,7,2]
names=["A","B","C","D","E"]
plt.bar(names,values,color="green")
plt.show()
```
<img width="731" height="567" alt="image" src="https://github.com/user-attachments/assets/281b0223-aa29-4d30-bef8-4c040a859435" />

```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```
<img width="765" height="619" alt="image" src="https://github.com/user-attachments/assets/ccb40b4f-5a3a-40ae-b71d-72035b007e2a" />

```
x=[2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color='blue',alpha=0.5)
plt.show()
```
<img width="731" height="569" alt="image" src="https://github.com/user-attachments/assets/b935c832-2fcc-4242-b30e-2c6101c9102d" />

# Result:
Thus, all the data visualization techniques of matplotlib has been implemented.
