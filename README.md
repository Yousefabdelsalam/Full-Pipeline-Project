# 🔁 ML Pipelines Project: Nested Preprocessing Pipelines with Scikit-Learn

## 📌 Project Description

This project demonstrates how to build **modular and reusable preprocessing pipelines** using Scikit-Learn.  
The main goal is to show how to structure all preprocessing tasks like **filling missing values**, **encoding categorical features**, and **transforming numeric columns** inside **pipelines** — and then combine them together in a clean and scalable way.

Instead of writing manual steps for each transformation, this project uses:
- `make_pipeline` for creating step-by-step preprocessing flows
- `ColumnTransformer` for applying different pipelines to different feature groups
- Full integration with ML models (e.g., Logistic Regression, Random Forest)

## 🛠️ Techniques Used

- **Missing Value Handling**
  - `SimpleImputer` (most frequent strategy)
  - `KNNImputer`
- **Encoding**
  - `OneHotEncoder` (with drop='first')
  - `BinaryEncoder` (from `category_encoders`)
- **Numerical Transformation**
  - `FunctionTransformer(np.log1p)`
- **Pipeline Tools**
  - `Pipeline`, `make_pipeline`, `ColumnTransformer`
- **Model Integration**
  - Training classifiers inside the final pipeline

## 🚀 Why It Matters

Using nested pipelines keeps your ML workflow:
- **Organized**
- **Scalable**
- **Easy to tune and debug**
- **Ready for deployment**

This structure is especially helpful when working on real-world machine learning systems where preprocessing needs to be repeatable and reliable.

## 📂 Files

- `Full Pipeline.ipynb`: Jupyter notebook with all code and explanations
- `README.md`: This file

---

Feel free to fork this project or reach out if you want help building your own preprocessing pipeline!

