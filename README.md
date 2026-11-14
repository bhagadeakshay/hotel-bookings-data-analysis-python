# Hotel Bookings Data Analysis

End-to-end exploratory data analysis on **Atliq Hotels** booking data (May–July 2022) using **Python, Pandas, NumPy, Matplotlib & Seaborn**.

## Project Structure

```
hotel_bookings_analysis/
├── datasets/
│   ├── fact_bookings.csv
│   ├── fact_aggregated_bookings.csv
│   ├── dim_hotels.csv
│   ├── dim_rooms.csv
│   ├── dim_date.csv
│   └── new_data_august.csv
├── Hotel_Bookings_Data_Analysis.ipynb   ← Main analysis notebook
├── requirements.txt
└── README.md
```

## How to Run

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the notebook:
   ```bash
   jupyter notebook Hotel_Bookings_Data_Analysis.ipynb
   ```

## Analysis Contents

1. **Data Loading & Exploration**
2. **Data Cleaning**
   - Invalid guest counts (`no_guests <= 0`)
   - Revenue outliers (mean + 3×std)
   - Missing capacity values
3. **Data Transformation** – Occupancy % column
4. **Insights**
   - Occupancy by room category, city, weekday/weekend
   - June occupancy by city
   - August data overview
   - Revenue by city and month
5. **Revenue Analysis** – Hotel-wise, city-wise, weekly trends
6. **Booking Analysis** – Cancellation rates, platform & room performance
7. **Occupancy Analysis** – Hotel, room class, day-wise, week-wise
8. **Advanced Metrics**
   - **ADR** – Average Daily Rate
   - **DBRN** – Day Booking Revenue per Night
   - **DSRN** – Day Sales (Capacity) per Night
   - **DURN** – Day Utilization Rate per Night

## Datasets

| File | Description |
|------|-------------|
| `fact_bookings.csv` | ~134k booking transactions |
| `fact_aggregated_bookings.csv` | Daily occupancy by property & room |
| `dim_hotels.csv` | 25 hotel properties |
| `dim_rooms.csv` | Room classes (Standard → Presidential) |
| `dim_date.csv` | Date dimension (May–July 2022) |
| `new_data_august.csv` | Sample August occupancy data |

## Tools

- Python 3
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook
