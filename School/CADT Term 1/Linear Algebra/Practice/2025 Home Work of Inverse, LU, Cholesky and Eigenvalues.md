# I. Find LU-factorization for the following matrix
### 1. $$\text{Let A = }\begin{bmatrix}2&4&2\\1&1&2\\-1&0&2\end{bmatrix}$$
$$U=A\xrightarrow[R_2:2R_2-R_1]{R_3:2R_3+R_1}=\begin{bmatrix}2&4&2\\0&-2&2\\0&4&6\end{bmatrix}\xrightarrow{R_3:R_3+2R_2}=\begin{bmatrix}2&4&2\\0&-2&2\\0&0&10\end{bmatrix}$$
# II. 
$$det(1)\neq1$$
$$det(\begin{bmatrix}1&2\\2&4\end{bmatrix})=4-4=0$$
# III.
a. Has
b. No
c. No
# VI. 
$$\left\{\begin{array}{l} (1985,227) &\\ (1995,249) &\\(2005,281) \end{array}\right.$$
$$\text{Let z = x-1995}$$
$$\text{We have } P(z) = az^2+bz+c$$
$$\left\{\begin{array}{l} \text{When x=1985 }(-10,227) &\\ \text{When x=1995 }(0,249) &\\\text{When x=2005 }(10,281) \end{array}\right.$$
$$\left\{\begin{array}{l} a(-10)^2-10b+c=227 &\\ c=249 &\\a(10)^2+10b+c=281\end{array}\right.$$
$$\left\{\begin{array}{l} a(-10)^2-10b=227-249 &\\a(10)^2+10b+c=281-249\end{array}\right.$$
$$\left\{\begin{array}{l} 100a-10b=-22 &\\100a+10b=32\end{array}\right.$$
$$a=\frac{5}{100},b=\frac{27}{10},c=249$$
$$P(z)=\frac{1}{20}z^2+\frac{27}{10}z+249$$
$$\text{But z=x-1995 }$$
$$P(x)=\frac{1}{20}(x-1995)^2+\frac{27}{10}(x-1995)+249$$
$$\text{If x = 2025 } P(2025)=\frac{1}{20}(30)^2+\frac{27}{10}(30)+249$$
$$P(2025)=375$$
# VII.
$$\text{Calculation }det(A), adj(A), A^-1,det(A^{-1}),det(5A) \text{ of matrix } A=\begin{bmatrix}2&0&1\\-3&3&-1\\-3&1&-1\end{bmatrix}$$
$$M=\begin{bmatrix}-2&0&6\\-1&1&2\\-3&1&6\end{bmatrix},C=\begin{bmatrix}2&0&6\\1&1&-2\\-3&-1&6\end{bmatrix}$$
$$det(A)=(2)(-2)+(0)(0)+(1)(6)=2$$
$$adj.A=C^T=\begin{bmatrix}2&1&-3\\0&1&-1\\6&-2&6\end{bmatrix}$$
$$A^{-1}=\frac{1}{2}\begin{bmatrix}2&1&-3\\0&1&-1\\6&-2&6\end{bmatrix}=\begin{bmatrix}1&\frac{1}{2}&-\frac{3}{2}\\0&\frac{1}{2}&-\frac{1}{2}\\3&-1&3\end{bmatrix}$$
$$det(A^{-1})=\frac{1}{det(A)}=\frac{1}{2}$$
$$det(5A)=5^3det(A)=125*2=250$$
# VIII.
$$\text{Solve the system of linear equation by LU Decomposition } \left\{\begin{array}{l} x_1+2x_2+3x_3=1 &\\ 2x_1+3x_2+4x_3=3 &\\ x_1+2x_2+x_3=3 \end{array}\right.$$
$$\begin{bmatrix}1&2&3\\2&3&4\\1&2&1\end{bmatrix}\begin{bmatrix}x_1\\x_2\\x_3\end{bmatrix}=\begin{bmatrix}1\\3\\3\end{bmatrix}$$
$$\text{Let A = } \begin{bmatrix}1&2&3\\2&3&4\\1&2&1\end{bmatrix}$$
$$U=A\xrightarrow[R_3:R_3-R_1]{R_2:R_2-2R_1}\begin{bmatrix}1&2&3\\0&-1&-2\\0&0&-2\end{bmatrix}$$
$$L=\begin{bmatrix}1&0&0\\2&1&0\\1&0&1\end{bmatrix}$$
$$\text{Solve for Ly=B , where y = } \begin{bmatrix}y_1\\y_2\\y_3\end{bmatrix}$$
$$\begin{bmatrix}1&0&0\\2&1&0\\1&0&1\end{bmatrix}\begin{bmatrix}y_1\\y_2\\y_3\end{bmatrix}=\begin{bmatrix}1\\3\\3\end{bmatrix}$$

$$\left\{\begin{array}{l} y_1=1&\\y_2=3-2=1&\\y_3=3-1=2\end{array}\right.$$
$$Ux=y$$
$$\begin{bmatrix}1&2&3\\0&-1&-2\\0&0&-2\end{bmatrix}\begin{bmatrix}x_1\\x_2\\x_3\end{bmatrix}=\begin{bmatrix}1\\1\\2\end{bmatrix}$$
$$\left\{\begin{array}{l} x_3=-1&\\x_2=1&\\x_1=2\end{array}\right.$$
$$x=\begin{bmatrix}-1\\1\\2\end{bmatrix}$$
# IX. $$\text{Consider A = } \begin{bmatrix}1&6&2\\2&12&5\\-1&-3&-1\end{bmatrix}$$
##### $$\text{a. Show that A doesn't have an LU decomposition}$$
$$det(\begin{bmatrix}1&6\\2&12\end{bmatrix})=0$$
##### $$\text{b. Re-order the rows of A and find an LU decomposition of the new matrix}$$
$$PA=\begin{bmatrix}1&0&0\\0&1&0\\0&0&1\end{bmatrix}\begin{bmatrix}1&6&2\\2&12&5\\-1&-3&-1\end{bmatrix}$$
$$P_{23}A=\begin{bmatrix}1&0&0\\0&0&1\\0&1&0\end{bmatrix}\begin{bmatrix}1&6&2\\-1&-3&-1\\2&12&5\end{bmatrix}$$
$$U=A\xrightarrow[R_3:R_3-2R_1]{R_2:R_2+R_1}\begin{bmatrix}1&6&2\\0&3&1\\0&0&1\end{bmatrix}$$
$$L=\begin{bmatrix}1&0&0\\-1&1&0\\2&0&1\end{bmatrix}$$
$$PA=\begin{bmatrix}1&0&0\\-1&1&0\\2&0&1\end{bmatrix}\begin{bmatrix}1&6&2\\0&3&1\\0&0&1\end{bmatrix}$$
##### $$\text{Hence solve } \left\{\begin{array}{l} x_1+6x_2+2x_3=9&\\2x_1+12x_2+5x_3=-4&\\-x_1-3x_2-x_3=17&\\\end{array}\right.$$
$$Ax=B$$
$$\begin{bmatrix}1&6&2\\2&12&5\\-1&-3&-1\end{bmatrix}\begin{bmatrix}x_1\\x_2\\x_3\end{bmatrix}=\begin{bmatrix}9\\17\\-4\end{bmatrix}$$
$$\text{Solve for Ly=B where, } y=\begin{bmatrix}y_1\\y_2\\y_3\end{bmatrix}$$
$$\begin{bmatrix}1&0&0\\-1&1&0\\2&0&1\end{bmatrix}\begin{bmatrix}y_1\\y_2\\y_3\end{bmatrix}=\begin{bmatrix}9\\17\\-4\end{bmatrix}$$
$$\left\{\begin{array}{l} y_1=9&\\y_2=26&\\y_3=-22\end{array}\right.$$
$$Ux=y$$
$$\begin{bmatrix}1&6&2\\0&3&1\\0&0&1\end{bmatrix}\begin{bmatrix}x_1\\x_2\\x_3\end{bmatrix}=\begin{bmatrix}9\\26\\-22\end{bmatrix}$$

$$x_1=-43,x_2=16,x_3=-22$$
### X$$\text{Find Cholesky Decomposition of Matrices below }$$
##### 1. $$A=\begin{bmatrix}16&20&-12\\20&29&-5\\-12&-5&35\end{bmatrix}$$
$$\text{By Cholesky Decomposition } A=LL^T$$
$$A=LL^T\rightarrow \begin{bmatrix}16&20&-12\\20&29&-5\\-12&-5&35\end{bmatrix}=\begin{bmatrix}l_{11}&0&0\\l_{21}&l_{22}&0\\l_{31}&l_{32}&l_{33}\end{bmatrix}\begin{bmatrix}l_{11}&l_{21}&l_{31}\\0&l_{22}&l_{32}\\0&0&l_{33}\end{bmatrix}=
\begin{bmatrix}l_{11}^2&l_{11}l_{21}&l_{11}l_{31}\\
l_{11}l_{21}&l_{11}^2+l_{22}^2&l_{21}l_{31}+l_{22}l_{32}\\
l_{11}l_{31}&l_{21}l_{31}+l_{22}l_{32}&l_{11}^2+l_{22}^2+l_{33}^2\end{bmatrix}$$
$$L = \begin{bmatrix}
4 & 0 & 0 \\
5 & 2 & 0 \\
-3 & 5 & 1
\end{bmatrix},L^T = \begin{bmatrix}
4 & 5 & -3 \\
0 & 2 & 5 \\
0 & 5 & 1
\end{bmatrix}$$
##### 2. $$A=\begin{bmatrix}4&4&8\\4&13&2\\8&2&56\end{bmatrix}$$
$$\text{By Cholesky Decomposition } A=LL^T$$
$$A=LL^T\rightarrow\begin{bmatrix}4&4&8\\4&13&2\\8&2&56\end{bmatrix}=
\begin{bmatrix}l_{11}^2&l_{11}l_{21}&l_{11}l_{31}\\
l_{11}l_{21}&l_{11}^2+l_{22}^2&l_{21}l_{31}+l_{22}l_{32}\\
l_{11}l_{31}&l_{21}l_{31}+l_{22}l_{32}&l_{11}^2+l_{22}^2+l_{33}^2\end{bmatrix}$$
$$L = \begin{bmatrix}
2 & 0 & 0 \\
2 & 3 & 0 \\
4 & -2 & 6
\end{bmatrix},L^T = \begin{bmatrix}
2 & 2 & 4 \\
0 & 3 & -2 \\
0 & 0 & 6
\end{bmatrix}$$

##### 3. $$A=\begin{bmatrix}9&3&6\\3&2&0\\6&0&12\end{bmatrix}$$$$\text{By Cholesky Decomposition } A=LL^T$$$$A=LL^T\rightarrow\begin{bmatrix}9&3&6\\3&2&0\\6&0&12\end{bmatrix}=
\begin{bmatrix}l_{11}^2&l_{11}l_{21}&l_{11}l_{31}\\
l_{11}l_{21}&l_{11}^2+l_{22}^2&l_{21}l_{31}+l_{22}l_{32}\\
l_{11}l_{31}&l_{21}l_{31}+l_{22}l_{32}&l_{11}^2+l_{22}^2+l_{33}^2\end{bmatrix}$$
$$L = \begin{bmatrix}
3 & 0 & 0 \\
1 & 1 & 0 \\
2 & -2 & 2
\end{bmatrix},L^T = \begin{bmatrix}
3 & 1 & 2 \\
0 & 1 & -2 \\
0 & 0 & 2
\end{bmatrix}$$


### XI. $$\text{Find Eigenvalues and Eigenvectors of Matrices}$$
##### 1. $$\text{A = } \begin{bmatrix}2&3\\4&10\end{bmatrix}$$
$$det(A-\lambda I)=0$$
$$A-\lambda I =\begin{bmatrix}2-\lambda&3\\4&10-\lambda\end{bmatrix}$$
$$det(A-\lambda I)=20-2\lambda-10\lambda+\lambda^2-12=0$$
$$\lambda^2-12\lambda+8=0$$
$$\lambda=\frac{12\pm\sqrt{144-32}}{2}=6\pm2\sqrt7$$
$$\text{Solve }(A-\lambda I )v=0$$
$$\text{If } \lambda_1 = 6+2\sqrt7$$
$$\begin{bmatrix}2&3\\4&10\end{bmatrix}-\begin{bmatrix}6+2\sqrt7&0\\0&6+2\sqrt7\end{bmatrix}$$
$$\begin{bmatrix}-4-2\sqrt7&3\\4&4-2\sqrt7\end{bmatrix}\begin{bmatrix}v_1\\v_2\end{bmatrix}=\begin{bmatrix}0\\0\end{bmatrix}$$
$$(-4-2\sqrt7)v_1+3v_2=0$$
$$v_2=\frac{4+2\sqrt7}{3}v_1$$
$$v_1=\begin{bmatrix}1\\\frac{4+2\sqrt7}{3}\end{bmatrix}$$
$$\lambda_2=6-2\sqrt7$$
$$\begin{bmatrix}2&3\\4&10\end{bmatrix}-\begin{bmatrix}6-2\sqrt7&0\\0&6-2\sqrt7\end{bmatrix}$$
$$\begin{bmatrix}-4+2\sqrt7&3\\4&4+2\sqrt7\end{bmatrix}\begin{bmatrix}v_1\\v_2\end{bmatrix}=\begin{bmatrix}0\\0\end{bmatrix}$$
$$(-4+2\sqrt7)v_1+3v_2=0$$
$$v_2=\frac{4-2\sqrt7}{3}v_1$$
$$v_1=\begin{bmatrix}1\\\frac{4-2\sqrt7}{3}\end{bmatrix}$$

$$  \lambda_1 = 6 + 2\sqrt{7}, \quad \lambda_2 = 6 - 2\sqrt{7}

$$$$
  \mathbf{v}_1 = \begin{bmatrix}1\\\frac{4 + 2\sqrt{7}}{3}\end{bmatrix}, \mathbf{v}_2 = \begin{bmatrix}1\\\frac{4 - 2\sqrt{7}}{3}\end{bmatrix}$$
  ##### 2.
  $$A=\begin{bmatrix}1&1&1\\-1&-3&-3\\2&4&4\end{bmatrix}$$
  $$det(A-\lambda I)=0$$
  $$A-\lambda I=\begin{bmatrix}1-\lambda&1&1\\-1&-3-\lambda&-3\\2&4&4-\lambda\end{bmatrix}$$
  $$det(A-\lambda I)=0$$$$(1-\lambda)(-3-\lambda)(4-\lambda)+1(-3)(2)+1(-1)(4)-2(-3-\lambda)(1)-(4)(-3)(1-\lambda)-(4-\lambda)(-1)(1)$$
  $$(-1)(4-\lambda-4\lambda+\lambda^2)(3+\lambda)-6-4+(6+2\lambda)-12(1-\lambda)+4-\lambda$$
$$-\lambda^3+2\lambda^2$$
$$\lambda^2(-\lambda+2)=0$$
$$\left\{\begin{array}{l} \lambda_{1}=0 &\\ \lambda_{2}=2 \end{array}\right.$$
$$(A-\lambda I)v=0$$
$$\text{If } \lambda_1=0$$
$$\begin{bmatrix}1&1&1\\-1&-3&-3\\2&4&4\end{bmatrix}\begin{bmatrix}x_1\\x_2\\x_3\end{bmatrix}=\begin{bmatrix}\end{bmatrix}$$