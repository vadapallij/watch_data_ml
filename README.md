# Watch ML Pipeline

## Directory Structure

```
watch-ml/
├── data/
│   ├── raw/         # Raw CSV/Parquet logs
│   ├── interim/     # Cleaned, resampled data
│   ├── features/    # Engineered features (Parquet)
│   └── models/      # Saved model checkpoints
├── src/
│   ├── ingest.py           # Data ingestion
│   ├── preprocess.py       # Data cleaning & preprocessing
│   ├── features.py         # Feature engineering
│   ├── dataset.py          # Dataset creation
│   ├── train.py           # Model training
│   ├── eval.py            # Model evaluation
│   ├── deploy_export.py   # Model deployment preparation
│   └── realtime.py        # Real-time inference
├── mlruns/          # MLflow experiment tracking
└── requirements.txt # Python dependencies
```

## Setup

```bash
cd watch-ml
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```
