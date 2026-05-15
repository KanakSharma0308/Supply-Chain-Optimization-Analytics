Supply Chain Analytics: Inventory Optimization & Demand Forecasting
📌Project OverviewThis project focuses on optimizing supply chain efficiency for an FMCG-centric dataset. By leveraging statistical modeling and data analytics, I addressed the core challenges of inventory management: demand unpredictability, stockout risks, and inventory carrying costs.The analysis transforms raw transactional data into actionable insights, helping businesses maintain a high service level while minimizing capital tied up in inventory.
📊 Key Analytical 
Modules1. Inventory Segmentation (ABC Analysis)Using the Pareto Principle (80/20 Rule), I categorized over 100 SKUs based on their revenue contribution to prioritize management focus.Category A: High-value items contributing to ~80% of total revenue ($6.9M+ from top performers like Field & Stream Sportsman).Category B: Moderate impact items.Category C: Low-value, high-volume items.Impact: Enabled a targeted inventory strategy where "A" items are monitored with high precision to prevent revenue loss.
2. Demand Forecasting (Exponential Smoothing)Implemented a Time-Series Forecasting model to predict quarterly demand patterns.Methodology: Simple Exponential Smoothing with a smoothing constant $\alpha = 0.2$.Evaluation: Calculated MAPE (Mean Absolute Percentage Error) and squared errors to validate forecast reliability against actual demand.Insight: Identified seasonal spikes and reduced the "Bullwhip Effect" by aligning procurement with predicted sales.
3. Risk-Based Inventory Policy (ROP & Safety Stock)Developed a dynamic reordering system to mitigate supply chain uncertainties.Lead Time Analysis: Analyzed historical shipping data to determine a standard deviation in lead time of 1.45 days.Safety Stock: Calculated buffer stock to protect against demand variability.Reorder Point (ROP): Established a threshold of ~1197 units for key products to trigger automated replenishment.Formula:$$ROP = (Average Daily Demand \times Lead Time) + Safety Stock$$
🛠️ Tech Stack & ToolsAdvanced Excel:
Pivot Tables, Statistical Functions, Solver.Data Analytic: Interactive dashboards for SKU performance tracking.
📈 Business Impact for FMCG (Mondelez Context)Service Level Optimization: Ensures that high-demand products (like Cadbury/Oreo equivalents) are always available.Cost Reduction: Minimizes excess stock of 'Category C' items, freeing up warehouse space and working capital.Data-Driven Decisions: Replaces gut-feeling ordering with statistical reorder triggers.
📂 Repository StructurePlaintext├── Data/
│   ├── ABC_Analysis_EOQ.csv
│   ├── Demand_Forecasting.csv
│   └── Reorder_Point_Calculations.csv
├── README.md
