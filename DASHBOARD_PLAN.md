# Apple Stock (AAPL) Dashboard Plan

## Overview
Build an interactive Streamlit dashboard to analyze Apple stock historical data from 1980-2023.

## Data Source
- **File:** `D:\Data analyst price stock\Apple price stock\AAPL_cleaned.csv`
- **Columns:** Date, Open, High, Low, Close, Adj Close, Volume
- **Records:** ~10,835 trading days

## Dashboard Structure

### 1. Main Page - Overview
- **Title:** Apple (AAPL) Stock Dashboard
- **Sidebar:**
  - Date range selector
  - Chart type selector
  - Moving average periods

### 2. Charts to Include
| # | Chart | Description |
|---|-------|-------------|
| 1 | Closing Price | Time series of close price over time |
| 2 | Open vs Close | Comparison line chart of both |
| 3 | High/Low Range | High & low with shaded range (volatility) |
| 4 | Volume | Trading volume bar chart |
| 5 | Moving Averages | Close price with 50-day & 200-day MA |

### 3. Key Metrics Display
- Current Price
- Price Change (daily/weekly)
- 52-week High/Low
- Average Volume
- Market Cap proxy

### 4. Interactive Features
- Date range filter (slider/selector)
- Zoom & pan on charts
- Tooltips with values
- Export data option

## Technical Stack
- **Framework:** Streamlit
- **Plotting:** Plotly (interactive) or Matplotlib
- **Data Processing:** Pandas
- **Run Command:** `streamlit run app.py`

## File Structure
```
Apple price stock/
├── AAPL_cleaned.csv
├── app.py              # Main dashboard
├── requirements.txt
└── assets/
    └── charts/
```

## Next Steps
1. Create `requirements.txt`
2. Build `app.py` with all visualizations
3. Test locally with `streamlit run app.py`
4. Deploy to Streamlit Cloud (optional)