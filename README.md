## 📌 Project Overview

This project is an end-to-end **ERP Analytics & Data Engineering solution**. It simulates a real-world enterprise environment by populating an **Odoo ERP** instance containerized in Docker with synthetic historical data, executing a custom **Python ETL pipeline** to build a dimensional Data Warehouse (Star Schema), and delivering executive-level insights through an interactive **Power BI dashboard**.

---

## 🏗️ End-to-End Architecture & Workflow

1. **Source System (ERP):** **Odoo Community** running on **Docker** with a PostgreSQL backend as the transactional OLTP database.
2. **Data Generation Pipeline:** Custom **Python** script using `Faker`, `xmlrpc.client`, and `NumPy` to generate realistic historical enterprise data across Sales, Purchasing, and Inventory modules.
3. **ETL Process & Data Warehouse:**
   * **Extractor & Transformer:** Python pipeline (`pandas`, `SQLAlchemy`, `psycopg2`) to extract raw data from Odoo, perform data cleaning/validation, and shape it into a dimensional model.
   * **Target Storage:** Analytical Data Warehouse structured in a **Star Schema** (Fact tables: Sales, Purchases, Inventory; Dimension tables: Product, Customer, Vendor, Date).
4. **Data Analytics & Visualization (Power BI):**
   * **Sales Analytics:** Revenue trends, profit margins, and Top-N product/customer performance.
   * **Inventory & Purchasing:** Inventory turnover, stockout analysis, dead stock (slow-moving products), and vendor efficiency.
   * **Executive Overview:** High-level KPIs and business health metrics for executive decision-making.
   * **Advanced DAX & SQL:** Time Intelligence measures (YoY, YTD, MTD), dynamic margins, cumulative totals, CTEs, and Window Functions.

---

## 🛠️ Tech Stack

* **ERP Platform:** Odoo Community (Dockerized)
* **Database & Warehousing:** PostgreSQL, SQL Server
* **Programming & ETL:** Python (`pandas`, `SQLAlchemy`, `psycopg2`, `xmlrpc.client`, `Faker`)
* **Business Intelligence:** Power BI Desktop / Power BI Service (DAX, Power Query)
* **Documentation & Portfolio:** Git, GitHub
