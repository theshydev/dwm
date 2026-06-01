# dwm

Given:

Total observations = **10**
Play = Yes → **6**
Play = No → **4**

Given **Sunny**:

Among **Yes** → Sunny = **4**
Among **No** → Sunny = **3**

Need Naïve Bayes.

Formula:
P(C|X) \propto P(X|C)P(C)

### Step 1: Prior probabilities

[
P(Yes)=\frac{6}{10}=0.6
]

[
P(No)=\frac{4}{10}=0.4
]

---

### Step 2: Likelihood probabilities

[
P(Sunny|Yes)=\frac{4}{6}
]

[
P(Sunny|No)=\frac{3}{4}
]

---

### Step 3: Calculate posterior scores

For **Play = Yes**

[
P(Yes|Sunny)\propto P(Sunny|Yes)\times P(Yes)
]

[
=\frac{4}{6}\times \frac{6}{10}
]

[
=\frac{4}{10}=0.4
]

For **Play = No**

[
P(No|Sunny)\propto P(Sunny|No)\times P(No)
]

[
=\frac{3}{4}\times \frac{4}{10}
]

[
=\frac{3}{10}=0.3
]

---

### Decision:

Since

[
0.4 > 0.3
]

**Predicted Class = Play = YES**

### 8-marks exam format:

**Definition:**
Naïve Bayes is a probabilistic classification algorithm based on Bayes theorem assuming feature independence.

**Formula:**
[
P(C|X)=P(X|C)\times P(C)
]

**Calculation:**
(P(Yes)=6/10) , (P(No)=4/10)

(P(Sunny|Yes)=4/6)

(P(Sunny|No)=3/4)

Yes score = **0.4**

No score = **0.3**

**Conclusion:**
Since **0.4 > 0.3**, the model predicts **“Play = Yes”**.
