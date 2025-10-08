Some cases are too complex to describle with mathmatical formulas, so we need to analyze data points. Here are the tasks: 
1. Fitting a selected model type or types to the data.
2. Choosing the best fitted model. 
3. Making predicitons.
### Relationship Between Model Fitting and Interpolation
Model Fitting involves finding a mathmatical function that best represents the given data. It doesn't necessarily pass through all the data points. Interpolation involves finding a function that exactly passes through all the data points.
### Sources of Error in the Modeling Process
1. Formulation error
   Formulation error presents in all the models when certain variables are negligible or simplifed in the assumption. 
2. Truncation error 
   Truncation error occors when numerical methods used to solve mathmatical problems cause inacurated errors. 
3. Round-off error
   Round-off error happens when infinit digit cannot be represented exactly using finit digits. 
4. Measurement error
   Measurement error is caused by inaccurate data collaction. 

## 3.1 Fitting Models to Data Graphically
Models need as many data points in the model curve. 
The *spacing* of the data points within that interval is also important. 
Accuracy of the data points need to be appraised everytime before fitiing the model. 
![[Pasted image 20250224123855.png|200]]
### Visual Model Fitting with the Original Data
Generally, when more than two data points exist, some points are not lied on a same line. There will be vertical distances between inaccurate points and the line. We call these vertical distances **absolute deviations**. For the best-fitiing line, we aim to minimize the sum of these absolute deviations. However, some large absolute deviations will impact the line a lot. A line that minimizes the largest deviation from any point is an alternative. 

### Transforming the Data
Sometimes the relationships are complex, thus the graphs are difficult to draw. In order to draw simpler graphs, we can put not only *x* ot *y* on the x-axis or y-axis, but also functions or relations about *x* and *y*. This need some more mathematical processes but will come up with simpler results, such as straight lines.  

## 3.2 Analytic Methods of Model Fitting
### Chebyshev Approximation Criterion
Chebyshe Approximation Criterion is used to minimize the largest absolute deviation. 
Given a function $y = f(x)$ and a collection of $n$ data points $(x_i, y_i)$. Minimizes the number
$$
\text{Maximum} 
 \quad |y_i - f(x_i)| \qquad  i = 1,2,...,n
$$
**Redidual** is difference between true value and measured value. Note that rediduals can be positive or negative, but absolute deviations are always positive. 
$$ r = x_i - m_i \qquad r = \text{Redidual}, \ x = \text{True Value}, \ m = \text{Measured Value}$$
For every data point, there is a residual $r_i$ . The largest absolute value among all $r_i$​ is called $r$, and we aim to **minimize** $r$.
The $r$ needs to meet: 
$$
|r_i| \leq r \quad -r \leq r_i \leq r
$$
$|r_i| \leq r$ can be expressed by $r - r_i \leq 0$ and $r + r_i \geq 0$ .  
$$
\begin{aligned}
r - (x_i - m_i) \geq 0 \quad (r - r_i \geq 0) \\
r + (x_i - m_i) \geq 0 \quad (r + r_i \geq 0)
\end{aligned}
$$
The weakness of Chebyshev Approximation Criterion is that it gives more weight to a single point with large deviation. 

### Minimizing the Sum of the Absolute Deviations
Given a function $y = f(x)$ and a collection of $n$ data points $(x_i, y_i)$. Then we want to minimize
$$
\sum_{i=1}^{n} \lvert y_i - f(x_i) \rvert
$$
$R_i = |y_i - f(x)|, i = 1, 2, ..., n$ represent each absolute deviation. We want to minimize by adding together the number $R_i$ .

### Least Squares Criterion
Given a function $y = f(x)$ and a collection of $n$ data points $(x_i, y_i)$. Then we want to minimize
$$
\sum_{i=1}^{n}|y_i - f(x_i)|^2
$$
$R_i = |y_i - f(x)|, i = 1, 2, ..., n$. Consider $R_i$ are scalar components of a deviation vector$\mathbf{R} = R_1 \mathbf{i} + R_2 \mathbf{j} + R_3 \mathbf{k}$. In other word, we want to make vector, $\mathbf R$, as short as possible. 
![[Pasted image 20250227231532.png]]
The formula to calculate this deviation vector is 
$$
|\mathbf R| = \sqrt{R_1^2 + R_2^2 + R_3^2}
$$
In order to minimize $|\mathbf R|$, we can minimize $|\mathbf R|^2$. 

### Relating the Criteria
Combining Chebyshev Approximation Criterion and Least Squares Criterion. 

The absolute deciations according to Chebyshev Approximation Criterion are:
$$c_i = |y_i - f(x_i)|, \quad i = 1,2,...,n$$
Define the largest absolute deviations is $c_{max}$, which we want to minimize. 

The absolute deciations according to Least Squares Criterion are:
$$
d_i = |y_i - f(x_i)|, \quad i = 1,2,...,n
$$
Define the largest absolute deviations is $d_{max}$.
Note: 
$$
d_{max} \leq c_{max}
$$
According to the definition of Least Squares Criterion, the sum of $d_i$ is the smallest, so: 
$$
d_1^2 + d_2^2 +...+ d_n^2 \leq c_1^2 + c_2^2 +...+ c_n^2
$$
Since $c_i < c_{max}$ , therefore, 
$$
d_1^2 + d_2^2 +...+ d_n^2 \leq nc_{max}^2
$$
Isolate $c_{max}$ by following formula: 
$$
c_{max} \geq \sqrt\frac{d_1^2 + d_2^2 +...+ d_n^2}{n}
$$
For ease of discussion, define
$$
D = \sqrt\frac{d_1^2 + d_2^2 +...+ d_n^2}{n}
$$
Thus, 
$$
D \leq c_{max} \leq d_{max}
$$If $|D - d_{max}|$ is too large, Chebyshev Approximation Criterion will be better than Least Squares Criterion. 