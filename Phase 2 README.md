PHASE 2
Part A — Intelligent Weather Prediction System

Objective
The Weather Prediction System analyses historical meteorological observations and develops machine-learning and deep-learning models for temperature prediction.
The implemented workflow includes data inspection, preprocessing, exploratory analysis, feature engineering, supervised learning, feature-importance analysis,
and temporal sequence modelling.

Main Workflow
Historical Weather Dataset
          │
          ▼
Data Inspection
          │
          ▼
Data Cleaning
          │
          ▼
Datetime Processing
          │
          ▼
Exploratory Data Analysis
          │
          ▼
Feature Engineering
          │
          ▼
Train/Test Preparation
          │
          ▼
Machine Learning Models
          │
          ▼
Model Evaluation
          │
          ▼
Feature Importance
          │
          ▼
LSTM Sequence Modelling
          │
          ▼
Prediction & Visualization

Machine Learning Models
The implementation includes three classical regression models:
Linear Regression
Decision Tree Regression
Random Forest Regression

The target variable is:
Temperature (°C)

The models are evaluated using:
Mean Absolute Error (MAE)
Root Mean Squared Error (RMSE)
R² Score
Feature Engineering

The prediction pipeline includes several engineered features designed to capture temporal and nonlinear relationships in meteorological observations.

Examples include:
Temperature–humidity interaction
Temperature–pressure interaction
Wind–visibility interaction
24-observation rolling mean
Rolling temperature variability
Lagged temperature
Lagged humidity
Lagged pressure
Month-based cyclical features
Hour-based cyclical features
LSTM Model

The project also investigates temporal deep learning using an LSTM network.
The implemented sequence model uses:
Sequence length: 24 observations
LSTM layer: 64 units
Dropout
LSTM layer: 32 units
Dropout
Single-neuron output layer
Adam optimizer
Mean Squared Error loss

The LSTM component is intended as a prototype for learning temporal dependencies within historical weather observations.

Part B — Generative AI Weather Research Assistant
Objective
The Weather Research Assistant provides natural-language access to scientific weather and climate information.

Instead of relying only on the language model's internal knowledge, the system retrieves relevant information from a curated collection of scientific documents
and uses that retrieved context to generate responses.

RAG Workflow
Scientific PDF Documents
          │
          ▼
Document Loading
          │
          ▼
Text Extraction
          │
          ▼
Text Chunking
          │
          ▼
Semantic Embeddings
          │
          ▼
FAISS Vector Database
          │
          ▼
Similarity Search
          │
          ▼
Relevant Scientific Context
          │
          ▼
Gemini
          │
          ▼
Grounded Response

Technologies Used
Weather Prediction
Python
Pandas
NumPy
Scikit-learn
Matplotlib
Machine Learning
LSTM / Deep Learning
Research Assistant
Python
LangChain
PyPDFLoader
RecursiveCharacterTextSplitter
Sentence Transformers
all-MiniLM-L6-v2
FAISS
Google Gemini

The submitted implementation uses PyPDFLoader for document ingestion,RecursiveCharacterTextSplitter for segmentation, Sentence Transformers for local embeddings, FAISS for similarity search, and Gemini for response generation.

Key Capabilities
Weather Prediction System
Historical weather-data analysis
Data preprocessing
Missing-value analysis
Duplicate detection
Exploratory data analysis
Feature engineering
Multiple regression models
Model comparison
Feature importance analysis
LSTM-based sequence modelling
Prediction visualization
Weather Research Assistant
Scientific PDF ingestion
Text extraction
Semantic document chunking
Dense embeddings
Vector database construction
Similarity-based retrieval
Scientific context retrieval
Gemini-based response generation
Retrieval-grounded answers

Project Structure
Phase2/
│
├── Weather Prediction/
│   ├── notebook / implementation
│   ├── dataset
│   └── outputs
│
└── Weather Research Assistant/
    ├── notebook / implementation
    ├── scientific documents
    ├── vector database
    └── generated responses

Project Outcome
Phase 2 demonstrates two complementary AI pipelines:
Numerical Intelligence
Historical meteorological observations → Machine Learning / Deep Learning → Temperature Prediction
Knowledge Intelligence
Scientific Documents → RAG → Evidence-Grounded Scientific Answers
The combination provides a foundation for a broader weather and climate
decision-support system.

Limitations
The systems should be considered research and internship prototypes rather than production-grade forecasting systems. The weather prediction component does not replace operational numerical weather
prediction systems, and the Research Assistant depends on the quality,
coverage, and authority of its document corpus.

Future Scope
Potential extensions include:
Larger and more diverse meteorological datasets
Advanced forecasting models
Transformer-based time-series models
Improved LSTM architectures
SHAP-based explainability
Better uncertainty estimation
Larger scientific document collections
Hybrid semantic and keyword retrieval
RAG evaluation benchmarks
Multimodal weather intelligence
Real-time weather-data integration
Unified decision-support interface

Conclusion
Phase 2 establishes an integrated foundation for AI-assisted weather and climate intelligence by combining predictive modelling with retrieval-grounded scientific
knowledge assistance. The project demonstrates how machine learning, deep learning, semantic retrieval, and generative AI can work together to support both numerical prediction and scientific information discovery.

Technologies
Python
Pandas
NumPy
Scikit-learn
LSTM / Deep Learning
LangChain
Sentence Transformers
FAISS
Google Gemini
Matplotlib

Project Outcome
The project establishes a prototype multi-modal weather intelligence platform that combines data-driven prediction with retrieval-grounded scientific
information assistance.

Future Scope
Advanced time-series and transformer models
Improved explainability
Larger scientific knowledge bases
Real-time weather-data integration
Multimodal weather intelligence
Unified decision-support interface

Author
M. Ayshwarya
