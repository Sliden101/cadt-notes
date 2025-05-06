# 1. Data

### 1.1 Data is divided into 2 categories, 
- qualitative (words, which can't be put into numbers)
- quantitative (discrete and continuous) 

#### 1.1.1 Discrete quantitative numbers 

- Numbers that isn't measured aka countable with a precise and defined "gap"

#### 1.1.2 Continous quantitative numbers

- numbers that are measured, without a clear "gap"

### 1.2 Outliers
- outliers are numbers that aren't within the normal range of our data or a data point that is too large or too small to fit within the confines of our data

most data comes unsorted and unfiltered which is why these outliers exist

# Table

Basically all problems at this stage just requires you to "organize" the data into something that actually human readable

### Discrete Tables

| $x_i$ | $f_i$ | $c.f$         | $i.c.f$               | ${r.c.f}$         | $r.i.c.f$           |
| ----- | ----- | ------------- | --------------------- | ----------------- | ------------------- |
| $x_1$ | $f_1$ | $f_1$         | $\Sigma{f_i}$         | $\frac{c.f_1}{n}$ | $\frac{i.c.f_1}{n}$ |
| $x_2$ | $f_2$ | $f_1+f_2$     | $\Sigma{f_i}-f_1-f_2$ | $\frac{c.f_2}{n}$ | $\frac{i.c.f_i}{n}$ |
| .     | .     | .             | .                     | .                 | .                   |
| $x_i$ | $f_i$ | $\Sigma{f_i}$ | $f_i$                 | $\frac{c.f_i}{n}$ | $\frac{i.c.f_i}{n}$ |
|       | $n$   |               |                       |                   |                     |

### Continous Tables 

let k be the amount of classes
n is the sample size
$$2^k=n$$
i is the size of the classes
$$i=\frac{H-L}{k}$$
$x_i$ is the middle of the classes

| classes | $x_i$ | $f_i$ | $f+$                | $c.f$         | $i.c.f$               | ${r.c.f}$         | $r.i.c.f$           |
| ------- | ----- | ----- | ------------------- | ------------- | --------------------- | ----------------- | ------------------- |
|         | $x_1$ | $f_1$ | $\frac{f_1}{n}*100$ | $f_1$         | $\Sigma{f_i}$         | $\frac{c.f_1}{n}$ | $\frac{i.c.f_1}{n}$ |
|         | $x_2$ | $f_2$ | $\frac{f_1}{n}*100$ | $f_1+f_2$     | $\Sigma{f_i}-f_1-f_2$ | $\frac{c.f_2}{n}$ | $\frac{i.c.f_i}{n}$ |
|         | .     | .     | .                   | .             | .                     | .                 | .                   |
|         | $x_i$ | $f_i$ | $\frac{f_i}{n}*100$ | $\Sigma{f_i}$ | $f_i$                 | $\frac{c.f_i}{n}$ | $\frac{i.c.f_i}{n}$ |
|         | x     | $n$   | $100$               |               |                       |                   |                     |

# 2. Analysis

### 2.1 Mode

| $x_i$ | 1   | 2   | 3   |
| ----- | --- | --- | --- |
| $f_i$ | 18  | 14  | 20  |

The variable with the highest frequency 
$M_0 = 3$

| $x_i$ | 1   | 2   | 3   |
| ----- | --- | --- | --- |
| $f_i$ | 20  | 14  | 20  |
If there are variables with the same amount of data points that are equally as high then there are that amount of modes as well

$M_0=1,M_0=3$

Mode for continuous is the class that has the highest amount of frequencies

| $\text{class}$ | [37-41[ | [41-45[ | [45-49[ |
| -------------- | ------- | ------- | ------- |
| $f_i$          | 119     | 14      | 20      |

$M_0 = \frac{45+49}{2} = 47$
### 2.2 Mean

Mean is just the average, usually denoted by $\bar{X}$

$\bar{X}=\frac{\Sigma{x_i}}{n}$

| $x_i$ | 1   | 2   | 3   |
| ----- | --- | --- | --- |
| $f_i$ | 20  | 14  | 20  |
$\bar{X}=\frac{\Sigma{f_ix_i}}{n},(n=\Sigma{f_i})$

### 2.3 Median

Usually denoted by $M_e$

The median literally means the middle value when sorted

| $x_i$ | 1   | 2   | 3   |
| ----- | --- | --- | --- |
| $f_i$ | 20  | 14  | 20  |

$n=20+14+20=54$ So the middle value is $\frac{54}{2}=27$
The 27th "element" is 2 so the median is 2

#### $$M_e(X)=\left\{\begin{array}{l} \frac{X[n+1]}{2} \text{ if n is odd} &\\ \frac{X[\frac{n}{2}]+X[\frac{n}{2}+1]}{2} \text{ if n is even} \end{array}\right.$$

### 2.4 Skewed-ness

$M_0=M_e=\bar{X}$ means that the graph is perfectly symmetrical

$M_0<M_e<\bar{X}$ Means that the graph is right-skewed, with more data points on the left side

$M_0>M_e>\bar{X}$ Means that the graph is left-skewed, with more data points on the right side

![[Pasted image 20250331125045.png]]

# 5. Measure of dispersion

### 5.1 Range

Range is the "distance" between the highest and lowest data points

$\text{Range} = H-L$
| $x_i$ | [20-30[ | [30-40[ | [40-50[ |
| ----- | ------- | ------- | ------- |
| $f_i$ | 20      | 14      | 20      |
$\text{Range}=[20:49]$

### 5.2 Mean Deviation

#### $MD=\frac{\Sigma{\mid{x_i-\bar{X}}\mid}}{n}, f=1$
#### $MD=\frac{\Sigma{\mid{x_i-\bar{X}}\mid}f_i}{n}, f>1$

both continous and discrete

### 5.3 Variance, $S^2$

#### $$S^2=\frac{\Sigma(x_i-\bar{X})^2}{n-1}=\frac{\Sigma{x_i^2}-\frac{(\Sigma{x_i})^2}{n}}{n-1}, f=1$$
#### $$S^2=\frac{\Sigma(x_i-\bar{X})^2f_i}{n-1}=\frac{\Sigma{f_ix_i^2}-\frac{\Sigma{f_ix_i}^2}{n}}{n-1}, f>1$$

$\text{Standard deviation is the square root of variance}$

$$S= \sqrt{S^2}$$

#### Theoretical Variance 

$V(x)\geq 0$
$$V(x)=E[(x-E(x))^2]=E(x^2)-E^2(x)$$

