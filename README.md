# 🧠 Early Alzheimer's Prediction from ADNI Data

A machine learning project that uses clinical data from the ADNI dataset to predict early-stage Alzheimer's disease — with a web app for interactive predictions.

---

## What's this about?

Alzheimer's is notoriously hard to catch early. This project explores whether machine learning can help by training models on real clinical data from the **Alzheimer's Disease Neuroimaging Initiative (ADNI)** and predicting which patients are at risk.

The end result is both a trained ML model and a simple web interface where you can input patient data and get a prediction.

---

## Project Structure
  ├── Data/          # Dataset files (ADNI-sourced clinical data)
  
  ├── Notebooks/     # Jupyter notebooks: exploration, preprocessing, model training

  ├── Reports/       # Write-ups, findings, and evaluation results
  
  └── webapp/        # Web app for interactive predictions

  ---

## What's inside the notebooks?

The notebooks walk through the full ML pipeline:

1. **Data loading & exploration** — understanding the ADNI dataset, class distributions, feature visualization
2. **Preprocessing** — handling missing values, encoding, feature scaling
3. **Feature selection** — identifying which clinical markers matter most
4. **Model training** — trying multiple classifiers and tuning them
5. **Evaluation** — comparing models using accuracy, precision, recall, AUC

---

## The Web App

The `webapp/` folder has a simple interface where you input a patient's clinical features and get a prediction from the trained model.

```bash
cd webapp
pip install -r requirements.txt
python app.py
```

Then open `http://localhost:5000` in your browser.

---

## Dataset

This project uses data from **ADNI (Alzheimer's Disease Neuroimaging Initiative)**.

> ADNI data requires access approval — request it at [adni.loni.usc.edu](https://adni.loni.usc.edu/data-samples/access-data/). Access is granted for research purposes.

---

## Tech Stack

- Python
- Jupyter Notebooks
- scikit-learn
- pandas, numpy
- matplotlib, seaborn
- Flask / Streamlit (webapp)

---

## Why this matters

Early detection of Alzheimer's can significantly improve patient outcomes — it opens the door for interventions before severe cognitive decline sets in. ML models trained on clinical data like ADNI can serve as a useful screening tool to flag high-risk patients for further evaluation.

---

## Notes

- This is a research/academic project and is **not** intended for clinical use.
- Model performance details are in the `Reports/` folder.
- Dataset credit goes to the ADNI researchers and participants.
