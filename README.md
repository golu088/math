# math
Here’s a structured format for your documentation. You can easily copy it into a Microsoft Word document and format it as per your preference for better clarity and presentation:

---

# **Probability and Stochastic Processes**

## **Unit I: Probability**

### **1. What is Probability?**

Probability is a measure of the likelihood of an event occurring, ranging from 0 to 1:
- **0**: The event cannot happen.
- **1**: The event is certain to happen.

#### **Key Terms:**
- **Experiment**: A process that produces an outcome (e.g., tossing a coin).
- **Outcome**: A possible result of an experiment (e.g., "Heads").
- **Sample Space (SS)**: The set of all possible outcomes of an experiment.
    - Example: Tossing a coin → \( S = \{\text{Heads}, \text{Tails}\} \).
- **Event (A)**: A subset of the sample space.
    - Example: Rolling a die and getting an even number → \( A = \{2, 4, 6\} \).

---

### **2. Types of Probability**

1. **Classical Probability**: Assumes all outcomes are equally likely.
    - Example: Rolling a fair die → \( P(\text{getting 3}) = \frac{1}{6} \).
2. **Empirical Probability**: Based on experiments or observations.
    - Example: A coin is tossed 100 times, and Heads appears 55 times. Then:  
      \( P(\text{Heads}) = \frac{55}{100} = 0.55 \).
3. **Subjective Probability**: Based on personal judgment or experience.
    - Example: Predicting a cricket team’s chance of winning.

---

### **3. Basic Rules of Probability**

1. **Addition Rule**:  
   For two events A and B:  
   \( P(A \cup B) = P(A) + P(B) - P(A \cap B) \).
   - If A and B are mutually exclusive (\( P(A \cap B) = 0 \)):  
   \( P(A \cup B) = P(A) + P(B) \).
   
2. **Multiplication Rule**:  
   For two events A and B:  
   \( P(A \cap B) = P(A) \cdot P(B|A) \).
   - If A and B are independent:  
   \( P(A \cap B) = P(A) \cdot P(B) \).

3. **Complement Rule**:  
   The probability of an event not happening (\( A^c \)):  
   \( P(A^c) = 1 - P(A) \).

---

### **4. Conditional Probability**

Definition: The probability of event A occurring, given that B has occurred:  
\( P(A|B) = \frac{P(A \cap B)}{P(B)} \), where \( P(B) \neq 0 \).

Example:  
If a card is drawn from a deck, what is the probability that it is a King given that it is a face card?
- Total face cards = 12 (King, Queen, Jack of each suit).
- Kings among face cards = 4.

\( P(\text{King | Face Card}) = \frac{4}{12} = \frac{1}{3} \).

---

### **5. Bayes’ Theorem**

Formula:  
\( P(A|B) = \frac{P(B|A) P(A)}{P(B)} \).

Application:  
Used when we know the reverse probability \( P(B|A) \) and want to find \( P(A|B) \).

Example:  
A medical test has:  
- \( P(\text{Positive | Disease}) = 0.98 \),  
- \( P(\text{Positive | No Disease}) = 0.05 \),  
- \( P(\text{Disease}) = 0.01 \).

Find the probability that a person has the disease if they tested positive:  
\( P(\text{Disease | Positive}) = \frac{P(\text{Positive | Disease}) \cdot P(\text{Disease})}{P(\text{Positive})} \).

---

### **6. Random Variables**

A random variable is a function that assigns numerical values to outcomes of a random experiment.

1. **Discrete Random Variable**:  
   Takes specific values.  
   Example: Number of Heads in 3 coin tosses \( X = \{0, 1, 2, 3\} \).
   
2. **Continuous Random Variable**:  
   Takes any value in a range.  
   Example: Heights of people \( X \in [150 \text{cm}, 200 \text{cm}] \).

---

### **7. Probability Distribution**

#### **Difference Between PMF and PDF:**
- **PMF**: Used for discrete random variables. Gives the probability at specific points.  
  Example: \( P(X = x) \).
  
