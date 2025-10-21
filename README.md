# KYC Compliance Dashboard - Power BI Project (v2)

This repository contains everything needed to recreate the **KYC Compliance Dashboard** in Power BI:
- Dataset (CSV) to import directly into Power BI
- Dashboard background image used for layout
- Power Query (M) script and DAX measures
- PBIX build guide and Power BI theme JSON (colors/fonts)
- Risk scoring & data logic documentation

## Files
- `kyc_clients_dataset.csv` - 2000 synthetic client records (realistic distribution, safe for demos)
- `KYC_Compliance_Dashboard_Image.png` - dashboard visual background image
- `PowerBI_Instructions.txt` - M & DAX + step-by-step import instructions
- `pbix_build_guide.md` - visual placement & formatting guide
- `KYC_Theme.json` - Power BI theme matching the dashboard look
- `risk_logic_documentation.txt` - explains risk rating derivation
- `LICENSE` - MIT license

## How to use
1. Open **Power BI Desktop**.
2. `Home -> Get Data -> Text/CSV` and select `kyc_clients_dataset.csv`.
3. Use `PowerBI_Instructions.txt` to paste the Power Query M script into Advanced Editor.
4. Create the DAX measures and visuals using the `pbix_build_guide.md` guidance.
5. Use `KYC_Compliance_Dashboard_Image.png` as Background (Format -> Page background) or insert as Image and Send to Back.
6. Save the report as `.pbix` and publish to Power BI Service or upload the files to GitHub.

