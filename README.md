# Census Bureau Income Classification & Segmentation Analysis

## Project Overview
This project addresses two key business objectives for a retail marketing client:
1. **Classification**: Predict whether individuals earn <$50k or >$50k based on 40 demographic/employment variables
2. **Segmentation**: Identify customer segments for targeted marketing strategies

## Data
- **Source**: 1994-1995 Current Population Surveys (Census Bureau weighted data)
- **Location**: `census-bureau.data` (data) and `census-bureau.columns` (column definitions)
- **Variables**: 40 demographic and employment features + weight + income label

## Project Structure
```
Project/
├── census-bureau.data              # Raw data file
├── census-bureau.columns           # Column definitions
├── 01_classification_model.ipynb   # Classification model development
├── 02_segmentation_model.ipynb     # Segmentation model development
├── README.md                       # This file
└── PROJECT_REPORT.md               # Client-facing report
```

## Setup Instructions

### Prerequisites
- Python 3.8+
- Jupyter Notebook
- Required packages: pandas, numpy, scikit-learn, matplotlib, seaborn, plotly

### Installation
```bash
# Create virtual environment (recommended)
python -m venv venv
source venv/Scripts/activate  # On Windows

# Install dependencies
pip install pandas numpy scikit-learn matplotlib seaborn plotly jupyter scipy imbalanced-learn
```

### Running the Analysis

#### 1. Classification Model
```bash
jupyter notebook 01_classification_model.ipynb
```
This notebook covers:
- Data loading and exploration
- Data Exploration and preprocessing
- Model training (multiple classifiers)
- Model evaluation
- Results interpretation

#### 2. Segmentation Model
```bash
jupyter notebook 02_segmentation_model.ipynb
```
This notebook covers:
- Data preparation for clustering
- Clustering analysis (K-means)
- Segment characterization

## Key Considerations
- **Weighted Sampling**: Data includes sampling weights
- **Class Imbalance**: Income distribution may be imbalanced
- **Feature Types**: Mix of categorical and numeric features
- **Business Context**: Focus on interpretability for marketing applications

## Deliverables Summary
1. ✅ `01_classification_model.ipynb` - Classification code
2. ✅ `02_segmentation_model.ipynb` - Segmentation code
3. ✅ `README.md` - Execution instructions
4. ✅ `PROJECT_REPORT.md` - Client report with findings & recommendations

## Notes
- All analysis emphasizes business interpretability over model complexity
- Code includes comments explaining key decisions and trade-offs
- Visualizations support business recommendations for marketing
