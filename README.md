# 🧹 Amazon Product Dataset Cleaning

## 🚀 Objective
Clean and preprocess Amazon product data to prepare it for analytics or machine learning.

---

## 🔧 Cleaning Steps
- Removed `$` sign and converted `product_original_price` to float.
- Handled missing values in price and star ratings.
- Normalized `sales_volume` (handled values like "2K+", etc.)
- Extracted:
  - `is_free_delivery`
  - `is_available_instantly`
  - `delivery_date` (e.g., "June 21")
- Dropped irrelevant or mostly-null columns like `unit_count`, `unit_price`.

---

## 📁 Files
- `amazon_product.csv` – Raw data (or a sample)
- `amazon_cleaning.py` – Cleaning script
- `amazon_cleaned.csv` – Final cleaned output (optional)
- `requirements.txt` – Python dependencies

---

## 🛠 How To Run
```bash
python amazon_cleaning.py



~By Rudra Pratap Singh ~ Aspiring AI engineer
