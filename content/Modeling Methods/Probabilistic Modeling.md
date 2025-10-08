### Probabilistic Modeling with Discrete 
Markov Chain is a process with following characteristics: 
1. There are the same finite number of states or outcomes that can be occupied at any given time.
2. The states do not overlap and cover all possible outcomes.
3. Next state **only** depends on the present state, called memory lessness. 
4. The sum of the probabilities for transitioning from the present state to the next state is **equal to 1** for each state.
For example, here are two states, State 1 and State 2. If it is State 1 now, the probability of maintaining the present state is $p$, then the probability of changing from State 1 to State 2 is $1-p$. The same applies to State 2. Notice $p_1$ does not necessary equal to $p_2$ .
 ![[Pasted image 20250317103711.png]]