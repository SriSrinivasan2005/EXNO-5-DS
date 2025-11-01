### EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

### Aim:
To Perform Data Visualization using matplot python library for the given datas.

### EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

### Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

### Coding and Output:
```
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```
### Line Plot
```
marks=[13,45,63,78]
student=['ABC','QOR','EFB','TOB']
plt.plot(marks,student)
plt.xlabel('Marks')
plt.ylabel('Student name')
plt.show()
```
<img width="881" height="724" alt="Screenshot 2025-10-28 113316" src="https://github.com/user-attachments/assets/ee586218-b53b-4f3f-8ddc-c09f21922d3f" />

```
student=['A','B','C','D']
attendence=[90,85,73,88]
plt.plot(attendence,student)
plt.xlabel('Attendence')
plt.ylabel('Student name')
plt.show()
```
<img width="912" height="716" alt="Screenshot 2025-10-28 113325" src="https://github.com/user-attachments/assets/10221c39-6c31-40d2-9819-611f21302801" />

### Scatter Plot
```
x=[10,20,30,40,50]
y=[100,200,300,400,500]
plt.scatter(x,y,label='stars',color='green',marker='*',s=30)
plt.show()
```
<img width="874" height="640" alt="Screenshot 2025-10-28 113339" src="https://github.com/user-attachments/assets/c7d9a511-e31a-4451-830d-7c3c13b45154" />

```
x=np.arange(0,15)
y=np.arange(0,15)
x
y
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('y axis')
plt.title('Scatter plot')
plt.show()
```
<img width="785" height="805" alt="Screenshot 2025-10-28 113354" src="https://github.com/user-attachments/assets/73cd5f99-d455-4b02-8d66-7c65aab035b2" />

### Pie Chart
```
act=['eat','sleep','work','play']
slices=[3,7,8,6]
color=['r','y','g','b']
plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```
<img width="1254" height="703" alt="Screenshot 2025-10-28 113413" src="https://github.com/user-attachments/assets/fc54a36f-3218-4766-b732-e64ec4fd429e" />


```
feedback=['Good','excellent','Perfect','Ok']
slices=[4,10,3,8]
color=['y','r','b','g']
plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```
<img width="1293" height="692" alt="Screenshot 2025-10-28 113429" src="https://github.com/user-attachments/assets/70b480c0-b847-4288-8706-ac85042bee7f" />

### Area Chart
```
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```

<img width="824" height="795" alt="Screenshot 2025-10-28 113443" src="https://github.com/user-attachments/assets/69af385d-4e93-40c2-ac90-c0d51cbdd9b9" />

### Bar Chart
```
height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green'] 
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()
```
<img width="829" height="805" alt="Screenshot 2025-10-28 113503" src="https://github.com/user-attachments/assets/6065edbc-e5f9-4c54-a533-fe3bacbeb75e" />

### Histogram
```
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```
<img width="837" height="631" alt="Screenshot 2025-10-28 113514" src="https://github.com/user-attachments/assets/cc8320bc-aca0-420b-9b67-d576e8c8ce94" />

### Box Plot
```
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```
<img width="853" height="550" alt="Screenshot 2025-10-28 113532" src="https://github.com/user-attachments/assets/ec8a0108-9659-4d0d-acc0-9441f6f35fb3" />

```
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
<img width="849" height="749" alt="Screenshot 2025-10-28 113551" src="https://github.com/user-attachments/assets/8c235da2-cccc-4d03-9245-c18bdd2314f1" />




### Result:
Thus, all the data visualization techniques of matplotlib has been implemented.
