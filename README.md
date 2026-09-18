# Finansijska sloboda 360 - Web aplikacija v2

## Funkcije
- 5 jednostavnih ekrana: Danas, Moj portfolio, Novi kapital, Put do slobode, Kompetencija
- online market feed sa podesivim tickerima i rucnim fallbackom
- Gold, Brent, CSPX/S&P 500 UCITS, Energy UCITS, VIX, US 10Y i EUR/USD
- evidencija gotovine, zastitne rezerve, fizickog zlata, ETF-ova, obveznica i druge aktive
- IFS (Financial Freedom Index), IRI (Investment Readiness Index) i Competence Index
- Market Regime + Portfolio Gap + raspodjela sljedeceg kapitala
- Excel export trenutnog snapshot-a

## Lokalno pokretanje
```bash
pip install -r requirements.txt
streamlit run app.py
```

## Streamlit Community Cloud
1. GitHub repository treba da sadrzi `app.py`, `requirements.txt` i `.streamlit/config.toml`.
2. U Streamlit Community Cloud izaberite repository, branch `main` i main file `app.py`.
3. Aplikacija ne zahtijeva secrets za osnovni market feed preko yfinance.
4. Za buduce placene/licencirane feedove API kljuceve drzati u Streamlit Secrets, nikada u GitHub kodu.

## Napomena
Market feed je informativan i moze kasniti ili privremeno biti nedostupan. Aplikacija nije automatizovani broker niti izvršava transakcije; sluzi kao decision-support sistem.
