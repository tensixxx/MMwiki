### Monte Carlo Simulation
Monte Carlo Simulation is a type of **probabilistic** model. 
**probabilistic**: Processes with randomness and uncertainty involved. Same input may have different output. 
**deterministic**: Processes with no randomness and uncertainty involved. Same input always has same output. 
### Simulating Deterministic Behavior: Area Under a Curve
In the graph, $y = f(x)$, where $0 \leq f(x) \leq M$ and $a \leq x \leq b$ . Now we select a random point $P (x,y)$ in the rectangle. Create two counters, one to count the total points and the other to count the points in the region below the curve. 
![[Pasted image 20250316165603.png]]
The formula to calculate the approximate value for the area below the curve is: 
$$
\text{area under curve} \approx \frac{\text{number of points counted below curve}}{\text{total number of random points}} \: \cdot \ \text{area of rectangle}
$$
This method needs a large number of trails. In general, to cut the expected error in half, four times more experiments are needed. 

### Volume Under a Surface
The method we use to approximate the volume is similar to the method we use to find the area under a curve. 
Here is the formula: 
$$
\text{volume of object to be measured} \approx \frac{\text{number of points in the object to be measured}}{\text{total number of points}} \cdot \ {\text{total volume}}
$$
