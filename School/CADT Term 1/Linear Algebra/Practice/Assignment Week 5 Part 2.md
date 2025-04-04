# 68-81/212
# I. Matrices
### 68. 
$\text{Show that all square matrices can be expressed as the sum of a symmetric matrix and skew-symmetric matrix?}$
$$\text{Let A be a square matrix, then } A=\frac{1}{2}(A+A^T)+\frac{1}{2}(A-A^T)=P+Q$$
$$\text{Where } P=\frac{1}{2}(A+A^T),Q=\frac{1}{2}(A-A^T)$$
$$P^T=\frac{1}{2}(A+A^T)^T=\frac{1}{2}[A^T+{(A^T)}^T]=\frac{1}{2}(A^T+A)$$
$$\text{So P is a symmetric matrix}$$
$$Q^T=\frac{1}{2}(A-A^T)^T=\frac{1}{2}[A^T-{(A^T)}^T]=\frac{1}{2}(A^T-{A})$$
$$Q^T=-Q=>\text{Q is a skew symmetric matrix}$$
$$A=P+Q, \text{We have A expressed as a the sum of a symmetric and skew symmetric matrix}$$
$$\text{Let A=W+L where W is a symmetric and L is a skew symmetric matrix}$$
$$A^T=(W+L)^T=W^T+L^T=W-L$$
$$=>W=\frac{1}{2}(A+A^T)=P,L=\frac{1}{2}(A-A^T)=Q$$
$$\text{Hence, A is  expressed as the sum of a symmetric matrix and skew-symmetric matrix}$$
$\text{Therefore all square matrices can be expressed as the sum of a symmetric matrix and skew-symmetric matrix}$

### 69.
$\text{Express } \begin{bmatrix}4&2&-1\\3&5&7\\1&2&-1\end{bmatrix}\text{ as the sum of two matrices of which one is symmetric and other skew symmetric}$
$$A=P+Q$$
$$\text{Where } P=\frac{1}{2}(A+A^T),Q=\frac{1}{2}(A-A^T)$$
$$\text{Let A = }\begin{bmatrix}4&2&-1\\3&5&7\\1&2&-1\end{bmatrix} => A^T=\begin{bmatrix}4&3&1\\2&5&2\\-1&7&-1\end{bmatrix}$$
$$P=\frac{1}{2}(\begin{bmatrix}4&2&-1\\3&5&7\\1&2&-1\end{bmatrix}+ \begin{bmatrix}4&3&1\\2&5&2\\-1&7&-1\end{bmatrix})$$
$$P=\begin{bmatrix}
4 & 2.5 & 0 \\
2.5 & 5 & 4.5 \\
0 & 4.5 & -1
\end{bmatrix}$$
$$Q=\frac{1}{2}(\begin{bmatrix}4&2&-1\\3&5&7\\1&2&-1\end{bmatrix}- \begin{bmatrix}4&3&1\\2&5&2\\-1&7&-1\end{bmatrix})=\begin{bmatrix}
0 & -0.5 & -1 \\
0.5 & 0 & 2.5 \\
1 & -2.5 & 0
\end{bmatrix}$$


$$\begin{bmatrix}4&2&-1\\3&5&7\\1&2&-1\end{bmatrix}=\begin{bmatrix}
4 & 2.5 & 0 \\
2.5 & 5 & 4.5 \\
0 & 4.5 & -1
\end{bmatrix}+\begin{bmatrix}
0 & -0.5 & -1 \\
0.5 & 0 & 2.5 \\
1 & -2.5 & 0
\end{bmatrix}$$
### 70.
$\text{Express } \begin{bmatrix}1&0&-9\\-6&2&7\\3&-5&6\end{bmatrix}\text{ as the sum of two matrices of which one is symmetric and other skew symmetric}$

$$A=P+Q$$
$$\text{Where } P=\frac{1}{2}(A+A^T),Q=\frac{1}{2}(A-A^T)$$
$$\text{Let A = } \begin{bmatrix}1&0&-9\\-6&2&7\\3&-5&6\end{bmatrix}=>A^T=\begin{bmatrix}1&-6&3\\0&2&-5\\-9&7&6\end{bmatrix}$$
$$P=\frac{1}{2}(\begin{bmatrix}1&0&-9\\-6&2&7\\3&-5&6\end{bmatrix}+\begin{bmatrix}1&-6&3\\0&2&-5\\-9&7&6\end{bmatrix})=\begin{bmatrix} 1 & -3 & -3 \\ -3 & 2 & 1 \\ -3 & 1 & 6 \end{bmatrix}$$
$$Q=\frac{1}{2}(\begin{bmatrix}1&0&-9\\-6&2&7\\3&-5&6\end{bmatrix}-\begin{bmatrix}1&-6&3\\0&2&-5\\-9&7&6\end{bmatrix})=\begin{bmatrix} 0 & 3 & -6 \\ -3 & 0 & 6 \\ 6 & -6 & 0 \end{bmatrix}$$

