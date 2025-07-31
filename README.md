
🏙️ Airbnb Listings EDA Project: New York 2024

📌 Project Overview

This project performs **Exploratory Data Analysis (EDA)** on Airbnb listings in New York City. Using libraries like **Pandas, NumPy, Matplotlib, and Seaborn**, the project uncovers trends and patterns related to prices, room types, host behavior, and availability.


🎯 Objective

The main goals of this project are to:

* Analyze **room types**, **prices**, and **availability** across different neighborhoods.
* Understand **host behavior** and **listing patterns**.
* Detect potential **outliers in prices**.
* Provide **recommendations** for guests and hosts based on the insights.


📂 Dataset Summary

Entries: 20,765
Features: 22
Key Columns:

`id`: Unique listing identifier
`name`: Listing title
`host_name`: Host’s name
`neighborhood_group`: NYC borough (e.g., Manhattan, Brooklyn)
`latitude/longitude`: Geolocation
`price`: Nightly rental price
`room_type`: Type of accommodation (e.g., Entire home, Private room)
`reviews_per_month`: Average monthly reviews
`availability_365`: Days available in a year

---

🧹 Steps and Workflow

1. 🔧 Data Cleaning

Handled Missing Values in `price`, `neighborhood`, and `beds`.
Fixed Data Types: Converted `last_review` to `datetime`.
Removed Outliers: Capped prices > **\$1,000** to prevent skewed visuals.

2. 📊 Exploratory Data Analysis (EDA)

🛏️ Room Type Distribution

Bar plots showed `Entire home/apt` is the most common.

🗺️ Neighborhood Insights

Manhattan had the highest average prices.

📆 Availability Trends

Heatmaps revealed correlations between `price`, `availability_365`, `reviews`, and `beds`.

💰 Price Distribution

 Histograms showed most listings priced between **\$50–\$300**.

👤 Host Listings

* Boxplots identified hosts with **multiple listings**, hinting at professional hosting.

✍️ Review Behavior

* Pair plots used to explore relationships between:

  * `number_of_reviews`
  * `price`
  * `availability_365`



📈 Data Visualization Tools Used

* **Pairplot** – For multi-variable correlation.
* **Heatmap** – For numerical feature correlation.
* **Histograms & Boxplots** – For price outlier detection.
* **Bar Charts** – For room type & neighborhood distribution.

---

🔍 Key Findings and Insights

💸 Price Trends

* **Manhattan** is the most expensive borough.
* **Entire homes/apartments** cost significantly more than other room types.

🛌 Room Type Distribution

* `Entire home/apt` listings dominate.
* `Private rooms` offer affordable alternatives.

🚨 Price Outliers

* Listings over **\$10,000+** were detected and filtered.

📅 Availability Patterns

* Higher availability = lower prices + more reviews → better guest experience.

🧑‍💼 Host Behavior

* Some hosts manage **multiple listings**, suggesting **professional hosting**.


▶️ How to Run This Project

1. Clone the repository:

   ```bash
   git clone https://github.com/najirh/Python-Project-P2-New-York-AirBnb-Listing-2024.git
   ```

2. Install dependencies:

   ```bash
   pip install pandas numpy matplotlib seaborn
   ```

3. Run the Jupyter Notebook:

   ```bash
   jupyter notebook day23_airbnb_eda.ipynb
   ```


✅ Recommendations

For Guests:

* Choose listings with **high availability** and **good reviews**.
* **Private rooms in Brooklyn** provide affordable options vs. Manhattan.

For Hosts:

* Increase **availability** and **respond to reviews** promptly.
* Use **competitive pricing** to stand out within your neighborhood.


🔮 Future Work

* Build a **machine learning model** to predict prices based on room type and location.
* Apply **sentiment analysis** to listing reviews for better guest feedback insights.
* Create an **interactive dashboard** using **Plotly or Tableau** for live data monitoring.


 🏁 Conclusion

This project provides actionable insights into the New York Airbnb market. By using EDA techniques, we discovered patterns in pricing, room types, host activity, and availability that benefit both **guests** and **hosts**. Future enhancements can include **predictive modeling** and **interactive tools** to further increase value and usability.


