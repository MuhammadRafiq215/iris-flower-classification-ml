# 🌸 Iris Flower Classification Using Machine Learning

A complete machine learning project that explores the classic Iris dataset, analyzes flower measurements, trains multiple classification algorithms, and evaluates their performance using cross-validation, hyperparameter tuning, and classification metrics.

## 📌 Project Overview

The Iris Flower Classification project demonstrates an end-to-end supervised machine learning workflow using Python. The objective is to predict the species of an Iris flower from four numerical measurements of its flower parts.

The project combines exploratory data analysis (EDA), data preprocessing, model development, hyperparameter optimization, and performance evaluation in a reproducible Jupyter Notebook.

It is designed to demonstrate practical skills in data analysis, machine learning, model selection, and communicating results.

## 🎯 Objectives

- Explore and understand the Iris dataset.
- Inspect dataset dimensions, data types, missing values, and descriptive statistics.
- Visualize relationships between flower measurements and species.
- Examine feature distributions and potential classification patterns.
- Split the data into training and testing sets using stratified sampling.
- Train and compare multiple machine learning classifiers.
- Use stratified cross-validation to assess model performance.
- Optimize model hyperparameters using `GridSearchCV`.
- Evaluate the selected model on unseen test data.
- Interpret model performance and investigate feature importance.

## 📊 Dataset

This project uses the **Iris dataset**, a well-known classification dataset available directly through `scikit-learn`.

The dataset contains **150 observations**, **four numerical features**, and **three Iris species**, with 50 observations per species.

### Features

| Feature | Description |
|---|---|
| Sepal length | Length of the sepal in centimetres |
| Sepal width | Width of the sepal in centimetres |
| Petal length | Length of the petal in centimetres |
| Petal width | Width of the petal in centimetres |

### Target classes

- *Iris setosa*
- *Iris versicolor*
- *Iris virginica*

The dataset is loaded directly from `scikit-learn`, so a separate dataset download is not required.

## 🛠️ Technologies and Libraries

- **Python** — programming language
- **NumPy** — numerical computing
- **Pandas** — data inspection and analysis
- **Matplotlib** — data visualization
- **Seaborn** — statistical visualization
- **Scikit-learn** — preprocessing, model training, cross-validation, tuning, and evaluation
- **Jupyter Notebook** — interactive analysis and documentation

## 🔬 Project Workflow

### 1. Data Loading and Inspection

Load the Iris dataset and inspect its structure, feature names, target classes, dimensions, data types, missing values, and descriptive statistics.

### 2. Exploratory Data Analysis

Use visualizations to investigate the relationships between flower measurements and species, including:

- Pairplot of the numerical features grouped by species
- Feature distribution and boxplots
- Comparisons of sepal and petal measurements
- Analysis of potentially informative features

### 3. Data Preparation

Separate the predictors from the target variable and create a stratified 80:20 training-test split.

Stratification preserves the class proportions across the two subsets. A fixed random seed supports reproducibility.

### 4. Model Training

Train and compare multiple classification algorithms:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest

Where appropriate, preprocessing is incorporated into scikit-learn pipelines to keep the workflow organized and help prevent data leakage during cross-validation.

### 5. Cross-Validation and Hyperparameter Tuning

Use stratified five-fold cross-validation to compare candidate models. Apply `GridSearchCV` to explore selected hyperparameters and identify a strong candidate model using the chosen macro F1-score criterion.

### 6. Model Evaluation

Evaluate the selected model on the held-out test set using:

- Accuracy
- Precision
- Recall
- F1-score
- Classification report
- Confusion matrix

The notebook also examines permutation feature importance to investigate how the input features contribute to predictive performance.

### 7. Interpretation

Compare the results, discuss the strengths and limitations of the candidate models, and identify which flower measurements are most useful for distinguishing the species.

Final performance values should be taken from the executed notebook rather than assumed in advance.

## 📈 Evaluation Metrics

| Metric | Purpose |
|---|---|
| Accuracy | Proportion of correctly classified samples |
| Precision | How often predictions for a class are correct |
| Recall | How many actual samples of a class are identified |
| F1-score | Harmonic mean of precision and recall |
| Confusion matrix | Shows correct and incorrect predictions by class |
| Cross-validation | Estimates performance across multiple training-validation splits |

Macro-averaged metrics give each species equal weight, making them useful for comparing performance across the three classes.

## 📂 Repository Structure

```text
iris-flower-classification-ml/
├── README.md


## ⚙️ Installation and Setup

### Prerequisites

- Python 3.10 or later
- Jupyter Notebook or JupyterLab
- `pip`

### 1. Clone the repository

```bash
git clone https://github.com/MuhammadRafiaq215/iris-flower-classification-ml.git
cd iris-flower-classification-ml
```

Replace the GitHub username in the clone URL if your actual username differs.

### 2. Create a virtual environment (recommended)

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

On macOS or Linux:

```bash
source .venv/bin/activate
```

### 3. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `iris_flower_classification.ipynb` and run the cells from top to bottom.

## 📦 Dependencies

The `requirements.txt` file should include:

```text
numpy
pandas
scikit-learn
matplotlib
seaborn
jupyter
notebook
```

## 💡 Key Learning Outcomes

This project provides practical experience with:

- Exploratory data analysis and statistical visualization
- Feature-target separation and stratified sampling
- Machine learning pipelines and preprocessing
- Supervised classification algorithms
- Cross-validation and model selection
- Hyperparameter optimization
- Classification metrics and error analysis
- Permutation feature importance
- Reproducible data science workflows

## ⚠️ Limitations

- The Iris dataset is small and relatively clean compared with real-world datasets.
- Strong results on this dataset do not guarantee similar performance on more complex datasets.
- Cross-validation and test scores may vary with the split and model configuration.
- Feature importance indicates predictive usefulness, not necessarily a causal relationship.

## 🚀 Future Improvements

- Add additional classification algorithms and compare their performance.
- Explore alternative cross-validation strategies.
- Add learning curves to investigate model generalization.
- Export selected plots and evaluation results into the repository.
- Experiment with a simple interactive prediction interface.
- Apply the same workflow to larger, more challenging classification datasets.

## 👨‍💻 Author

**Muhammad Rafique**

Aspiring AI & Data Science Student

Interested in machine learning, data analysis, Python development, and building practical software projects.

## 📜 License

This project can be published under the MIT License if you choose to distribute your code under those terms. Add a `LICENSE` file containing the MIT License before describing the repository as MIT-licensed.

## ⭐ Acknowledgements

- The scikit-learn team for providing convenient access to the Iris dataset and machine learning tools.
- The open-source Python data science community for its excellent libraries and educational resources.

---

**If you find this project useful, consider giving the repository a star!**
