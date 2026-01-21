# Obesity Classification Workflow 

```mermaid
flowchart TD
    Start --> Import[Import Libraries]
    Import --> Load[Load Dataset]
    Load -->|Yes| Clean[Clean Data]
    Load -->|No| Fail[Dataset load failed]
    Clean --> Analyze[Analyze Data]
    Analyze --> Preprocess[Preprocess Data]
    Preprocess --> Models[Initialize Models]
    Models --> Train[Train Models]
    Train --> Predict[Predict & Evaluate]
    Predict --> Compare[Compare Models]
    Compare --> Best[Select Best Model]
    Best --> Final[Generate Final Predictions]
    Final --> Visual[Visualize Results]
    Visual --> End[End]

