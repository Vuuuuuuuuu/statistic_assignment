### 1.Measures of Central Tendency: 
```python
y= [12, 15, 14, 10, 18, 20, 22, 24, 17, 19] 
mean= sum(y)/len(y)
n= len(y)
print("mean= ",mean)
if len(y)%2==0:
  median = (y[int(len(y)/2)-1]+y[int(len(y)/2)])/2
else:
  median = y[len]
print("median= ",median)

mode={}

for num in y:
    mode[num] = mode.get(num, 0) + 1
    
max_frequency = max(mode.values())

mode = [num for num, freq in mode.items() if freq == max_frequency]
print(mode)

if max_frequency == 1:
    print("no mode")  
else:
    print("mode", mode)
```

### 2 Percentiles and Quartiles:
``` python
x=sorted(y)
Q1= x[int(len(y)*0.25)]
print("Q1", Q1)
Q2=x[int(len(y)*0.5)]
print("Q2", Q2)
Q3= x[int(len(y)*0.75)]
print("Q3",Q3)
```

### 3. Interquartile Range (IQR):
```python
IQR= x[int(len(y)*0.75)]-x[int(len(y)*0.25)]
print("IQR",IQR)
```
### 4. Min and Max: 
```python
print("min",min(y))
print("max",max(y))
```
### 5. Finding Outliers Using Quartiles: 
```python
LB= Q1-1.5*IQR
UB= Q3+1.5*IQR

print("lower bound",LB)
print("upper bound",UB)
if x[0]< LB:
  print("lower outlier", x[0])
else:
  print("no lower outlier")
if x[len(x)-1]> UB:
  print("upper outlier", x[len(x)])
else:
  print("no upper outlier")
```
### 6.Measures of Dispersion:
```python
range= max(y)-min(y)
print("range",range)
yv=[]
i=0
while i<10:
 yv.append((y[i]-mean)**2)
 i+=1
var= sum(yv)/(len(y)-1)
print("var",var)
std= var**0.5
print("std",std)
```
### 7. Z-score Standardization:
```python
i=0 
zscore=[]
while i<10:
  zscore.append((y[i]-mean)/std)
  i+=1
print("zscore",zscore)
```

### 9.scatterplot
```python
import matplotlib.pyplot as plt

a = [10, 20, 30, 40, 50]
b = [5, 10, 15, 20, 25]

plt.scatter(a,b)
plt.show() 

```