$$\begin{bmatrix}1&0&-9\\-6&2&7\\3&-5&6\end{bmatrix}=\begin{bmatrix} 1 & -3 & -3 \\ -3 & 2 & 1 \\ -3 & 1 & 6 \end{bmatrix}+\begin{bmatrix} 0 & 3 & -6 \\ -3 & 0 & 6 \\ 6 & -6 & 0 \end{bmatrix}$$
### 71.
$\text{If A and B are symmetric matrices of same order , prove that AB + BA is symmetric and AB - BA is a skew-symmetric matrix?}$
$$\text{A and B are symmetric =>} A=A^T,B=B^T$$
$$\text{(2) We have AB=BA}$$
$$\text{Symmetry: } (AB+BA)^T=BA+AB$$
$$(AB+BA)^T=(AB+BA) \text{ which means AB+BA is symmetric}$$
$$\text{Skew symmetry: }(AB-BA)^T=B^TA^T-A^TB^T=>BA-AB=-(AB-BA)$$
$$(AB-BA)^T=-(AB-BA) \text{ which means AB-BA is skew-symmetric}$$
$$\text{Therefore AB + BA is symmetric and AB - BA is a skew-symmetric matrix}$$
### 72. 
$$\text{Prove that the principle diagonal elements of a skew symmetric matrix are all zero}$$
$$\text{We have }a_{ij}=-a_{ji}$$
$$\text{Elements are diagonal only if i=j }$$
$$a_{ii}=-a_{ii}=>2a_{ii}=0=>a_{ii}=0$$
### 73.
$$\text{For the matrix A , prove that }A+A^T\text{ is a symmetric matrix}$$
$${(A+A^T)}^T=A^T+A$$
$$\text{Therefore }A+A^T \text{ is a symmetric matrix}$$
### 74.
$$\text{For the matrix A , prove that }A-A^T\text{ is a skew-symmetric matrix}$$
$${(A-A^T)}^T=A^T-A=-(A-A^T)$$
$$\text{Therefore }A-A^T \text{ is a skew-symmetric matrix}$$
### 75.
$$\text{If B is a skew symmetric matrix, prove that }(ABA^T)\text{ is a skew symmetric matrix}$$
$$\text{We have } B=-B^T$$
$$\text{Show }{(ABA^T)}^T=-(ABA^T)$$
$${(ABA^T)}^T={A^T}^TB^TA^T=A(-B)(A^T)=-(ABA^T)$$
$$\text{Since }{(ABA^T)}^T=-(ABA^T), \text{ Therefore }(ABA^T)\text{ is a skew symmetric matrix}$$
### 76.
$$\text{If A is a 3 x 4 matrix and B is a matrix such that A’B and BA’ are both defined , find the order of B ?}$$
$$\text{For A'B to be defined, column of A' must match row of B} $$
$$\text{Let B have an order of mxn, we know m = 3}$$
$$\text{For BA' to be defined, column of B must match row of A'} $$
$$\text{n=4}$$
$$\text{The order of B is 3x4}$$
### 77.
$\text{Express } \begin{bmatrix}2&-2&-4\\-1&3&4\\1&-2&-3\end{bmatrix}\text{ as the sum of two matrices of which one is symmetric and other skew symmetric}$

$$A=P+Q$$
$$\text{Where } P=\frac{1}{2}(A+A^T),Q=\frac{1}{2}(A-A^T)$$
$$\text{Let A = }\begin{bmatrix}2&-2&-4\\-1&3&4\\1&-2&-3\end{bmatrix}=>A^T=\begin{bmatrix}2&-1&1\\-2&3&-2\\-4&4&-3\end{bmatrix}$$
$$P=\frac{1}{2}(\begin{bmatrix}2&-2&-4\\-1&3&4\\1&-2&-3\end{bmatrix}+\begin{bmatrix}2&-1&1\\-2&3&-2\\-4&4&-3\end{bmatrix})= \begin{bmatrix}
2 & -\frac{3}{2} & -\frac{3}{2} \\
-\frac{3}{2} & 3 & 1 \\
-\frac{3}{2} & 1 & -3
\end{bmatrix}$$

