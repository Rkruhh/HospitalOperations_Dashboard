
**🏥 Hospital Operations & Cost Dashboard**

From 27,891 encounters to a boardroom-ready view of volume, cost and who actually pays.

<img width="2940" height="1408" alt="image" src="https://github.com/user-attachments/assets/41d2b8b3-dd07-4691-8ed1-b03eadc9c4ce" />

**✨ Features**

An interactive, single-file dashboard for hospital executives (CEO, COO, CFO). One sticky filter bar drives every KPI, chart and insight.

**🧮 KPI cards**

Six headline metrics, each with a ▲/▼ indicator against the prior year. For cost and readmission, an increase is shown in red.

### Key Performance Indicators (KPIs)

| KPI | Definition |
| :--- | :--- |
| **Total Encounters** | Total count of medical encounters within the selection. |
| **Unique Patients** | Number of distinct patients with at least one recorded encounter. |
| **Total Claim Cost** | Cumulative sum of all `TOTAL_CLAIM_COST` entries. |
| **Payer Coverage Rate** | Ratio of the covered amount relative to the total claim cost. |
| **Avg Cost per Encounter** | Mean cost per encounter (Total Claim Cost ÷ Total Encounters). |
| **30-Day Readmission Rate** | Percentage of encounters occurring within 30 days of a patient's previous encounter. |


### 🎛️ Global Filter Bar

The dashboard includes a comprehensive filter bar to allow for granular analysis of hospital data:

| Filter | Control Type | Options |
| :--- | :--- | :--- |
| **Year** | Single-select | All, 2011–2022 |
| **Encounter Class** | Multi-select | Ambulatory, Outpatient, Urgent Care, Emergency, Wellness, Inpatient |
| **Payer** | Multi-select | 10 payers (including NO_INSURANCE) |
| **Gender** | Multi-select | Based on patient demographic data |
| **Race** | Multi-select | Based on patient demographic data |
| **Age Group** | Multi-select | 0–17, 18–39, 40–64, 65+ (based on age at encounter date) |
| **County** | Multi-select | Geographical location of patient |

### 🗂️ Data Sources

The dashboard is built upon the following datasets, covering the period from January 2011 to February 2022:

| File | Contents |
| :--- | :--- |
| `encounters.csv` | 27,891 records: dates, class, payer, reason, costs, and coverage |
| `patients.csv` | 974 patients: demographics, location, and vital status |
| `procedures.csv` | 47,701 linked procedures with associated base costs |
| `payers.csv` | 10 distinct insurance payers |
| `organizations.csv` | Massachusetts General Hospital metadata |
| `data_dictionary.csv` | Detailed column definitions |

**Dataset Summary:**
* **Total Claim Cost:** $101.5M ($31.1M covered by payers / 30.6% coverage rate)
* **Patient Demographics:** 974 total patients, including 154 deceased.
