# nebpmJudy Monthly Process Verification

- [ ] **1. BQ Pre-Scrape:** Verify the [tags: only_BQ_data Dataform jobs](https://console.cloud.google.com/bigquery/dataform/locations/us-central1/repositories/nebpm-monthly-report/workspaces/dataform-test/actions?inv=1&invt=Ab4rwA&project=bigquery-bonafide-bonanza) completed successfully.
- [ ] **2. Website Scrape:** Confirm the [scrape & create data action](https://github.com/UniversityofNebraskaNET/nebpmMonthlyReport/blob/main/.github/workflows/scrape_website.yaml) ran successfully.
  - [ ] Check if the Claude Model is still available. Claude's model choice is hardcoded in the classification script. 
- [ ] **3. BQ Post-Scrape Join:** Verify the [tags: wait_for_GH_actions Dataform jobs](https://console.cloud.google.com/bigquery/dataform/locations/us-central1/repositories/nebpm-monthly-report/workspaces/dataform-test/actions?inv=1&invt=Ab4rwA&project=bigquery-bonafide-bonanza) completed successfully.
- [ ] **4. Final Data Test:** Confirm the [Judy data Test](https://github.com/UniversityofNebraskaNET/nebpmMonthlyReport/blob/main/.github/workflows/test_judy_data.yaml) passed.
- [ ] **5. Check if the website running fine**: Visit the [Judy website](https://nebraskapublicmedia.shinyapps.io/nebpmJudy/) and ensure no duplicate data or missing data.

## nebpmDigit Process Verification

### Monthly Check

- [ ] **Monthly Data:** Verify the [tags: monthly_run Dataform job](https://console.cloud.google.com/bigquery/dataform/locations/us-central1/repositories/nebpmDigit/workspaces/dataform-test/actions?inv=1&invt=Ab4rwA&project=bigquery-bonafide-bonanza) completed successfully.

### Daily Checks

- [ ] **1. Daily Data:** Verify the [tags: daily_run Dataform job](https://console.cloud.google.com/bigquery/dataform/locations/us-central1/repositories/nebpmDigit/workspaces/dataform-test/actions?inv=1&invt=Ab4rwA&project=bigquery-bonafide-bonanza) completed successfully.
- [ ] **2. Forecasting:** Confirm the [forecasting pipeline action](https://github.com/UniversityofNebraskaNET/nebpmDigit/blob/main/.github/workflows/forecasting_pipeline.yaml) ran successfully.

### General Checks

- [ ] **1. Check if the website running fine**: Visit the [Digit website](https://nebraskapublicmedia.shinyapps.io/nebpmDigit/) and ensure no duplicate data or missing data.