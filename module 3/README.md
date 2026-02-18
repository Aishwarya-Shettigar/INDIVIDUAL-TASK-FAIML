# Bayes Theorem in Real Life – Credit Card Fraud Detection

## 1.Introduction

Bayes Theorem is a statistical method used to calculate conditional probability. It helps in updating the probability of an event when new evidence is available.
Bayes Theorem is widely used in classification problems such as:

 - Fraud detection
 - Risk analysis
 - Recommendation systems
 - Predictive modeling

## 2.Bayes Theorem Formula


<img width="316" height="96" alt="Screenshot 2026-02-18 161042" src="https://github.com/user-attachments/assets/410f4820-ac73-4cea-9061-9af1d882a6d4" />

​
#### Where:

 - P(A) → Prior Probability
 - P(B|A) → Likelihood
 - P(B) → Evidence
 - P(A|B) → Posterior Probability

## 3.Real-World Scenario: Credit Card Fraud Detection

Banks use AI systems to detect fraudulent transactions in real time.
For example, companies like Visa Inc. use machine learning models to identify suspicious activities.
Suppose the system checks whether a transaction is fraudulent based on a suspicious pattern (such as unusual location or large amount).

## 4.Given Data (Assumed Example)

#### Suppose:

 - 2% of all transactions are fraudulent
   → P(Fraud) = 0.02

- 98% of transactions are genuine
  → P(Not Fraud) = 0.98

- The AI system correctly detects fraud 95% of the time
  → P(Alert | Fraud) = 0.95

- The system wrongly flags 5% of genuine transactions
  → P(Alert | Not Fraud) = 0.05

We need to calculate:

P(Fraud∣Alert)

That means:If the system gives an alert, what is the probability that the transaction is actually fraud.

## 5️.Step-by-Step Calculation
Step 1: Calculate P(Alert)

 **P(Alert) = P(Alert∣Fraud) P(Fraud) + P(Alert∣NotFraud) P(NotFraud)**

 Substitute values:
  =(0.95×0.02)+(0.05×0.98)
  =0.019+0.049
  =0.068

Step 2: Apply Bayes Theorem

<img width="536" height="88" alt="Screenshot 2026-02-18 162024" src="https://github.com/user-attachments/assets/df794093-6af4-4b01-ba17-ff77d183ec57" />

 =(0.95×0.02)/0.068
 =0.019/0.068
 =0.279

## 6.Final Answer

 **P(Fraud∣Alert)** =0.279=27.9%
 
## 7.Interpretation

Even though the system is 95% accurate in detecting fraud,if an alert is raised, there is only 27.9% probability that the transaction is actually fraudulent.

This happens because fraud transactions are rare (only 2%).

This shows the importance of prior probability in decision-making.

## 8.Conclusion

Bayes Theorem is a powerful tool in AI and Machine Learning for updating probabilities based on new evidence.

In fraud detection systems, it helps determine the actual probability of fraud when a suspicious alert is generated.

Thus, Bayes Theorem plays a critical role in intelligent decision-making systems.
​

