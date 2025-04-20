# boston-crime-prediction
This project uses machine learning classification models to predict whether neighborhoods in Boston exceed the median crime rate per capita, based on the Boston Housing dataset. Key features include CRIM, ZN, INDUS, CHAS, NOX, and others, with Logistic Regression and KNN applied to classify the outcome.

flowchart TD
    %% Nodes
    A("fa:fa-database Load Data")
    B("fa:fa-chart-bar Explore Correlations")
    C("fa:fa-chart-line Visualize Crime Distribution")
    D("fa:fa-sliders-h Define Binary Target")
    E{"fa:fa-random Train / Val / Test Split"}
    F("fa:fa-robot Logistic Regression")
    G("fa:fa-check Evaluate Accuracy")
    H("fa:fa-cogs Train Final Logistic Model")
    I("fa:fa-project-diagram KNN (Varying K)")
    J("fa:fa-thumbs-up Select K = 16")
    K("fa:fa-brain Train Final KNN Model")
    L("fa:fa-vial Test Set Evaluation")
    M("fa:fa-balance-scale Compare Models & Conclude")

    %% Connections
    A --> B --> C --> D --> E
    E --> F --> G
    G --> H
    G --> I --> J --> K
    H --> L
    K --> L --> M

    %% Styling
    style A fill:#1565C0,stroke:#0D47A1,color:#fff
    style E fill:#6A1B9A,stroke:#4A148C,color:#fff
    style F fill:#2E7D32,stroke:#1B5E20,color:#fff
    style I fill:#00897B,stroke:#00695C,color:#fff
    style L fill:#EF6C00,stroke:#E65100,color:#fff
    style M fill:#C62828,stroke:#B71C1C,color:#fff


