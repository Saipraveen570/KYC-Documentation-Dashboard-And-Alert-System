PBIX Build Guide - Visual Layout & Formatting
-------------------------------------------
Page & Theme
- Page size: 1400 x 900 (Format -> Page size -> Custom)
- Set background image: KYC_Compliance_Dashboard_Image.png (Fit, 0% Transparency)
- Font: Segoe UI or Arial; Title font-size ~36; Card title 14; Card value 28-32

Visuals to create (suggested positions correspond to the background layout):
1) KPI Cards (top row)
   - Total Clients (Total Clients)
   - Fully Compliant % (Fully Compliant % formatted as %)
   - Missing Docs % (Missing Docs %)
   - Expired Docs % (Expired Docs %)
   - Avg Days to Expiry (Avg Days to Expiry)

2) Donut chart - KYC Status
   - Values: count of ClientID, Legend: KYCStatus, show percentage data labels inside slices
   - Position: left-mid

3) Map / Filled Map - Clients by Region/Country
   - Location: Country, Size: count of ClientID or AssetsUnderManagement (optional)

4) Bar chart - Top Relationship Managers (Non-Compliant)
   - Axis: RelationshipManager; Value: count of ClientID filtered where KYCStatus <> 'Valid'
   - Sort descending by value

5) Line chart - Non-Compliant Trends over time
   - Axis: KYCSubmissionDate (use monthly aggregation), Value: Non-Compliant Count measure (KYCStatus <> 'Valid')
   - Smoothing: off; Stroke width 2-3

6) Drillthrough / Client Details page
   - Create a second page for drillthrough with ClientID as drillthrough field and a table with client details + history

Formatting tips:
- Card backgrounds: white with subtle shadow
- Use navy (#0B2A4A), slate gray (#6B7280), accent green (#2E8B57), warning orange (#D97706), danger red (#DC2626)
- Add bookmarks for filters like "High Risk" and "Expiring soon"

