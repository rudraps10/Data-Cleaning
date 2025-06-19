# 🧹 Amazon Product Dataset Cleaning

## 🚀 Objective
Clean and preprocess Amazon product data to prepare it for analytics, visualization, or machine learning.

---

## 🔧 Cleaning Steps Performed
- Removed `$` sign and converted `product_original_price` to float.
- Filled missing values in `product_original_price` and `product_star_rating` using median/mean.
- Normalized `sales_volume` values (handled "2K+", etc.).
- Extracted useful features from `delivery` column:
  - `is_free_delivery`
  - `is_available_instantly`
  - `delivery_date` (like “June 21”)
- Dropped irrelevant or mostly null columns:
  - `unit_count`, `unit_price`, `product_availability`
- Dropped duplicate rows to ensure clean data.

---

## 📁 Files in This Project
| File | Description |
|------|-------------|
| `amazon_product.csv` | Raw input dataset |
| `amazon_cleaned.csv` | Final cleaned dataset |
| `amazon_cleaning.py` | Python script that does the full cleaning |
| `requirements.txt` | Python libraries used |

---

## 📦 How to Run
Make sure the input CSV file (`amazon_product.csv`) is present in the same folder.

```bash
python amazon_cleaning.py
