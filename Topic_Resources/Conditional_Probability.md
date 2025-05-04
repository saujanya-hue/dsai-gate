# 📘 Probability & Statistics – Topic-Wise Guide

## 🎯 Conditional Probability

### 🔑 Key Concepts

* Marginal, Joint, and Conditional Probability
* Bayes’ Theorem
* Conditional Expectation and Variance
* Conditional Probability Density Function

### 📚 Resources

* **Slides:** [CMU Probability Basics](https://www.cs.cmu.edu/~16385/s17/Slides/8.1_Probability_Basics.pdf) [Clarity 5⭐]
* University of Connecticut – Probability Textbook Chapter
Comprehensive coverage of conditional probability with examples. 
https://probability.oer.math.uconn.edu/wp-content/uploads/sites/2187/2018/01/prob3160ch4.pdf
* [Conditional Probability Video Lecture](https://www.youtube.com/watch?v=IT_NpA1PpOg&ab_channel=AmitGoyal)
* **Cheatsheet:** Comprehensive Probability and Statistics cheatsheet by Joe Blitzstein (Harvard).
* **Notes & Examples:** Detailed explanations and practice problems available in the [Probability-Statistics-Readme.md](https://github.com/DS-AI-GATE/dsai-gate/blob/main/Probability-Statistics-Readme.md).



### Questions
* **Conditional Expectations** : https://davidrosenberg.github.io/mlcourse/Notes/conditional-expectations.pdf
* [Gate 2025 Q11 Solution](https://www.youtube.com/watch?v=pDxBJhav3TA&ab_channel=AmitGoyal)
* [ Constant Conditional Expectation function implies zero covariance. ](https://www.youtube.com/watch?v=xO9WJc-enIU&ab_channel=AmitGoyal)


## 📝 Practice Questions

### **Question 1:**

If $P(A) = 0.3$, $P(B) = 0.7$, and $P(A \cap B) = 0.1$, find $P(A|B)$ and $P(B|A)$.([GeeksforGeeks][1])

**Solution:**

* $P(A|B) = \frac{P(A \cap B)}{P(B)} = \frac{0.1}{0.7} \approx 0.143$
* $P(B|A) = \frac{P(A \cap B)}{P(A)} = \frac{0.1}{0.3} \approx 0.333$

---

### **Question 2:**

In a survey, 60% read Hindi newspapers, 40% read English newspapers, and 20% read both. If a person is known to read Hindi newspapers, what is the probability that they also read English newspapers?([BYJU'S][2])

**Solution:**

* $P(\text{English}|\text{Hindi}) = \frac{P(\text{Hindi} \cap \text{English})}{P(\text{Hindi})} = \frac{0.2}{0.6} \approx 0.333$

---

### **Question 3:**

A fair coin is tossed twice. Let event E be "both head and tail appear," and event F be "at most one head appears." Find $P(E \cap F)$ and $P(F|E)$.([BYJU'S][2])

**Solution:**

* Sample space: {HH, HT, TH, TT}
* E = {HT, TH}, F = {TT, HT, TH}
* $E \cap F = \{HT, TH\}$
* $P(E \cap F) = \frac{2}{4} = 0.5$
* $P(E) = \frac{2}{4} = 0.5$
* $P(F|E) = \frac{P(E \cap F)}{P(E)} = \frac{0.5}{0.5} = 1$([GeeksforGeeks][1])

---

### **Question 4:**

A coin is tossed three times. Let event C be "head on the first toss," and event D be "tail on the second toss." Find $P(C|D)$.

**Solution:**

* Sample space: {HHH, HHT, HTH, HTT, THH, THT, TTH, TTT}
* C = {HHH, HHT, HTH, HTT}, D = {HTH, HTT, TTH, TTT}
* $C \cap D = \{HTH, HTT\}$
* $P(C \cap D) = \frac{2}{8} = 0.25$
* $P(D) = \frac{4}{8} = 0.5$
* $P(C|D) = \frac{P(C \cap D)}{P(D)} = \frac{0.25}{0.5} = 0.5$([GeeksforGeeks][1])

---

### **Question 5:**

In a rainy season, it rains 70% of the days. If it rains, the chance that a village fair will make a loss is 80%. If it doesn't rain, the chance of a loss is 10%. If the fair did not make a loss on a given day, what is the probability that it did not rain that day?([Testbook][3])

**Solution:**
Let:

* $R$: It rains
* $L$: Fair makes a loss([Testbook][3])

Given:

* $P(R) = 0.7$, $P(\neg R) = 0.3$
* $P(L|R) = 0.8$, $P(L|\neg R) = 0.1$

We need to find $P(\neg R|\neg L)$. Using Bayes' Theorem:

$P(\neg R|\neg L) = \frac{P(\neg L|\neg R) \cdot P(\neg R)}{P(\neg L)}$

First, compute $P(\neg L)$:

$P(\neg L) = P(\neg L|R) \cdot P(R) + P(\neg L|\neg R) \cdot P(\neg R)$

$= (1 - 0.8) \cdot 0.7 + (1 - 0.1) \cdot 0.3 = 0.14 + 0.27 = 0.41$

Now, compute $P(\neg R|\neg L)$:

$P(\neg R|\neg L) = \frac{0.9 \cdot 0.3}{0.41} \approx \frac{0.27}{0.41} \approx 0.6585$

---

For more practice questions and detailed solutions, consider exploring the following resources:

* [BYJU'S: Conditional Probability Questions with Solutions](https://byjus.com/maths/conditional-probability-questions/)
* [GeeksforGeeks: Conditional Probability Practice Question](https://www.geeksforgeeks.org/conditional-probability-practice-question/)
* [Khan Academy: Calculating Conditional Probability](https://www.khanacademy.org/math/ap-statistics/probability-ap/stats-conditional-probability/e/calculating-conditional-probability)

Feel free to reach out if you need further assistance or resources on other topics!

[1]: https://www.geeksforgeeks.org/conditional-probability-practice-question/?utm_source=chatgpt.com "Conditional Probability Practice Question | GeeksforGeeks"
[2]: https://byjus.com/maths/conditional-probability-questions/?utm_source=chatgpt.com "Conditional Probability Questions with Solutions - BYJU'S"
[3]: https://testbook.com/objective-questions/mcq-on-conditional-probability--5eea6a0a39140f30f369dc5b?utm_source=chatgpt.com "Conditional Probability MCQ Quiz - Objective Question with Answer ..."


