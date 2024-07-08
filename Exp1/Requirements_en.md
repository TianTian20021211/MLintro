### Introduction to Machine Learning - First Experiment

Spring 2024

---

### Implement a Naive Bayes Classifier and Evaluate It on a Real Dataset

**Main Contents:**

- How to implement a machine learning algorithm and apply it to a real dataset?
- How to evaluate the performance of a machine learning model?
- How to analyze experimental results?

**Note:** All three parts are important and should be reflected in the code/report.

---

### Hypothesis: 
\(P(y|x_1, \ldots, x_n) \propto P(y) \prod_{i=1}^n P(x_i|y)\)

**Training Phase:**

- Estimate \(P(y)\) and \(P(x_i|y)\)

**Testing Phase:**

- Output \(\hat{y} = \arg\max_y P(y) \prod_{i=1}^n P(x_i|y)\)

---

### Task: Determine whether an email is spam

**Dataset:** English email dataset  
[https://plg.uwaterloo.ca/~gvcormac/treccorpus06/](https://plg.uwaterloo.ca/~gvcormac/treccorpus06/)

**File Format:**

- `./data/`: Each file is an email, including body and metadata (total 37,822 emails)
- `./label/index`: Each line includes the label (spam/ham) and the relative path to the corresponding email
- There might be some noisy data (e.g., different encodings)

---

### Train the classifier on the training set and test its performance on the test set

- Use five-fold cross-validation
- At least report average accuracy:
  \[
  \text{Accuracy} = \frac{\text{Number of correctly classified samples}}{\text{Number of test samples}}
  \]
- Encourage using other relevant evaluation metrics (e.g., precision, recall, or F1)

---

### What problems did you encounter or explore during the experiment?

- How to analyze and solve problems?
- How to design further experiments?
- How to adjust the algorithm?
- Was the solution effective?
- Did it improve the model's performance?
- Finally, explain the reason for the effectiveness (or ineffectiveness) of the solution.

---

### How does the size of the training set affect the performance of the classifier?

**Suggested Scheme:**

- Sample 5%, 50%, and 100% of the training set data for training and observe performance changes

---

### Suppose there is no sample with \(x_i = k, y = c\) in the training set

- Then \(P(y=c|x_1, \ldots, x_i=k, \ldots, x_n) = 0\)
- What impact does this have on performance? Under what circumstances might this happen?

**A Possible Solution:**

- Smoothing: \(\hat{P}(x_i = k|y = c) = \frac{\# \{x_i=k, y=c\} + \alpha}{\# \{y=c\} + \alpha N}\)

\(\alpha\) is a smoothing parameter, \(N\) is the number of possible values for \(x_i\)

---

### What other features can be used besides the bag-of-words model?

**Hints:**

- Received from...
- Time
- Priority/Mailer

---

### Implement a Naive Bayes classifier (30%)

Solve the following three problems:

- Problem 1 (30%)
- Problems 2 & 3 (2 * 20% = 40%)

**Note:** Scoring is not based on model performance but on how you implement the algorithm, evaluate the model, and analyze the experimental results.

---

### A compressed file containing the following:

**Source Code**

- With necessary comments
- Ensure that the TA can understand and run the code to reproduce the results (pay attention to setting random seeds)

**README**

- A text file (UTF8 encoding) containing your name, student ID, contact information, and code running instructions

**Report**

- A PDF file: experiment design/results/analysis/discussion
- Do not directly copy the code
- Do not upload the dataset

---

### Deadline: 2024.04.07 Sunday 23:59

- Upload the compressed file to the course system, the file name should be Name_StudentID
- Late submission will result in point deductions
  - Late ≤ one week: 0.8; Late > one week: 0.6
- If there are special circumstances, please inform the TA in advance
- Plagiarism of code and reports is not allowed. The school provides an assignment plagiarism detection system, and assignments confirmed to be plagiarized will be severely penalized.

---

**Contact TAs:**

- Wang Yifan, Li Jiayu, He Zhiyu
- {yf-wang21, jy-li20, hezy22}@mails.tsinghua.edu.cn

---

### References:

[http://scikit-learn.org/stable/modules/naive_bayes.html](http://scikit-learn.org/stable/modules/naive_bayes.html)  
(Basic theory and smoothing techniques)

**Note:** For reference only, the core algorithm should be implemented by yourself.

