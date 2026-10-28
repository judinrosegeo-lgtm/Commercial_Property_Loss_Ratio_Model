# Commercial Property Loss Ratio Model (Canada, 2011–2022)

An Excel model that calculates and tracks the loss ratio for Canadian commercial property insurance from public industry data, checks it against published figures, and shows the reserving step with chain-ladder and Bornhuetter-Ferguson methods.

Every result in the workbook is a live formula. Change an assumption and the whole model recalculates.

## Key results

| Metric | Result |
|---|---|
| Long-run loss ratio, 2011–2022 | **62.6%** (about 37 cents of each premium dollar left for expenses and profit) |
| Worst year | **2016: 82.2%** (Fort McMurray wildfire) |
| Second-worst year | **2013: 75.3%** (Alberta and Toronto floods) |
| Recent years | **45.3%** (2021), **50.0%** (2022), after the price increases from 2019 onward |
| Validation | Within **1.5 pts** on average of loss ratios published by IBC and PACICC |
| Reserving (simulated triangles) | Three methods estimate ultimate losses of **$48.7bn–$49.1bn**, within 1% of the true figure |

## What's in the workbook

| Sheet | Purpose |
|---|---|
| `README` | Model overview, data source and core formula |
| `Inputs` | Assumptions (earning fraction, ULAE load, target loss ratio) and the IBC data |
| `LR_Model` | Calendar-year earned and written loss ratios against a 65% target |
| `Line_Comparison_2022` | Commercial property compared with auto, personal property, liability and other lines, direct and net of reinsurance |
| `Benchmarks` | Model results compared with loss ratios published by IBC and PACICC |
| `Calculator` | Loss ratio calculator for your own book of business |
| `Triangle_Data` | Paid and reported loss development triangles (**simulated**, see below) |
| `Chain_Ladder` | Age-to-age factors, a choice of four LDF averaging methods, tail factors and CDFs |
| `Reserve_Summary` | Ultimate losses and IBNR by paid CL, reported CL and Bornhuetter-Ferguson |
| `Queries` | Plain-English answers to common questions about the method |

**Core formula:** Loss Ratio = (Net Claims Incurred + ULAE) / Net Earned Premium

## Data sources

- **Model input:** Insurance Bureau of Canada, *Facts of the Property and Casualty Insurance Industry in Canada 2023*, Section 1, pp. 9 and 11 (data from IBC, MSA Research, SCOR and the AMF). [ibc.ca/industry-resources/resources-data/facts-book](https://ibc.ca/industry-resources/resources-data/facts-book)
- **Validation only:** published loss ratios from IBC (via Canadian Underwriter, 2014) and PACICC (via Canadian Underwriter, 2022)

The data covers private insurers only and is net of reinsurance, in $ millions CAD. The model stops at 2022 because insurers moved from IFRS 4 to IFRS 17 reporting in 2023.

> **Note:** Industry loss development data for Canadian commercial property is not public, so the reserving triangles are **simulated**. They are scaled to the real premiums and loss ratios and labelled in the workbook. Replace them with real company data before using the reserving results for anything.

## Files

- [`Commercial_Property_Loss_Ratio_Model_v1.xlsx`](Commercial_Property_Loss_Ratio_Model_v1.xlsx): the model
- [`Commercial_Property_Loss_Ratio_Model_Explanation.docx`](Commercial_Property_Loss_Ratio_Model_Explanation.docx): full write-up covering objective, data, definitions, method and results

## Skills shown

Loss ratio and profitability analysis · Premium earning (written to earned) · Chain-ladder and Bornhuetter-Ferguson reserving · IBNR estimation · Model validation against benchmarks · Financial modelling in Excel

## Author

**Judin Rose George**, Actuarial Professional (M.Sc. Actuarial Science, P&C reserving and pricing)
