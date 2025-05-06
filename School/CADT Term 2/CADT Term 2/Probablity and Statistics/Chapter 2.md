# Mean definition

### $$\bar{X}=\frac{1}{n}(x_1+x_2+...+x_n)=\frac{1}{n}\Sigma_{i=1}^{n}{(x_i)}$$

### Example 2:
- let x be the stats score
- we have data (realization of X the student's stats score) as following
	 7 8 9 5 7 8 7 9 6 8

- questions:
- a. find average deduce formula for mean
- b. construct freqency tqable
- c. deduce second formula for mean from b
- d. calculate the sum of $\Sigma_{i=1}^{n}(X_i-\bar{X})$ and then intepret the result
- e.prove the result in d

a. Average: $$\bar{X}=\frac{7+8+9+5+7+8+7+9+6+8}{10}=7.4$$
Thus: $\bar{X}=\frac{1}{n}(x_1+x_2+...+x_n)$

b. 

| $x_i$ | $f_i$ | $c.f$ | $i.c.f$ | ${r.c.f}$ | $r.i.c.f$ | $X_i-\bar{X}$ |
| ----- | ----- | ----- | ------- | --------- | --------- | ------------- |
| 5     | 1     | 1     | 10      | 1/10      | 10/10     | 2.4           |
| 6     | 1     | 2     | 9       | 2/10      | 9/10      | 1.4           |
| 7     | 3     | 5     | 8       | 5/10      | 8/10      | 0.4           |
| 8     | 3     | 8     | 5       | 8/10      | 5/10      | -0.6          |
| 9     | 2     | 10    | 2       | 10/10     | 2/10      | -1.6          |
|       | 10    |       |         |           |           |               |

c. since we have the frequency of each data points
$$\bar{X}=\frac{1}{n}(x_1*f_1+x_2*f_2+...+x_i*f_i)=\frac{1}{n}\Sigma^{n}_{i=1}(x_i*f_i)$$

d. $$2.4+1.4+3(0.4)+3(-0.6)+2(-1.6) = 0$$
mean is correct



### Example 4:

A: 5,7,8,6,4
B: 10,2,3,7,9

$$MD=\frac{\Sigma{\mid{x_i-\bar{X}}\mid}}{n}, f=1$$
$MD_A:(1+1+2+0+2)/5=6/5=1.2$ 
$MD_B:(3.8+4.2+3.2+1.2+2.8)/5=3.04$

$$S^2=\frac{\Sigma(x_i-\bar{X})^2}{n-1}$$

$S^2_A:(1+1+4+4)/4=2.5$
$S^2_B:(3.8^2+4.2^2+3.2^2+1.2^2+2.8^2)/4=12.9$

$$S= \sqrt{S^2}$$

$S_A=1.58$
$S_B=3.59$

$$CV=\frac{SD}{\bar{X}}$$

|           | A       | B        |
| --------- | ------- | -------- |
| $\bar{X}$ | $6$     | $6.2$    |
| $MD$      | $1.2$   | $3.04$   |
| $S^2$     | $2.5$   | $12.9$   |
| $SD$      | $1.58$  | $3.59$   |
| $CV$      | $0.263$ | $0.579;$ |


