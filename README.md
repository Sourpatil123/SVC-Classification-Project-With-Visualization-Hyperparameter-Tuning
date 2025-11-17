# SVC-Classification-Project-With-Visualization-Hyperparameter-Tuning

his project demonstrates the implementation of Support Vector Classifier (SVC) on a synthetic binary classification dataset.
The dataset is generated using make_classification() with two features, making it ideal for visualization using a 2D scatter plot.
📌 Project Overview

Generated dataset using make_classification
X, y = make_classification(
    n_samples=1000,
    n_features=2,
    n_classes=2,
    n_clusters_per_class=2,
    n_redundant=0
)

Visualized data using a scatter plot.

Built SVC models using:

Default SVC

Sigmoid Kernel SVC

Hyperparameter Tuned SVC (GridSearchCV)

Evaluated using:

Precision

Recall

F1-Score

📊 Dataset Visualization

A scatter plot was created to show the separation between the two classes using the two generated features.
This helps in understanding SVC’s boundary and margin effectiveness.

🧠 Model Performance
1️⃣ Train Results (Default SVC)
| Metric    | Score    |
| --------- | -------- |
| Precision | **0.96** |
| Recall    | **0.91** |
| F1 Score  | **0.93** |

2️⃣ Test Results (Default SVC)
| Metric    | Score    |
| --------- | -------- |
| Precision | **0.95** |
| Recall    | **0.92** |
| F1 Score  | **0.93** |

🔁 Sigmoid Kernel Performance
| Metric    | Score    |
| --------- | -------- |
| Precision | **0.55** |
| Recall    | **0.81** |
| F1 Score  | **0.83** |

⚙️ Hyperparameter Tuning – GridSearchCV

A tuning experiment was performed using GridSearchCV to optimize SVC parameters such as:

C

gamma

kernel

Best Model Performance
| Metric    | Score    |
| --------- | -------- |
| Precision | **0.94** |
| Recall    | **0.92** |
| F1 Score  | **0.93** |

📈 Conclusion

Default SVC performed best overall with strong precision, recall, and F1 on both train and test data.

Sigmoid kernel underperformed, showing why kernel selection is important.

GridSearchCV tuning produced a well-balanced model close to the original SVC performance.

The project demonstrates:

Model building

Visualization

Model evaluation

Kernel comparison

Hyperparameter tuning

📁 Technologies Used

Python

Scikit-learn

NumPy

Matplotlib
