# Heart Stroke Risk Predictor

A simple Streamlit app that predicts heart disease risk using a trained machine learning model.

## Files

- `app.py` - Streamlit application.
- `Heart.pkl` - Trained classification model.
- `Scaler.pkl` - Feature scaler used before prediction.
- `columns.pkl` - Expected input columns for the model.
- `requirements.txt` - Python dependencies.
- `vercel.json` - Vercel deployment configuration.

## Local setup

1. Create a virtual environment:

```bash
python -m venv venv
```

2. Activate it:

```powershell
venv\Scripts\Activate.ps1
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Run the app:

```bash
streamlit run app.py
```

5. Open the URL shown in your terminal.

## Deploy to Vercel

1. Push this repository to GitHub.
2. In Vercel, create a new project and import your repository.
3. Set the root directory to `heart_risk_predictor` if needed.
4. Vercel will use `vercel.json` and `requirements.txt` automatically.

### Notes

- The app loads the model and scaler from the repo root.
- If deployment issues occur, verify that `vercel.json` is present and the project root is correct.
- Vercel may not be the best fit for persistent Streamlit apps; use Render, Railway, or Fly.io for more consistent Python web hosting if needed.
