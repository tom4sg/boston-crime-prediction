# boston-crime-prediction
This project uses machine learning classification models to predict whether neighborhoods in Boston exceed the median crime rate per capita, based on the Boston Housing dataset. Key features include CRIM, ZN, INDUS, CHAS, NOX, and others, with Logistic Regression and KNN applied to classify the outcome.

<pre><code>```mermaid flowchart TD A[Load Data] --> B[Explore Descriptive Stats and Correlations] B --> C[Visualize Skewed Distribution of Crime Rates] C --> D[Define Binary Target: crim\_over\_thresh] D --> E[Split Dataset: Train / Val / Test] E --> F[Logistic Regression on Each Predictor] F --> G[Evaluate Validation Accuracy - Best: NOX] G --> H[Train Logistic Model on NOX] G --> I[KNN Models with Varying K on NOX] I --> J[Select K = 16 (Avoid Overfitting)] J --> K[Train Final KNN Model] H --> L[Test Set Evaluation: Classification Report] K --> L L --> M[Conclusion: KNN Outperforms Logistic Regression] ```</code></pre>

