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
import numpy as np

x = np.arange(20, 50)
y = np.arange(50, 80)
a = np.arange(80, 110)
b = np.arange(110, 140)

plt.scatter(x, y, c='b')
plt.xlabel('X-Axis')
plt.ylabel('Y-Axis')
plt.title('Graph in 2D')
plt.show()

```
<img width="747" height="575" alt="image" src="https://github.com/user-attachments/assets/0c575bc7-d751-4e91-a873-365eb636531f" />

```
plt.plot(x, y, 'b*', linestyle='dashed', linewidth=1, markersize=10)
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('2D Diagram')
plt.show()
plt.subplot(3, 2, 1)
plt.plot(x, y, 'r.')
plt.subplot(3, 2, 2)
plt.plot(x, y, 'b*')
plt.subplot(3, 2, 3)
plt.plot(x, y, 'yo')
plt.subplot(3, 2, 4)
plt.plot(x, y, 'g*')
plt.subplot(3, 2, 5)
plt.plot(x, y, 'r.--')
plt.subplot(3, 2, 6)
plt.plot(x, y, 'g*')
x = np.arange(1, 10)
y = x * x
plt.plot(x, y, 'ro')
plt.xlabel('X-Axis')
plt.ylabel('Y-Axis')
plt.title('Graph')
plt.show()
```
<img width="732" height="558" alt="image" src="https://github.com/user-attachments/assets/a1cbb82e-ce8b-4e55-9ec8-5ca7cad57885" />
<img width="759" height="569" alt="image" src="https://github.com/user-attachments/assets/93e215f3-6eaa-435d-9f17-83389f9f0a33" />

```
x = np.arange(0, 4 * np.pi, 0.1)
y = np.sin(x)
plt.title('Sine Wave')
plt.plot(x, y)
plt.show()
```
<img width="789" height="534" alt="image" src="https://github.com/user-attachments/assets/170b7042-7148-4873-96f1-3ac2c08b7711" />

```
x = np.arange(0, 6 * np.pi, 0.1)
y_sin = np.sin(x)
y_cos = np.cos(x)
plt.subplot(2, 1, 1)
plt.plot(x, y_sin, 'y-')
plt.title('Sine Wave')
plt.show()
plt.subplot(2, 1, 2)
plt.plot(x, y_cos, 'b-')
plt.title('Cos Wave')
plt.show()
```
<img width="764" height="588" alt="image" src="https://github.com/user-attachments/assets/4c5dc9e2-2de9-4646-adf4-8315ba28c38a" />

```
x = [2, 4, 6]
y = [3, 5, 7]
x2 = [12, 14, 16]
y2 = [13, 15, 17]
plt.bar(x, y, color='b')
plt.bar(x2, y2, color='y')
plt.title("Bar Graph")
plt.show()
```
<img width="706" height="540" alt="image" src="https://github.com/user-attachments/assets/4856f1ac-5253-45c7-b0f8-a86427876cc0" />

```
a = np.array([34, 65, 79, 90, 82, 10, 94, 39, 34, 92, 72, 49])
plt.hist(a)
plt.title("Histogram")
plt.show()
```
<img width="729" height="539" alt="image" src="https://github.com/user-attachments/assets/919ca291-af36-458b-b099-dec97354688a" />

```
a = [np.random.normal(0, std, 100) for std in range(1, 4)]
plt.boxplot(a, vert=True, patch_artist=True)
plt.show()
plt.boxplot(a, vert=False, patch_artist=False)
plt.show()
```
<img width="832" height="507" alt="image" src="https://github.com/user-attachments/assets/8eb7adfa-fbd4-4aa2-8c86-f10bb738db92" />
<img width="713" height="527" alt="image" src="https://github.com/user-attachments/assets/793f8e6f-ec2e-452a-92c8-07569f1a0805" />


```
labels = ['Maths', 'Science', 'English', 'Computer']
sizes = [85, 90, 75, 95]
colors = ['gold', 'lightblue', 'lightgreen', 'pink']
explode = (0, 0.2, 0, 0)
plt.pie(sizes, explode=explode, labels=labels, colors=colors, autopct='%.1f%%')
plt.title("Student Marks Distribution")
plt.axis('equal')
plt.show()
```
<img width="873" height="508" alt="image" src="https://github.com/user-attachments/assets/47530ca4-0676-4ab2-a889-7b96d9ab2b02" />

## Result:
Thus the Data visualisation was successfully done with the MatPlotlib.
