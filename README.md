# r-prog-mba-data

Public data assets for the [R Programming for MBA Students](https://github.com/karrtikiyer/r-prog-mba) course.

Hosted separately from the main course repository so that notebooks can fetch data via `read_csv()` / `download.file()` from `raw.githubusercontent.com` URLs without exposing the course code itself.

## Structure

```
week5/
├── superstore_orders.csv          # cleaned Superstore (dates: DD-MM-YYYY)
├── customers_master_mirror.csv    # CSV mirror of the live Google Sheet
├── regional_targets.xlsx          # 4-sheet workbook (Q1-Q4)
├── returns/
│   └── returns_2024_01.csv ... 06.csv
└── homework/
    ├── orders_hw.csv
    ├── targets_hw.xlsx
    └── customers_hw.csv
```

## Regeneration

Data is reproducibly generated from a fixed seed. See `scripts/build_week5_data.R` in the main course repo.

## License

These data files are derived from the public Superstore dataset (a widely-used teaching dataset). The synthetic additions (regional targets, customer demographics, monthly returns) are released under the MIT license for educational use.
