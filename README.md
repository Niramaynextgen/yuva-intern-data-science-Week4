# yuva-intern-data-science-Week4


## Files
- `week4_eda_feature_engineering.py`: reusable starter script.
- Run it from a folder containing a `data/` directory and your CSV files.
 
## Install dependencies
```bash
python -m pip install pandas numpy matplotlib seaborn scipy
```

## Run
```bash
python week4_eda_feature_engineering.py
```

## Expected transaction columns
Required: `order_id`, `customer_id`, `order_date`, `quantity`, `unit_price`.

Optional: `product_id`, `discount_rate`, `category`, `brand`, `channel`.

`discount_rate` is expected as a decimal (0.20 = 20%). Verify the actual data definition before use. The estimated sales calculation excludes tax, shipping, returns, and currency conversion unless you add them.

## Output
The script creates `outputs/tables/` with quality audits, descriptive statistics, category performance, time trends, customer features, product features, and optional statistical-test results. It creates `outputs/plots/` with distributions, category charts, a correlation heatmap, and weekly sales trends.

## Important
This is a starter template, not a guarantee that it will run unchanged on an unknown dataset. Edit the column mapping in `COL` to match your data. Inspect flagged data-quality issues and validate all sales definitions before interpreting results. Use a time-based split and calculate features using only information available at the prediction cutoff to avoid leakage.