$$Q=\frac{1}{2}(\begin{bmatrix}2&-2&-4\\-1&3&4\\1&-2&-3\end{bmatrix}-\begin{bmatrix}2&-1&1\\-2&3&-2\\-4&4&-3\end{bmatrix})=Q = \begin{bmatrix}
0 & -\frac{1}{2} & -\frac{5}{2} \\
\frac{1}{2} & 0 & 3 \\
\frac{5}{2} & -3 & 0
\end{bmatrix}$$
$$\begin{bmatrix}2&-2&-4\\-1&3&4\\1&-2&-3\end{bmatrix}=\begin{bmatrix}
2 & -\frac{3}{2} & -\frac{3}{2} \\
-\frac{3}{2} & 3 & 1 \\
-\frac{3}{2} & 1 & -3
\end{bmatrix}+\begin{bmatrix}
0 & -\frac{1}{2} & -\frac{5}{2} \\
\frac{1}{2} & 0 & 3 \\
\frac{5}{2} & -3 & 0
\end{bmatrix}$$
### 78.
$$\text{If A = } \begin{bmatrix}1&2&3\end{bmatrix} \text{ Write } AA^T$$
$$\text{We have A=}\begin{bmatrix}1&2&3\end{bmatrix}=>A^T=\begin{bmatrix}1\\2\\3\end{bmatrix}$$
$$AA^T=\begin{bmatrix}1&2&3\end{bmatrix}\begin{bmatrix}1\\2\\3\end{bmatrix}=\begin{bmatrix}14\end{bmatrix}$$
### 79. 
$$\text{Let A = }\begin{bmatrix}1\\0\end{bmatrix} \text{ find }AA^T$$
$$\text{We have } A=\begin{bmatrix}1\\0\end{bmatrix}=>A^T=\begin{bmatrix}1&0\end{bmatrix}$$
$$\text{We have } A=\begin{bmatrix}1\\0\end{bmatrix}\begin{bmatrix}1&0\end{bmatrix}=\begin{bmatrix}1\end{bmatrix}$$
### 80.
$$\text{Name a matrix which is both symmetric as well as skew symmetric}$$
$$\text{Nil matrix } A_{\text{nxn}} = \begin{bmatrix}a_{ij}\end{bmatrix};i=j=0$$
### 81. 
$$\text{If the matrix A = } \begin{bmatrix}0&a&-3\\2&0&-1\\b&1&0\end{bmatrix}\text{ is skew symmetric, find a and b}$$
$$A^T=\begin{bmatrix}0&a&-3\\2&0&-1\\b&1&0\end{bmatrix}^T=\begin{bmatrix}0&2&b\\a&0&1\\-3&-1&0\end{bmatrix}$$
$$-A=\begin{bmatrix}0&-a&3\\-2&0&1\\-b&-1&0\end{bmatrix}$$
$$\begin{bmatrix}0&2&b\\a&0&1\\-3&-1&0\end{bmatrix}=\begin{bmatrix}0&-a&3\\-2&0&1\\-b&-1&0\end{bmatrix}$$
$$\left\{\begin{array}{l} a=2 &\\ b=3 \end{array}\right.$$
# II. Determinants
### 1. 
$$\text{Evaluate the determinant of the following matrices }$$
$$A=\begin{bmatrix}3&-5\\-8&9\end{bmatrix}=>det(A)=-13$$
$$B=\begin{bmatrix}cosx&-sinx\\sinx&cosx\end{bmatrix}=>det(B)=cos^2x+sin^2x=1$$
$$C=\begin{bmatrix}0&sin\alpha&-cos\alpha\\-sin\alpha&0&sin\beta\\-cos\alpha&-sin\beta&0\end{bmatrix}$$
$$=>det(C)=-sin\alpha(cos\alpha sin\beta)-cos\alpha(sin\alpha sin\beta)=-2sin\alpha sin\beta cos\alpha$$
$$D=\begin{bmatrix}1&2&5\\2&3&1\\-1&1&1\end{bmatrix}=>det(D)=(3-1)-2(2+1)+5(2+3)=21$$
### 2. 
$$\text{For what value of x, the matrix} \begin{bmatrix}5-x&x+1\\2&4\end{bmatrix} \text{ is singular}$$
$$\text{A matrix is singular only if the determinant of the matrix is 0}$$
$$\text{Let A = } \begin{bmatrix}5-x&x+1\\2&4\end{bmatrix}$$
$$=>det(A)=20-4x-2x-2=18-6x$$
$$6(3-x)=0=>x=3$$
### 3. 
$$\text{If A = } \begin{bmatrix}1&0&1\\0&1&2\\0&0&4\end{bmatrix}\text{, prove that |3A|=27|A|}$$
$$|A|=4$$
$$|3A|=3(3*12)=108$$
$$|3A|=27|A|=>108=4*27=108 \text{ (True)}$$
### 4. 
$$\text{Find the integral value of x if }det(A)=\begin{bmatrix}x^2&x&1\\0&2&1\\3&1&4\end{bmatrix}=28$$
$$det(A)=x^2(8-1)-x(-3)+1(0-6)=7x^2+3x-6=28$$
$$x=\frac{-3\pm\sqrt{3^2-4(7)(-6)}}{2*7}$$
$$x_1=2,x_2=-\frac{17}{7}$$
$$\text{Since }x_2 \text{ is not an integer } x=2\text{ is the integral value}$$
### 7.
$$\text{Evaluate the determinant } \begin{bmatrix}log_3{512}&log_4{3}\\log_3{8}&log_4{9}\end{bmatrix}$$
$$\text{Let A = } \begin{bmatrix}log_3{512}&log_4{3}\\log_3{8}&log_4{9}\end{bmatrix}$$
$$\begin{bmatrix}log_3{2^9}&log_4{3}\\log_3{2^3}&log_4{3^3}\end{bmatrix}$$

$$\begin{bmatrix}9log_3{2}&log_4{3}\\3log_3{2}&3log_4{3}\end{bmatrix}$$
$$det(A)=9log_32*3log_43-log_43*3log_32$$
$$det(A)=18log_32*2log_43-3log_4*3log_32=15log_32*log_43$$
$$det(A)=15log_32*log_43$$
### 8.
$$\text{What positive value of x that makes the pair of determinants equal } det(\begin{bmatrix}2x&3\\5&x\end{bmatrix}),det(\begin{bmatrix}16&3\\5&2\end{bmatrix})$$
$$2x^2-8=32-8=>x=\sqrt{16}=>x=\pm4$$
### 9.
$$\text{If A is a 3x3 matrix and if |A| = 4 and |B| = 5, find |2AB|}$$
$$|2AB|=2^3|A||B|=8*4*5=160$$
### 10.
$$\text{For any 2x2 matrix A, |A| = 5, find |kA|}$$
$$|kA|=5k^2$$
### 11.
$$\text{If A is a square matrix of order 3 such that |adj A|=100, find |A|}$$
$$|adjA|=|A|^{n-1}$$
$$|A|^{3-1}=100=>A=\sqrt{100}=>A=\pm10$$
### 12.
$$\text{What is the value of }|3I_3|\text{ where } I_3 \text{ is the identity matrix of order 3}$$
$$|3I_3|=3^3*1=9$$
### 13.
$$\text{A square matrix A is of order 3, and has |A| = 5, find |A adj.A|}$$
$$\text{|A adj.A|} = |A|^3=125$$
### 14.
$$\text{Find the minors and cofactors for A =} \begin{bmatrix}1&-3&2\\4&7&8\\8&-3&-1\end{bmatrix}$$
$$M_{a_{11}}=-7+24=17$$
$$M_{a_{12}}=-4-64=-68$$
$$M_{a_{13}}=-12-56=-68$$
$$M_{a_{21}}=3+6=9$$
$$M_{a_{22}}=-1-16=-17$$
$$M_{a_{23}}=-3+24=21$$
$$M_{a_{31}}=-24-14=-38$$
$$M_{a_{32}}=8-8=0$$
$$M_{a_{33}}=7+12=19$$
$$M=\begin{bmatrix}
17 & -68 & -68 \\
9 & -17 & 21 \\
-38 & 0 & 19
\end{bmatrix}.$$
$$C=\begin{bmatrix}
17 & 68 & -68 \\
-9 & -17 & -21 \\
-38 & 0 & 19
\end{bmatrix}.$$
### 15.

### 16. 
$$\text{Write the adjoint of following matrix }\begin{bmatrix}2&-1\\4&3\end{bmatrix}$$
$$\text{Adj.}\begin{bmatrix}2&-1\\4&3\end{bmatrix}=\begin{bmatrix}3&1\\-4&2\end{bmatrix}$$
### 17.
$$\text{If A = } \begin{bmatrix}1&2\\3&4\end{bmatrix}\text{, verify that A(adj.A) = }|A|I_2$$
$$A(adj.A)=\begin{bmatrix}1&2\\3&4\end{bmatrix}\begin{bmatrix}4&-2\\-3&1\end{bmatrix}=\begin{bmatrix}-2&0\\0&-2\end{bmatrix}$$
$$|A|I_2=4-6\begin{bmatrix}1&0\\0&1\end{bmatrix}=\begin{bmatrix}-2&0\\0&-2\end{bmatrix}$$
