# Support Vector Machines (SVM)

`supervised learning`

Used for classification and regression.

The fundamental idea behind SVM is to find a hyperplane \(plane in higher dimensions\) that best separates the different classes of data while maximizing the margin \(distance\) between the classes. This hyperplane is called the **decision boundary**.
![image.png](image/image.png)

The data points closest to the decision boundary are known as **support vectors**, and they play a crucial role in determining the position and orientation of the decision boundary, while data points farther from the decision boundary contribute less to the decision boundary.

## Kernel SVM

In cases where the data is not linearly separable, SVMs can use kernel functions to transform the input data into a higher\-dimensional space where the classes might become linearly separable. These kernels allow SVMs to capture complex relationships within the data.
