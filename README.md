# boston-crime-prediction
This project uses machine learning classification models to predict whether neighborhoods in Boston exceed the median crime rate per capita, based on the Boston Housing dataset. Key features include CRIM, ZN, INDUS, CHAS, NOX, and others, with Logistic Regression and KNN applied to classify the outcome.

```mermaid
flowchart TD
    A[Load Data] --> B[Explore Descriptive Stats & Correlations]
    B --> C[Visualize Skewed Distribution of Crime Rates]
    C --> D[Define Binary Target: crim_over_thresh (Median Split)]
    D --> E[Split Dataset (Train / Val / Test)]
    E --> F[Logistic Regression (Univariate Predictors)]
    F --> G[Evaluate on Validation Set → Best Predictor: NOX]
    G --> H[Train Logistic Model with Best Predictor]
    G --> I[KNN Models with Varying K on Best Predictor]
    I --> J[Select Optimal K (k=16) to Avoid Overfitting]
    J --> K[Train KNN with Optimal K]
    H --> L[Test Set Evaluation: Classification Report]
    K --> L
    L --> M[Conclusion: KNN Outperforms Logistic Regression]

