###  Q17
``` python
y= [45, 50, 55, 60, 62, 48, 52]
mean= sum(y)/len(y)

n=int(len(y))
r=[]
for i in range(n):
 r.append((y[i]-mean)**2)
print(sum(r))
s= (sum(r)/6)**0.5
print(s)
t=(mean-50)/(s/(n**0.5))
print(t)
```

6.22972903178973
t=1.3347640585603673
t stat= 2.4
significant
### Q18
```
y=[85, 90, 88, 92, 86]
x=[78, 75, 80, 83, 79]
xmean = sum(x)/len(x)
ymean =sum(y)/len(y)
print("a mean= ",ymean)
print("b mean= ",xmean)
yn= int(len(y))
xn= int(len(x))
yp=[]
for i in range(yn):
 yp.append((y[i]-ymean)**2)
s1= (sum(yp)/4)**0.5
print(sum(yp))
print("s1= ",s1)
xp=[]
for i in range(xn):
 xp.append((x[i]-xmean)**2)
s2= (sum(xp)/4)**0.5
print(sum(xp))
print("s2= ",s2)
sp=(((yn-1)*s1**2)+((xn-1)*s2**2))/(yn+xn- 2)
print("sp= ",sp)
t=(ymean-xmean)/((sp*((1/yn)+(1/xn)))**0.5)
print("t= ", t)
```
a mean=  88.2
b mean=  79.0
32.8
s1=  2.8635642126552705
34.0
s2=  2.9154759474226504
sp=  8.35
t=  5.034016027514163
1.86
t stat=1.860
not significant
### Q19
NOT SIGNIFICANT
### Q20
#### DESCRIPTIVE
 Descriptive statistics summarize and describe the main features of a dataset. They provide a clear and concise way to understand the data without making generalizations beyond the dataset.
- Business: Summarizing sales data to identify trends (e.g., average monthly sales, most popular products).

- Healthcare: Describing patient demographics (e.g., average age, gender distribution) in a hospital.

- Education: Reporting average test scores and pass rates for a school district.
#### INFERENTIAL
Inferential statistics use sample data to make predictions, inferences, or generalizations about a larger population. They help draw conclusions beyond the immediate data.
- Marketing: Predicting customer behavior based on survey data (e.g., likelihood of purchasing a product).

- Public Policy: Estimating the impact of a new policy on unemployment rates using sample data.

- Quality Control: Inferring the quality of an entire production batch by testing a sample of products.

