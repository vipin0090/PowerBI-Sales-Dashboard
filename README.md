🛒 E-Commerce Sales Dashboard — Power BI
An interactive Power BI dashboard that analyzes e-commerce sales performance across Indian states for the year 2018. It provides a 360° view of revenue, profitability, quantity sold, customer behavior, and payment trends — all in a single-page dark-themed report.

📁 Project Structure
e-commerce sales_dashboard/
│
├── datasets/
│   ├── Details.csv        # 1,500 order line-items (amount, profit, category, payment)
│   └── Orders.xlsx        # 500 orders (date, customer, state, city)
│
├── Sales_Dashboard.pbix   # Power BI report file
└── Sales_Dashboard.png    # Dashboard screenshot

📊 Key Metrics (KPI Cards)
MetricValueSum of Amount₹ 438KSum of Profit₹ 37KSum of Quantity5,615 unitsSum of AOV (Avg. Order Value)₹ 121K

📈 Visuals in the Report
VisualTypeInsightSum of Amount by StateHorizontal Bar ChartMaharashtra leads in revenue, followed by Madhya Pradesh and Uttar PradeshSum of Quantity by CategoryDonut ChartClothing dominates at 63%, Electronics 21%, Furniture 17%Sum of Profit by MonthBar ChartPeak profits in January–March; losses in July–August & DecemberSum of Amount by CustomerNameBar ChartTop customers: Harivansh, Madhav, Madan Mohan, Shiva, VishakhaSum of Quantity by PaymentModeDonut ChartCOD is most preferred (44%), followed by UPI (21%)Sum of Profit by Sub-CategoryBar ChartPrinters and Bookcases are the most profitable sub-categories

🗂️ Dataset Details
datasets/Details.csv — 1,500 rows
ColumnDescriptionOrder IDUnique order identifier (e.g., B-25681)AmountRevenue generated per order line (₹ 4 – ₹ 5,729)ProfitProfit earned per order lineQuantityNumber of units soldCategoryProduct category: Electronics, Furniture, ClothingSub-Category17 sub-categories (Printers, Chairs, Saree, Phones, etc.)PaymentModePayment method: COD, UPI, Debit Card, Credit Card, EMI
datasets/Orders.xlsx — 500 rows
ColumnDescriptionOrder IDUnique order identifier (links to Details.csv)Order DateDate of order (Jan 2018 – Dec 2018)CustomerNameName of the customerStateIndian state (19 states covered)CityCity of delivery

Relationship: Orders[Order ID] → Details[Order ID] (One-to-Many)


🛠️ Tools & Technologies

Power BI Desktop — Report building, DAX measures, data modelling
Microsoft Excel / CSV — Source data files
DAX — Calculated measures (AOV, total profit, monthly aggregations)


🚀 How to Open the Dashboard

Download and install Power BI Desktop (free).
Clone or download this repository.
Open Sales_Dashboard.pbix in Power BI Desktop.
The datasets are embedded in the .pbix file — no additional setup needed.


Note: If the data source paths break, go to Home → Transform Data → Data Source Settings and re-point to the datasets/ folder.


💡 Key Insights

Clothing is the highest-selling category by volume (63%), but Electronics sub-categories like Printers drive the most profit.
COD (Cash on Delivery) remains the most used payment mode at 44%, suggesting a trust gap in digital payments among the customer base.
Maharashtra generates the highest revenue among all states.
Profits dip sharply in mid-year (July–August), which could indicate a seasonal slowdown or higher return rates.
Q1 (Jan–Mar) is consistently the strongest quarter for profitability.


📌 Use Cases

Sales performance monitoring
Regional revenue analysis
Customer segmentation
Payment mode trend analysis
Product category profitability review


🙌 Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

📄 License
This project is open-source and available under the MIT License.
