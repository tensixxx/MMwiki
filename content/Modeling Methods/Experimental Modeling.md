### One-Term Models
A  **One-Term Model**  describle the quantity changes over time using a single mathmatical term or expression. These models follow **differential equation** of the form: 
$$
\frac{dx}{dt} = f(x)
$$
where $x$ is the variable, $t$ represents time, and $\frac{dx}{dt}$ is the rate of change. 
### High-Order Polynomial Models
In some cases, models with more than one term will be considered, especially when a data set has asymptote(s). Thus, High-Order Polynomial models will be considered. 

If there are $N$ data points, the highest order that can perfectly fit all the data points is $N - 1$. 
### Advantages and Disadvantages of High-Order Polynomials
High-Order Polynomials can approximate all data points, making future integral and derivative analyses more convenient. 

On the other hand, consider a situation where data points form a positively sloped straight line, except for the last point, which is below the line. If a linear approximation is applied, the end of the line will continue to increase. However, if the high-order polynomial, such as quadrartic function, is used, the trend at the end may be decreasing. 