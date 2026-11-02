# 🚚 Supply Chain & Inventory Performance Dashboard

An enterprise-grade **Supply Chain Intelligence Dashboard** built with Microsoft Power BI, providing end-to-end operational visibility across procurement, manufacturing production, inventory balance, and logistics fulfillment.

---

## 📸 Dashboard Previews

### Inventory & Stock Health
![Supply Chain Inventory](./inventory.png)

---

## 📌 Business Problem & Objectives
Modern supply chain operations require unified visibility across fragmented data points. This project integrates:
1. **Procurement Timelines:** Supplier lead times, on-time delivery rates, and vendor purchase costs.
2. **Production Tracking:** Facility capacity utilization, production batch cycles, and yield output.
3. **Inventory Management:** Stock turnover ratio, safety stock compliance, and stockout risk mitigation.
4. **Logistics & Shipment:** On-time in-full (OTIF) shipping performance and customer order cycle duration.

---

## 🏗️ Data Architecture & Star Schema
The model connects granular transactional facts to shared enterprise dimensions:
- **Fact Tables:**
  - `fact_procurement.csv`: Supplier orders and fulfillment metrics.
  - `fact_production.csv`: Manufacturing runs and facility outputs.
  - `fact_inventory.csv`: Warehouse stock balances and reorder thresholds.
  - `fact_sales.csv`: Customer orders and sales transactions.
  - `fact_shipment.csv`: Carrier delivery and logistics records.
- **Dimension Tables:**
  - `dim_supplier.csv`, `dim_facility.csv`, `dim_product.csv`, `dim_customer.csv`, `dim_date.csv`.

---

## 🛠️ Tech Stack
- **Microsoft Power BI Desktop:** Interactive multi-view dashboard (`SupplyChainSales.pbix`).
- **DAX Calculations:** Dynamic inventory turnover, OTIF percentages, delivery lead time averages.
- **Data Modeling:** Multi-fact Star Schema with unidirectional one-to-many relationships.

---

## 📁 Repository Structure
```
├── SupplyChainSales.pbix        # Interactive Power BI report file
├── inventory.png                # Dashboard screenshot preview
├── project .docx                # In-depth project documentation & metrics definitions
├── dataset/                     # Normalized dimensional schema CSV files
│   ├── dim_customer.csv
│   ├── dim_date.csv
│   ├── dim_facility.csv
│   ├── dim_product.csv
│   ├── dim_supplier.csv
│   ├── fact_inventory.csv
│   ├── fact_procurement.csv
│   ├── fact_production.csv
│   ├── fact_sales.csv
│   └── fact_shipment.csv
└── README.md                    # Project documentation
```

---

## 🚀 How to Open
1. Clone the repository:
   ```bash
   git clone https://github.com/MianSabooh/Supply-Chain-Performance-Dashboard.git
   ```
2. Open `SupplyChainSales.pbix` in Power BI Desktop to explore all pages and visual filters.
