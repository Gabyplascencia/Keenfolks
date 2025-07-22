
# 📌 DAX Measures – Keenfolks Dashboard

## 1. Total Revenue
```dax
Total Revenue = SUM('Transactions'[Revenue])
```

## 2. Total Cost
```dax
Total Cost = SUM('Transactions'[Cost])
```

## 3. Gross Margin
```dax
Gross Margin = [Total Revenue] - [Total Cost]
```

## 4. Gross Margin %
```dax
Gross Margin % = DIVIDE([Gross Margin], [Total Revenue], 0)
```

## 5. ROI
```dax
ROI = DIVIDE(([Total Revenue] - [Total Cost]), [Total Cost], 0)
```

## 6. Client Lifetime Value
```dax
CLV = AVERAGEX(VALUES('Clients'[Client ID]), [Total Revenue])
```

## 7. Monthly Retention Rate
```dax
Retention Rate = 
VAR TotalClientsPrevMonth = CALCULATE(DISTINCTCOUNT('Clients'[Client ID]), PREVIOUSMONTH('Date'[Date]))
VAR TotalClientsThisMonth = CALCULATE(DISTINCTCOUNT('Clients'[Client ID]), 'Date'[Month] = MONTH(TODAY()))
RETURN DIVIDE(TotalClientsThisMonth, TotalClientsPrevMonth, 0)
```

## 8. Top Clients by Revenue
*This insight was created using a visual table with a descending sort on Total Revenue.*
