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

```python
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=[2018,2019,2020,2021,2022]
y=[15000,20000,25000,30000,35000]
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('2D Diagram')
plt.show()
```
<img width="874" height="660" alt="image" src="https://github.com/user-attachments/assets/0452d318-eba0-4d4e-ba3c-40ed1944f47a" />

```python
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
```
<img width="855" height="616" alt="image" src="https://github.com/user-attachments/assets/4c454701-d3cc-4294-b52d-f2459f3c1e51" />

```python
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine waveform")
plt.plot(x,y)
plt.show()
```
<img width="855" height="647" alt="image" src="https://github.com/user-attachments/assets/b3ff73da-c8e5-4496-85b0-47b6ecc7107e" />

```python
x=[2,8,10]
y=[11,16,9]
x1=[3,9,11]
y1=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x1,y1,color='g')
plt.title("Bar graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
<img width="844" height="665" alt="image" src="https://github.com/user-attachments/assets/2e346858-a227-4a09-8f73-f8aaf99b4032" />
```python
x=[1,2,3]
y=[7,3,9]
plt.plot(x,y,color='g')
plt.title("Line graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
<img width="836" height="681" alt="image" src="https://github.com/user-attachments/assets/1b99a11d-4b87-41e2-a716-e3a0259f54be" />

```python
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label='line1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label='line2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```
<img width="852" height="642" alt="image" src="https://github.com/user-attachments/assets/dbe5eda9-9b7e-4bb2-b372-44f6260bf1a3" />

```python
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='red',markersize=12,label='spices')
plt.ylim(1,8)
plt.xlim(1,8)
plt.title("line graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```
<img width="843" height="673" alt="image" src="https://github.com/user-attachments/assets/6a3694c8-1498-45d7-b5d5-ccc76bdfb81d" />

```python
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples,linestyle="dashed",linewidth=3,marker="*",markersize=12,color='g')
plt.show()
```
<img width="841" height="612" alt="image" src="https://github.com/user-attachments/assets/11a5ca59-6191-4afd-b6d4-990b244144d2" />

```python
oranges=[2,4,6,7,8,12,45]
apples=[2,4,5,6,8,23,37]
years=[2019,2020,2021,2022,2023,2024,2025]
plt.plot(years,apples,marker='o')
plt.plot(years,oranges,marker='*')
plt.title("Crop yields in Kanto")
plt.xlabel("Year")
plt.ylabel("Yield (tons per hectare)")
plt.legend(['apples','oranges'])
plt.show()
```
<img width="843" height="667" alt="image" src="https://github.com/user-attachments/assets/89eaeebf-85ed-413c-adee-ee80673c781f" />

```python
oranges=[2,4,6,7,8,12]
apples=[2,4,5,6,8,23]
years=[2019,2020,2021,2022,2023,2024]
plt.bar(oranges,apples)
plt.plot(years,apples,label="apples",marker='*')
plt.plot(years,oranges,label="oranges",marker='o')
plt.title("Fruit Sales")
plt.xlabel("x-axis")
plt.ylabel("y-axis")
plt.legend()
plt.show()
```
<img width="832" height="674" alt="image" src="https://github.com/user-attachments/assets/89fa0357-0342-4ccf-b523-449fd36c0b57" />

```python
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o',label='oranges')
plt.title("Yield of oranges (tons per hectare)")
plt.legend()
```
<img width="881" height="484" alt="image" src="https://github.com/user-attachments/assets/a6550c4f-dc14-4923-94eb-7911d972606c" />

```python
print("Scatter plot is")
x=[1,2,3,4,5,6,7,8,9,10]
y=[2,4,5,7,6,8,9,11,12,12]
plt.scatter(x,y,label="star",color="green",marker="*",s=30)
plt.title("Scatterplot")
plt.xlabel("x-axis")
plt.ylabel("y-axis")
plt.legend()
plt.show()
```
<img width="838" height="675" alt="image" src="https://github.com/user-attachments/assets/e763b1cc-ba5f-47ab-88e6-a74a1e25aeb0" />
```python
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color="green",label="y1")
plt.fill_between(x,y2,color="blue",label="y2")
plt.fill_between(x,y3,color="red",label="y3")
plt.title("Fill between")
plt.legend()
plt.show()
```
<img width="851" height="653" alt="image" src="https://github.com/user-attachments/assets/8e5bf0f9-a3bb-4b0f-92e7-6713ddf17ac2" />

```python
plt.stackplot(x,y1,y2,y3,labels=['line1','line2','line3'])
plt.legend()#by default aligned to left in jupyter. give loc="upper left" in collab
plt.title("Stacked line chart")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
<img width="847" height="662" alt="image" src="https://github.com/user-attachments/assets/5a9766c7-e1b6-45ba-9eaa-e716a232149c" />

```python
from scipy.interpolate import make_interp_spline
x=np.array([1,2,3,4,5,6,7,8,9,10])
y=np.array([2,4,5,7,8,9,10,11,12,13])
spl=make_interp_spline(x,y)
x_smooth=np.linspace(x.min(),x.max(),100)
y_smooth=spl(x_smooth)
plt.plot(x,y,'o',label='data')
plt.plot(x_smooth,y_smooth,'-',label="spline")
plt.legend()
plt.show()
```
<img width="817" height="622" alt="image" src="https://github.com/user-attachments/assets/a5701bbb-c9b6-4c20-b69c-1971f89b195f" />

```python
values=[5,6,7,3,2]
names=['A','B','C','D','E']
plt.bar(names,values,color='green')
plt.show()
```
<img width="803" height="603" alt="image" src="https://github.com/user-attachments/assets/a5e558a9-baa4-4461-8cd1-e19b954e2da1" />

```python
ages=[2,5,70,40,45,50,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range1=(0,100)
bins=10
plt.hist(ages,bins,range1,color="green",histtype="bar",rwidth=0.8)
plt.xlabel('ages')
plt.ylabel('no.of people')
plt.title('my histogram')
plt.show()
```
<img width="828" height="673" alt="image" src="https://github.com/user-attachments/assets/317c0f86-0692-4ba6-b724-da6449f4e6d3" />

```python
cx=[2,1,6,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color="green",alpha=0.5)
plt.show()
```
<img width="800" height="622" alt="image" src="https://github.com/user-attachments/assets/fa19512f-b994-4b9e-add0-dffce1fd3b41" />

```python
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
<img width="798" height="538" alt="image" src="https://github.com/user-attachments/assets/955cb047-6e07-4ce7-8c9c-4b538cebfc0d" />

```python
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('x-axis')
ax.set_ylabel('y-axis')
ax.set_title('box plot')
```
<img width="862" height="664" alt="image" src="https://github.com/user-attachments/assets/32ba9949-aff2-4bf0-b01a-0a8257e5fc26" />

```python
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct="X1.1")
plt.legend()
plt.show()
```
<img width="712" height="597" alt="image" src="https://github.com/user-attachments/assets/376bd48f-6879-49aa-bae9-5c3922df7968" />

```python
labels='python','C+','ruby','java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,colors=colors,labels=labels,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
<img width="648" height="575" alt="image" src="https://github.com/user-attachments/assets/6128f7f1-ae53-461e-ac7c-d1dfe0a8f621" />


























# Result:
Data Visualization has been performed using matplot python library for the given datas.

