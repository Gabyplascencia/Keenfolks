
# 🚀 How to Open and Explore the Project

To explore this Power BI project on your local machine, follow these steps:

---

### ✅ Requirements

- **Power BI Desktop**  
  You can download it here: [https://powerbi.microsoft.com/desktop](https://powerbi.microsoft.com/desktop)

- **Sample data** (included in `/data/` folder or embedded in the `.pbix` file)

---

### 📂 File Structure

```
/data/
    client_data.xlsx
    transactions_data.xlsx

/dashboard/
    keenfolks_dashboard.pbix

/code/
    dax_calculations.md

README.md
```

---

### 🧭 Steps to Open the Dashboard

1. **Download or clone** this repository:
```bash
git clone https://github.com/Gabyplascencia/Reto-Keenfolks.git
```

2. Open **Power BI Desktop**.

3. Go to **File > Open** and select:
```
/dashboard/keenfolks_dashboard.pbix
```

4. If prompted, **refresh the data** or relink the Excel files found in `/data/`.

5. Explore the **report tabs, filters, and KPIs** built for client performance analysis.

---

### 💡 Tips

- You can view or modify all DAX calculations in the **Model > Measures** section.
- Visualizations are grouped by **performance, revenue, ROI, and retention**.
- Use the filters on the left side to segment clients or campaigns dynamically.
