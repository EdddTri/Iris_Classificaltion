# 🌸 Iris Classification with Support Vector Machines (SVM)

This project demonstrates how to implement **Support Vector Machines (SVM)** from scratch (using convex optimization) and compare them with scikit-learn’s implementation on the **Iris dataset**. Both **hard-margin** and **soft-margin** approaches are covered, along with visualizations of decision boundaries, margins, and support vectors.

---

## 📂 Project Structure
- **IRIS_Classification_SVM.ipynb** → Jupyter Notebook containing all experiments and visualizations.  
---

## ⚙️ Code Workflow
1. **Dataset Preparation**
   - Loads the **Iris dataset**.
   - Uses feature subsets (`sepal length`, `petal width`, etc.).
   - Normalizes features using `StandardScaler`.

2. **Custom Hard-Margin SVM**
   - Implemented with `cvxpy`.
   - Optimizes weight vector and bias with constraints.
   - Visualizes decision boundaries and margins.

3. **Soft-Margin SVM**
   - Adds regularization parameter `C` to handle non-separable data.
   - Compares with hard-margin results.

4. **One-vs-All Strategy**
   - Multi-class classification built from binary SVMs.

5. **Visualization Functions**
   - Plots **decision boundaries**, **margins**, and **support vectors**.

---

## 📊 Results & Visualizations

### 🔹 1. Hard-Margin SVM Decision Boundary 
Plots decision boundary and margins for binary classification between *Setosa* and *Non-Setosa*.  
Support vectors are circled.

---

### 🔹 2. Hard-Margin SVM (Alternate Features)
Shows the separating hyperplane with margins for another feature subset.

---

### 🔹 3. scikit-learn SVM (Linear Kernel, Original Data)  
Trains a **linear kernel SVM** with sklearn on raw Iris data.  
Support vectors (circled) define the margin.

---

### 🔹 4. scikit-learn SVM (Linear Kernel, Normalized Data)
Same SVM as above, but trained on **normalized features**.  
Decision boundary is better aligned after scaling.

---

### 🔹 5. Custom SVM: Hard vs Soft Margin)  
Comparison:
- **Top** → Hard-Margin SVM  
- **Bottom** → Soft-Margin SVM (allows some misclassification, more robust).  

---

### 🔹 6. Final Visualization: Margins & Support Vectors  
Shows the decision boundary with support vectors explicitly circled.  

---
## 📌 Key Learnings

- **Hard-Margin SVM** works only with linearly separable data.  
- **Soft-Margin SVM** generalizes better for noisy data.  
- **Feature normalization** is crucial for SVM performance.  
- **Support vectors** alone define the decision boundary.  
