# Urban Mobility & Economic Productivity Analysis 🚗📉

![Traffic vs GDP](https://vuestra-imagen-o-grafico-aqui.png) ## 📝 Context
This project investigates the relationship between traffic congestion and GDP per capita across major global cities in 2024. The goal was to determine if time lost in traffic acts as a measurable brake on economic growth by integrating TomTom mobility data with OECD macroeconomic indicators.

## 🛠 Methodology

### Technical Stack
- **Language:** Python
- **Libraries:** Pandas (Data Cleaning), NumPy, Matplotlib/Seaborn (Visualization).
- **Process:** Data integration from multiple sources, normalization of travel time metrics, and correlation analysis.

### Executive Overview of the Process
The analysis was structured into a three-stage technical workflow:
1. **Data Engineering:** I performed an extensive cleaning process, standardizing city names and date formats to ensure consistency. A key step was the **Inner Join** integration between mobility datasets (Jams/Traffic) and economic datasets (GDP), ensuring only validated records were used.
2. **Advanced Processing:** To eliminate seasonal "noise" and daily fluctuations, I applied city-year aggregations using annual averages. This provided a stable baseline for comparing long-term economic trends.
3. **Comparative Analysis & Normalization:** Recognizing that GDP and traffic indices operate on vastly different numerical scales, I applied **data normalization**. This was crucial to prevent the GDP figures from "eclipsing" the traffic data, allowing for a truthful visual comparison of regional efficiency.

### 📊 Findings (Key Insights)
The patterns detected break the idea of a simple linear correlation:
- **The "Eclipsing" Effect:** In unnormalized charts, GDP per capita (measured in tens of thousands) completely "eclipses" the traffic index (measured in hundreds), leading to deceptive decision-making.
- **Saturation in CDMX:** The normalized chart reveals that **Mexico City** has reached a point of total saturation, where traffic levels practically equal its GDP.
- **The Santiago Anomaly:** **Santiago de Chile** is the most critical case in the region. It is the only city where the congestion index (blue bar) visually surpasses the productivity level (orange bar), representing a massive regional inefficiency.
- **Efficient Models:** Cities like **Buenos Aires and Brasilia** demonstrate a healthy gap where the economy dominates over congestion, showing that growth is possible without total mobility collapse.
  
![Visualización de Resultados](nombre_de_tu_imagen.png)

## 💡 Business Recommendations
- **Infrastructure Prioritization:** Investment should shift towards mass transit systems in high-density areas to unlock economic potential currently lost in traffic.
- **Logistics Optimization:** Companies should use data-driven routing to mitigate the "congestion tax" on their operations.
