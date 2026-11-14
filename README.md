# Hotel Bookings Data Analysis

End-to-end **Exploratory Data Analysis (EDA)** on Atliq Hotels booking data (May–July 2022) using **Python, Pandas, NumPy, Matplotlib & Seaborn**.

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.x-11557c)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12-4C72B0)

---

## 📌 Project Overview

Atliq Hotels operates across **Delhi, Mumbai, Bangalore, and Hyderabad** with Luxury and Business properties.  
This project analyzes ~134,000 booking transactions and daily occupancy data to answer key business questions on:

- Occupancy rates
- Revenue performance
- Cancellations & no-shows
- Platform effectiveness
- Advanced hotel metrics (ADR, DBRN, DSRN, DURN)

---

## 📁 Project Structure

```
hotel-bookings-data-analysis/
│
├── datasets/
│   ├── fact_bookings.csv              # ~134k booking transactions
│   ├── fact_aggregated_bookings.csv   # Daily occupancy metrics
│   ├── dim_hotels.csv                 # Hotel properties (25)
│   ├── dim_rooms.csv                  # Room classes (RT1–RT4)
│   ├── dim_date.csv                   # Date dimension (May–Jul 2022)
│   └── new_data_august.csv            # Sample August data
│
├── Hotel_Bookings_Data_Analysis.ipynb # Main analysis notebook
├── requirements.txt
└── README.md
```

---

## 🛠️ Technologies Used

| Tool | Purpose |
|------|---------|
| **Python 3** | Core language |
| **Pandas** | Data loading, cleaning, aggregation |
| **NumPy** | Numerical operations |
| **Matplotlib** | Charts & trends |
| **Seaborn** | Statistical visualizations |
| **Jupyter Notebook** | Interactive analysis |

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/hotel-bookings-data-analysis.git
   cd hotel-bookings-data-analysis
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Open the notebook**
   ```bash
   jupyter notebook Hotel_Bookings_Data_Analysis.ipynb
   ```

---

## 📊 Analysis Contents

### 1. Data Loading & Exploration
- Shape, columns, unique values, distributions

### 2. Data Cleaning
- Removed invalid guest counts (`no_guests <= 0`)
- Removed revenue outliers (mean + 3×std)
- Filled missing capacity with median

### 3. Data Transformation
- Created **Occupancy %** column

### 4. Insights Generated
| # | Question |
|---|----------|
| 1 | Average occupancy by room category |
| 2 | Occupancy rate by city |
| 3 | Weekday vs Weekend occupancy |
| 4 | June occupancy by city |
| 5 | Append & review August data |
| 6 | Revenue realized per city |
| 7 | Month-by-month revenue |

### 5. Revenue Analysis
- Hotel-wise revenue
- City-wise revenue
- Weekly revenue trends

### 6. Booking Analysis
- Cancellation / Checkout / No-Show % by hotel
- Platform-wise bookings
- Room category-wise bookings & revenue

### 7. Occupancy Analysis
- Hotel-wise occupancy
- Room class-wise occupancy
- Day-wise & week-wise occupancy

### 8. Advanced Metrics
| Metric | Full Form | Formula |
|--------|-----------|---------|
| **ADR** | Average Daily Rate | Revenue ÷ Bookings |
| **DBRN** | Day Booking Revenue per Night | Checked-out bookings ÷ Total days |
| **DSRN** | Day Sales (Capacity) per Night | Total capacity ÷ Total days |
| **DURN** | Day Utilization Rate per Night | Checked-out bookings ÷ Total days |

---

## 📈 Key Insights (Summary)

- Clear differences in occupancy across cities and room classes
- Weekend vs weekday occupancy patterns identified
- Top-performing hotels and cities by revenue highlighted
- Platform-wise volume and cancellation behaviour analyzed
- ADR, DBRN, DSRN, DURN calculated for hotel comparison

---

## 📦 Datasets

| File | Rows (approx) | Description |
|------|---------------|-------------|
| `fact_bookings.csv` | 134,590 | Transaction-level bookings |
| `fact_aggregated_bookings.csv` | 9,200 | Daily successful bookings & capacity |
| `dim_hotels.csv` | 25 | Property master |
| `dim_rooms.csv` | 4 | Room classes |
| `dim_date.csv` | 92 | Date attributes |
| `new_data_august.csv` | 7 | August sample |

---

## ✍️ Author

**Your Name**  
Data Analysis Project | Hospitality Domain

---

## 📄 License

This project is for educational / portfolio purposes.
