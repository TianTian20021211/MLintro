### Introduction to Machine Learning - Second Experiment
**Spring 2024**

---

### Implementation of K-Means Clustering Algorithm and Evaluation on a Real Dataset

**K-Means Algorithm:**

1. Given the number of clusters \( K \), initialize \( K \) cluster centers: \{g1,…,gk\}.
2. Assign each sample to the nearest cluster center.
3. For each cluster, recalculate its center using all samples belonging to that cluster: \{g1,…,gk\}.
4. Repeat steps 2-3 until a termination condition is met.

---

### MNIST Dataset

- **Publisher:** National Institute of Standards and Technology
- **Description:** A large database of handwritten digit images
- **Training set size:** 60,000
- **Test set size:** 10,000
- **Image normalization:** Ensured digits are centered, size 28x28 pixels
- **Dataset URL:** [MNIST Dataset](https://paperswithcode.com/dataset/mnist)
- **Usage:** Perform K-means clustering and analysis using only the training data
- **Download options:** Available through PyTorch, TensorFlow, Keras, etc.

---

### Code Implementation of K-Means Algorithm

**Challenges:**
- How to determine the number of clusters?
- How to initialize cluster centers?
- How to represent images using feature vectors?
- How to measure sample distances?
- How to set termination conditions?

---

### Model Performance (Quantitative): Accuracy

- **Report the accuracy on the training set**

### Model Performance (Qualitative): Visualization of Clustering Results

- **How to infer the label for each cluster?**
  - e.g., Majority voting
- **How to visualize high-dimensional data?**
  - e.g., t-SNE
  - For large datasets: sample representation
- **Other metrics for evaluating clustering results?**

---

### Issues Encountered or Explored in the Experiment

- **Impact of different implementation details on results:**
  - e.g., Choice of \( K \), initialization of cluster centers, image representation, sample distance measurement
- **Analysis of visualization results:**
  - e.g., Indicating difficult samples
- **Usage of other clustering methods?**

---

### Evaluation Criteria

- **Implementing a K-means algorithm:** 50%
- **Measuring model performance using accuracy:** 20%
- **Visualizing clustering results:** 20%
- **Other experimental analyses:** 10%
- **Note:** Evaluation is based on the implementation of the algorithm, model evaluation, and analysis of experimental results, not solely on model performance (accuracy).

---

### Submission Requirements

**Compressed file containing:**
- **Source code:**
  - Include necessary comments
  - Ensure the TA can understand and run the code to reproduce results (note the random seed setting for cluster initialization)
- **README:**
  - Text file (UTF-8 encoding): name, student ID, contact information, code execution guide
- **Experiment report:**
  - PDF file: experimental design, results, analysis, discussion
  - Do not directly copy code
- **Do not upload the dataset**

---

### Deadline: April 21, 2024 (Sunday) 23:59:00

- **Upload the compressed file to the online learning platform with the file name in the format: Name_StudentID**
- **Late submissions will incur penalties:**
  - Late ≤ one week: 0.8
  - Late > one week: 0.6
- **For special circumstances, contact the TA in advance**
- **Strictly no plagiarism of code and reports**
  - The school provides an assignment plagiarism detection system, and confirmed plagiarism will result in severe penalties
- **For any questions, contact the TA:**
  - Jia-Yu Li, Yi-Fan Wang, Zhi-Yu He
  - {jy-li20, yf-wang21, hezy22}@mails.tsinghua.edu.cn