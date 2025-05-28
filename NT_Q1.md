# NT_Q1

# Fact-Checking and Bias Detection Model

## Week 1: Problem Understanding, Data Sourcing, and Initial EDA

**Tasks**

- Split into:
    1. Fact-checking (true/false).
    2. Bias detection (left-leaning, right-leaning, speculative, factual).
- Inputs: News article text; Outputs: Labels for fact-checking and bias.
- Fact-checking datasets: LIAR, FEVER.
- Bias datasets: Media Bias/Fact Check, AllSides.
- Create label distributions (eg. PCA scatter plot), standard deviation etc. to understand the data.
- Identify issues such as class imbalance, noise
- Plan Preprocessing such as Cleaning, tokenization, vectorization (TF-IDF/embeddings).
- If necessary, perform manual labelling or synthetic data set generation.

**Deliverable**

Problem statement document, dataset retrieval pipeline, preprocessing plan

## Week 2: Data Preprocessing, Advanced EDA, and Baseline Models

**Tasks**

- Perform preprocessing. Refine the pipeline to improve data quality
- Create baseline ML model like K-Means clustering, to evaluate preprocessing performance
- Perform advanced EDA such as feature recognition.
- Ideate and research which model is best suited for the job.
- If using synthetic data, try to increase diversity of data.
- Maintain versioning between different preprocessing pipelines

**Deliverables**

EDA document, baseline metrics for different preprocessing pipelines, identify model to use for trainiing

## Week 3: Model Training, and Optimization

**Tasks**

- Evaluate ideal GPU provider to use. Consider using team mate laptops together for a Multi-GPU training using methods like Federated Learning.
- Write model algorithm. Train on preprocessed data. Evaluate performance
- Decide if current approach will be successful. If not pivot to another approach.
- If model is finalized (such as LSTM, BERT, CNN), start hyperparameter tuning using software such as Optuna.

**Deliverables**

Model Metrics, graphs.

## Week 4: Explore advanced methods

**Tasks**

- Explore advanced methods to improve performance. Refine all parts of the pipeline from processing to training, to get small gains in performance
- Build frontend using frameworks like StreamLit. Build the product that we will pitch/ship.
- Organize all documented data such as metrics, references, custom algorithms, citations etc.

**Deliverables**

Documentation and final product/app.

## Team Roles

- **Model**: Write implementation for the model. Perform tuning.
- **Data**: EDA, feature engineering.
- **Frontend**: Streamlit, ChromaDB and other software to support the model
- **Project Manager**: Coordination, timelines

## Risk Mitigation

- Regular meets
- problem in a domain of expertise of at least one of team members
- Proper version control for keeping backups
- Baseline model comparison for ball-park estimates
- Room for pivoting in Week 2 and 3