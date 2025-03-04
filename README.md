This project focuses on detecting credit card fraud using machine learning techniques. The dataset used contains transactions made by credit cards in September 2013 by European cardholders. It is highly imbalanced, with the positive class (frauds) accounting for only 0.17% of all transactions. The project involves data preprocessing, feature scaling, and the application of various machine learning algorithms, including Logistic Regression, K-Nearest Neighbors, Support Vector Classifier, and Decision Tree Classifier. Additionally, techniques like SMOTE (Synthetic Minority Over-sampling Technique) and NearMiss are used to handle the class imbalance. The performance of the models is evaluated using metrics such as precision, recall, F1-score, and ROC-AUC score. The project also includes visualization of the results through confusion matrices and ROC curves.
This project focuses on detecting credit card fraud using machine learning techniques. The dataset used contains transactions made by credit cards in September 2013 by European cardholders. It is highly imbalanced, with the positive class (frauds) accounting for only 0.17% of all transactions. The project involves data preprocessing, feature scaling, and the application of various machine learning algorithms, including Logistic Regression, K-Nearest Neighbors, Support Vector Classifier, and Decision Tree Classifier. Additionally, techniques like SMOTE (Synthetic Minority Over-sampling Technique) and NearMiss are used to handle the class imbalance. The performance of the models is evaluated using metrics such as precision, recall, F1-score, and ROC-AUC score. The project also includes visualization of the results through confusion matrices and ROC curves.

### Handling Large Dataset Files with Git LFS

If you encounter issues while pushing large dataset files to your repository, you can use Git Large File Storage (LFS) to manage them. Follow these steps to resolve the issue:

1. Go to the [Git LFS website](https://git-lfs.com/) and download Git LFS.
2. Install Git LFS by running the following command in your terminal:
    ```bash
    git lfs install
    ```
3. Track your large dataset file (e.g., `creditcard.csv`) with Git LFS:
    ```bash
    git lfs track "creditcard.csv"
    ```
4. Add the `.gitattributes` file created by Git LFS:
    ```bash
    git add .gitattributes
    ```
5. Add your large dataset file:
    ```bash
    git add creditcard.csv
    ```
6. Commit the changes:
    ```bash
    git commit -m "Track creditcard.csv with Git LFS"
    ```
7. Push the project to your repository again:
    ```bash
    git push
    ```

By following these steps, you can manage large files in your repository without encountering issues related to file size limits.