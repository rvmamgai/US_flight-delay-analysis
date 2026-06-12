# US_flight-delay-analysis
US Flight Delay Analysis 2015 | SQL + Power BI | 5.8M rows

# ✈️ US Flight Delay Analysis 2015

## 📌 Project Overview
An end-to-end data analysis project analyzing **5.82 million US domestic flights** 
from 2015 to identify delay patterns, cancellation trends, and airline/airport performance.

## 🛠️ Tech Stack
- **Database:** MySQL 8.0
- **Data Processing:** Python (Pandas, mysql-connector)
- **Visualization:** Power BI Desktop
- **Dataset:** [US Flight Delays 2015 - Kaggle](https://www.kaggle.com/datasets/usdot/flight-delays)

## 📊 Dashboard Preview
![Overview Page]()
### Overview
![Overview](report/Screenshot (371).png)

### Airline Performance  
![Airline](report/Screenshot (372).png)

### Airport Performance
![Airport](report/Screenshot (373).png)

### Misc & Summary
![Misc & Summary](report/Screenshot (374).png)

### Key Findings
![Key Findings](report/Screenshot (375).png)
!(US_flight-delay-analysis/report
/Screenshot (371).png)

## 🔑 Key Findings
- **5.82M flights** analyzed with **82.41% On-Time Performance (OTP)**
- **Late Aircraft delays** are the biggest contributor at **39.84%** of all delays
- **Weather** causes only 4.95% of delay minutes but **54.38% of cancellations**
- **Hawaiian Airlines** has best OTP at **89.50%**; Spirit Airlines worst at **72%**
- **Chicago O'Hare** has highest avg departure delay at **14.1 minutes**
- **Night flights (18-20h)** have 5x more delays than early morning flights

## 📁 Repository Structure
├── README.md

├── data/

│   └── data_source.md        # Dataset info and download link

├── sql_queries/

│   ├── 01_create_table   # Table creation

│   ├── 02_data_cleaning  # Data cleaning & preparation

│   ├── 03_eda_queries    # EDA & KPI queries

│   └── 04_views          # Analytical view

├── python/

│   ├── generate_table.py     # Auto-generate CREATE TABLE from CSV

│   └── fix_cancellation.py   # Fix cancellation reason codes

├── powerbi/

│   └── flight_analysis.pbix  # Power BI dashboard file

└── report/

└── Flight_Analysis_Report.pdf

## 🚀 How to Run
1. Download dataset from Kaggle (link in data/data_source.md)
2. Run `python/generate_table.py` to create the table structure
3. Import CSV using MySQL CLI with `--local-infile=1`
4. Run SQL files in order (01 → 02 → 03 → 04)
5. Open `powerbi/flight_analysis.pbix` and update MySQL connection

## 📈 Dashboard Pages
| Page | Description |
|------|-------------|
| Overview | KPI cards, cancellation reasons, delay breakdown |
| Airline Performance | OTP, delays, cancellations by airline |
| Airport Performance | Map, busiest/most delayed airports |
| Temporal Trends | Monthly, daily, hourly patterns |

## 💡 Recommendations
1. **Airlines** — Reduce late aircraft turnaround at hub airports to cut 39.84% cascade delays
2. **Airports** — Optimize ground operations at Chicago O'Hare (14.1 min avg delay)
3. **Passengers** — Book early morning flights (3 min avg delay vs 15 min for night flights)

## 👤 Author
**RAvi Mamgai**  
[LinkedIn](linkedin.com/in/ravi-mamgai) | [GitHub](github.com/rvmamgai)
