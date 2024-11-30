I understand! Here's how I can format the documentation in a more organized way to make it look better when transferred to MS Word:

---

### **Probability**

1. **What is Probability?**
   
   Probability is a measure of the likelihood of an event occurring. It ranges between 0 and 1:
   - **0**: The event cannot happen.
   - **1**: The event is certain to happen.

   **Key Terms:**
   - **Experiment**: A process that produces an outcome (e.g., tossing a coin).
   - **Outcome**: A possible result of an experiment (e.g., "Heads").
   - **Sample Space (SS)**: The set of all possible outcomes of an experiment.
     - Example: Tossing a coin → SS = {Heads, Tails}.
   - **Event (A)**: A subset of the sample space.
     - Example: Rolling a die and getting an even number → A = {2, 4, 6}.

2. **Types of Probability**

   - **Classical Probability**: Assumes all outcomes are equally likely.
     - Example: Rolling a fair die → P(getting 3) = 1/6.
   - **Empirical Probability**: Based on experiments or observations.
     - Example: A coin is tossed 100 times, and Heads appears 55 times. Then:  
       P(Heads) = Number of Heads / Total Tosses = 55/100 = 0.55.
   - **Subjective Probability**: Based on personal judgment or experience.
     - Example: Predicting a cricket team’s chance of winning.

3. **Basic Rules of Probability**

   - **Addition Rule**:  
     For two events A and B:  
     P(A ∪ B) = P(A) + P(B) − P(A ∩ B).
     - If A and B are mutually exclusive (P(A ∩ B) = 0), then:  
       P(A ∪ B) = P(A) + P(B).
   - **Multiplication Rule**:  
     For two events A and B:  
     P(A ∩ B) = P(A) ⋅ P(B | A).
     - If A and B are independent:  
       P(A ∩ B) = P(A) ⋅ P(B).
   - **Complement Rule**:  
     The probability of an event not happening (Ac):  
     P(A^c) = 1 − P(A).

4. **Conditional Probability**
   
   The probability of event A occurring, given that B has occurred:  
   P(A | B) = P(A ∩ B) / P(B), where P(B) ≠ 0.

   **Example**:  
   If a card is drawn from a deck, what is the probability that it is a King given it is a face card?  
   - Total face cards = 12 (King, Queen, Jack of each suit).  
   - Kings among face cards = 4.  
   P(King | Face Card) = 4/12 = 1/3.

5. **Bayes' Theorem**

   Formula:  
   P(A | B) = (P(B | A) ⋅ P(A)) / P(B).

   **Example**:  
   A medical test has:  
   - P(Positive | Disease) = 0.98,  
   - P(Positive | No Disease) = 0.05,  
   - P(Disease) = 0.01.  
   Find the probability that a person has the disease if they tested positive.  
   P(Disease | Positive) = P(Positive | Disease) ⋅ P(Disease) / P(Positive).

6. **Random Variables**
   
   A random variable is a function that assigns numerical values to outcomes of a random experiment.

   - **Discrete Random Variable**: Takes specific values.
     - Example: Number of Heads in 3 coin tosses (X = 0, 1, 2, 3).
   - **Continuous Random Variable**: Takes any value in a range.
     - Example: Heights of people (X ∈ [150 cm, 200 cm]).

7. **Probability Distribution**

   - **PMF (Probability Mass Function)**:  
     Used for discrete random variables. Gives the probability at specific points.  
     Example: P(X = x).
   - **PDF (Probability Density Function)**:  
     Used for continuous random variables. Represents density, not direct probability.  
     Example: f(x), where P(a ≤ X ≤ b) = ∫(a to b) f(x) dx.

8. **Expectation and Variance**

   - **Mean (Expectation)**:  
     Discrete: E(X) = ∑x ⋅ P(X = x).  
     Continuous: E(X) = ∫(−∞ to ∞) x ⋅ f(x) dx.
   - **Variance**:  
     Measures the spread of a distribution:  
     Var(X) = E(X^2) − [E(X)]^2.

9. **Important Theorems**

   - **Law of Large Numbers**:  
     The average of results from many trials will converge to the expected value.
   - **Central Limit Theorem (CLT)**:  
     The sum (or mean) of many independent random variables tends to follow a normal distribution, even if the original variables are not normally distributed.

10. **Key Probability Distributions**

   - **Binomial Distribution**:  
     Discrete distribution for n trials with success probability p.  
     PMF: P(X = k) = (n choose k) ⋅ p^k ⋅ (1 − p)^(n − k).
   - **Normal Distribution**:  
     Continuous bell-shaped curve.  
     PDF: f(x) = (1 / √(2πσ²)) ⋅ e^−((x − μ)² / 2σ²).
   - **Poisson Distribution**:  
     Models rare events occurring over time or space.  
     PMF: P(X = k) = (λ^k e^−λ) / k!.

---

I hope this format is more readable for your MS Word document! Let me know if you'd like me to adjust anything else.
