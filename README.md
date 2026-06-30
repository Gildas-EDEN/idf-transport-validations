# Paris Region Transit Validations — Open Data Analysis

Python data-science mini-project on daily ticket validations of the Île-de-France
rail network, including an analysis of the 2024 Summer Olympics impact.

> Group project (binôme, AMSE). Contributor: Gildas Edenakpo.

## Highlights

- **Data acquisition** by script (no manual download) from Île-de-France
  Mobilités Open Data.
- **Data preparation**: understanding the validation counts encoding, fixing the
  counting strategy, identifying the main ticket categories.
- **Analysis**: traffic in a given station, weekly traffic fluctuation, and the
  impact of the **2024 Summer Olympics** on validations.
- **Modeling**: Random Forest regression with an improvement iteration.

## Dataset

| | |
|---|---|
| **Name** | Validations on the rail network — daily counts (`NB_FER`) |
| **Source** | [Île-de-France Mobilités Open Data](https://data.iledefrance-mobilites.fr) |
| **License** | Open data (Licence Ouverte / Etalab) |
| **Coverage** | Q2–Q4 2024 and Q1–Q3 2025 |

The notebook downloads each quarter directly, e.g.:

```
https://data.iledefrance-mobilites.fr/explore/dataset/validations-reseau-ferre-nombre-validations-par-jour-2eme-trimestre/download?format=csv
```

(`;` separator, `latin1` encoding.)

## Setup

```bash
python -m venv .venv && source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook
```

## Author

Gildas Edenakpo — M2 Econometrics & Data Science, Aix-Marseille School of Economics.
Group project, see note above.
