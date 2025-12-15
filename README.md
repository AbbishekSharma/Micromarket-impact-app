# Micromarket Supply Impact App (Traffic + Productivity Loss)

This Streamlit app converts your Excel model into an interactive APP.

## What it does
- Takes **new supply** (area → seats → arrivals) and converts it into **added road PCU**
- Applies the **BPR delay curve**: `t = t0 * (1 + A * (V/C)^B)`
- Produces:
  - **Extra travel minutes** (future vs current)
  - **LOS change by corridor**
  - **Daily hours lost**
  - **Productivity loss ₹/day and ₹/month** for existing occupiers

## Start
```bash
pip install -r requirements.txt
streamlit run app.py
```

## Excel template support
Upload your workbook (same format as the Cybercity model).  
The app will pre-fill values from these sheets:
- Inputs
- Capacity Vs. Actual
- Productivity Loss