- **PDF**: Used for continuous random variables. Represents density, not direct probability.  
  Example: \( f(x) \), where \( P(a \leq X \leq b) = \int_a^b f(x) \, dx \).

---

### **8. Expectation and Variance**

1. **Mean (Expectation)**:
    - Discrete: \( E(X) = \sum_x x \cdot P(X=x) \).
    - Continuous: \( E(X) = \int_{-\infty}^{\infty} x \cdot f(x) \, dx \).

2. **Variance**:  
   Measures the spread of a distribution:  
   \( \text{Var}(X) = E(X^2) - [E(X)]^2 \).

---

### **9. Important Theorems**

1. **Law of Large Numbers**:  
   The average of results from many trials will converge to the expected value.

2. **Central Limit Theorem (CLT)**:  
   The sum (or mean) of many independent random variables tends to follow a normal distribution, even if the original variables are not normally distributed.

---

### **10. Key Probability Distributions**

1. **Binomial Distribution**:  
   Discrete distribution for \( n \) trials with success probability \( p \).  
   PMF:  
   \( P(X = k) = \binom{n}{k} p^k (1 - p)^{n - k} \).
   
2. **Normal Distribution**:  
   Continuous bell-shaped curve.  
   PDF:  
   \( f(x) = \frac{1}{\sqrt{2 \pi \sigma^2}} e^{-\frac{(x - \mu)^2}{2 \sigma^2}} \).

3. **Poisson Distribution**:  
   Models rare events occurring over time or space.  
   PMF:  
   \( P(X = k) = \frac{\lambda^k e^{-\lambda}}{k!} \).

---

## **Unit II: Stochastic Processes**

### **1. Poisson Process**

A Poisson process is a stochastic process modeling events occurring randomly over time at a constant average rate.

#### **Poisson Process Formula:**

For the number of events \( X(t) \) that have occurred by time \( t \), the probability of exactly \( k \) events is given by the Poisson distribution:  
\( P(X(t) = k) = \frac{(\lambda t)^k e^{-\lambda t}}{k!} \),  
Where:  
- \( \lambda \) = average rate of events per unit time.  
- \( t \) = time period.  
- \( k \) = number of events.

---

### **2. Discrete-Time Markov Chains (DTMC)**

A DTMC is a stochastic process where the future state depends only on the current state and not on previous states.

#### **Transition Probability Matrix:**

For two states, the transition matrix might look like this:  
\( P = \begin{bmatrix} P(S1 \to S1) & P(S1 \to S2) \\ P(S2 \to S1) & P(S2 \to S2) \end{bmatrix} \).

---

### **3. Continuous-Time Markov Process**

The system transitions randomly, with rates (rather than probabilities), between states.

#### **Example: Birth and Death Process**  
- Birth rate: \( \lambda \)  
- Death rate: \( \mu \)

---

### **4. Hidden Markov Model (HMM)**

An HMM is a Markov chain where the system’s state is hidden, but observable outputs provide information about the state.

#### **Example: Weather and Umbrella Model**  
- Hidden states: Sunny or Rainy.  
- Observations: Whether people carry umbrellas or not.

---

### **Practice Questions for Viva:**

1. **Poisson Process**: A store receives 5 customers per hour on average. What’s the probability of getting exactly 3 customers in the next hour?
2. **DTMC**: Given the transition matrix for a weather model:  
   \( P = \begin{bmatrix} 0.9 & 0.1 \\ 0.2 & 0.8 \end{bmatrix} \),  
   What’s the probability of it being sunny two days from now if it’s sunny today?
3. **Birth-Death Process**: In a population model with a birth rate of 2 and a death rate of 1, describe how the population changes over time.
4. **HMM**:

 Given the weather system with observations of whether an umbrella is carried, explain how HMM helps predict the weather.

---

Let me know if you need further details or if you'd like to modify anything in the document.
