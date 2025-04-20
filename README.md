# boston-crime-prediction
This project uses machine learning classification models to predict whether neighborhoods in Boston exceed the median crime rate per capita, based on the Boston Housing dataset. Key features include CRIM, ZN, INDUS, CHAS, NOX, and others, with Logistic Regression and KNN applied to classify the outcome.


```mermaid
graph TD;
    A[Load Data] --> B[Explore and Visualize];
    B --> C[Create Target Variable];
    C --> D[Split Data];
    D --> E[Train Logistic Regression];
    D --> F[Train KNN];
    E --> G[Evaluate Models];
    F --> G;
    G --> H[Compare Results];
```
