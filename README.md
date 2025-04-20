# boston-crime-prediction
This project uses machine learning classification models to predict whether neighborhoods in Boston exceed the median crime rate per capita, based on the Boston Housing dataset. Key features include CRIM, ZN, INDUS, CHAS, NOX, and others, with Logistic Regression and KNN applied to classify the outcome.


```mermaid
graph TD;
    A[Load Data] --> B[Explore Descriptive Stats and Correlations];
    B --> C[Visualize Crime Rate Distribution];
    C --> D[Define Binary Target (crim_over_thresh)];
    D --> E[Split Data: Train / Val / Test];
    E --> F[Logistic Regression on Each Feature];
    F --> G[Evaluate Accuracy, Select Best Feature];
    G --> H[Train Final Logistic Model];
    G --> I[Train KNN with Varying K];
    I --> J[Select Best K (e.g. K=16)];
    J --> K[Train Final KNN Model];
    H --> L[Test Set Evaluation];
    K --> L;
    L --> M[Compare Models and Draw Conclusion];
```
