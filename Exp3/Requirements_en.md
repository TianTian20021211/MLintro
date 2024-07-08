Sure, here is the translation of the document:

---

## Experiment 3: Ensemble Learning

- **Introduction to Machine Learning - Third Experiment**
- **Spring 2024**

### Experiment 3: Ensemble Learning

- Implement different ensemble learning algorithms.
- Compare their performance when combined with different base classifiers.
- Four combinations in total.
- Two ensemble learning algorithms: Bagging, AdaBoost.
- Two base classifiers: SVM, Decision Tree.
- Base classifiers can use existing toolkits.
- However, the ensemble learning algorithms need to be implemented by yourself.

### Task: Rating Prediction Based on Reviews

- `exp3-reviews.csv`: 220,000 entries.
- Please do not use data from other resources, including pre-trained word vectors.

### Dataset Columns:

- **overall**: The label column indicating the user's rating of the item (from 1 to 5).
- **reviewerID**: Unique identifier for each reviewer.
- **asin**: Unique identifier for each item.
- **unixReviewTime**: Timestamp of the review text.
- **summary**: Summary of the review content, in English, unprocessed.
- **reviewText**: Full review content, in English, unprocessed.

### Requirements:

- Implement Bagging and AdaBoost (60%).
- Compare and analyze the 4 combinations (40%).
- Metrics: At least include MAE, RMSE.
- Both classification and regression tasks are allowed.
- Split the data into training and testing sets in a 9:1 ratio.
- If the data is too large, you may sample it.
- Note: The grading is based on your implementation method, performance evaluation, and result analysis, not model performance (e.g., accuracy).

### Submission:

- A compressed file containing the following:
  - **Source Code**:
    - Include necessary comments.
    - Ensure the TA can understand and run the code to reproduce the results (set random seeds).
  - **README**:
    - A text file (UTF-8 encoded) with your name, student ID, contact information, and code running guide.
  - **Report**:
    - A PDF file with experimental design, results, analysis, and discussion (do not copy the code directly).
  - Do not upload the dataset.

### Deadline:

- **2024.05.12 Sunday 23:59:00**.
- Upload the compressed file to the online learning platform, named as **Name_StudentID**.
- Late submissions will be penalized.
  - Late ≤ one week: 0.8; Late > one week: 0.6.
- If there are special circumstances, inform the TA in advance.
- Code and report plagiarism is not allowed.
  - The school provides an assignment plagiarism detection system. Confirmed plagiarized assignments will be severely penalized.
- For any questions, contact the TAs:
  - Wang Yifan, Li Jiayu, He Zhiyu
  - {yf-wang21, jy-li20, hezy22}@mails.tsinghua.edu.cn

### Tools:

- **SVM**:
  - Sklearn: [https://scikit-learn.org/stable/modules/svm.html](https://scikit-learn.org/stable/modules/svm.html)
  - LibSVM: [https://www.csie.ntu.edu.tw/~cjlin/libsvm/](https://www.csie.ntu.edu.tw/~cjlin/libsvm/)
  - SVM-light: [https://www.cs.cornell.edu/people/tj/svm_light/](https://www.cs.cornell.edu/people/tj/svm_light/)
- **Decision Tree**:
  - Sklearn: [https://scikit-learn.org/stable/modules/tree.html](https://scikit-learn.org/stable/modules/tree.html)
  - C4.5: [http://www.rulequest.com/Personal/](http://www.rulequest.com/Personal/)
  - C5.0: [http://www.rulequest.com/see5-info.html](http://www.rulequest.com/see5-info.html)
- Note: Do not use the ensemble learning tools provided within the packages.

---

If you need further assistance or any modifications, please let me know!