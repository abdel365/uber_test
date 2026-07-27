# Render sample Streamlit app (Jedha Launch)

Slim Uber pickups demo for Render Free (512 MB). Local 5k-row CSV. No pydeck.

## Files

- `app.py` — hour slider, `st.map`, Altair chart
- `data/uber_pickups_sample.csv` — 5000 rows
- `.streamlit/config.toml` — headless + `0.0.0.0`
- `Dockerfile` / `requirements.txt`

## Push + deploy

See `../MANUAL_DEPLOY_RUNBOOK.md` (one level up from `phase0-samples`, in `D06-Launch`).

Full path:

`AIFS/.changelogs/M08-ML_Engineering/D06-Launch/MANUAL_DEPLOY_RUNBOOK.md`

## Local (no Docker)

```bash
pip install -r requirements.txt
streamlit run app.py --server.port=10000 --server.address=0.0.0.0
```
