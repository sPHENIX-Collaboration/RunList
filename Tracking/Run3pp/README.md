# Run3pp Run List

The **Golden Run List** and **Acceptable Run List** are obtained from detector occupancy and MBD-rate-based quality criteria for the MVTX, INTT, and TPC.

Runs shorter than 5 minutes are excluded from the analysis. For each remaining run, the detector cluster counts are evaluated using two independent criteria:

1. Cluster count as a function of run number.
2. Cluster count as a function of the average MBD rate.

For each detector and each criterion, a 1σ and 2σ band is used to classify the run:

- **Good:** within the 1σ band.
- **Acceptable:** outside the 1σ band but within the 2σ band.
- **Bad:** outside the 2σ band.

The overall run quality is determined from the MVTX, INTT, and TPC classifications for both criteria.

- A run is included in the **Golden Run List** when all detector classifications are **Good**.
- A run is included in the **Acceptable Run List** when no detector is **Bad** and at least one detector is classified as **Acceptable**.
- Runs with missing information required for the classification are assigned an **Unknown** quality and are not included in either list.

The detailed run-by-run classification, including detector quality and overall run quality, is available in the [Tracking Run List summary spreadsheet](https://docs.google.com/spreadsheets/d/1c2SNsvb3aFJMJfRk194JQ2azA5tNzCrfIdu1omJezPA/edit?usp=sharing).

## Run List Summary

| Run List | Total Runs | Total Raw Events (MBD12) | Total Live Events (MBD12) | Total Scaled Events (MBD12) |
|:---|---:|---:|---:|---:|
| **Golden** | 327 | 172,055,315,122 | 165,745,989,146 | 3,375,148,673 |
| **Acceptable** | 275 | 129,635,961,353 | 124,261,987,430 | 2,315,642,302 |


## Quality Classification

| Classification | Definition |
|:---|:---|
| **Good** | Detector cluster count is within the 1σ band. |
| **Acceptable** | Detector cluster count is outside the 1σ band but within the 2σ band. |
| **Bad** | Detector cluster count is outside the 2σ band. |
| **Unknown** | Required information for classification is missing. |

## Overall Run Selection

| Run List | Selection Criteria |
|:---|:---|
| **Golden** | All MVTX, INTT, and TPC classifications are **Good** for both criteria. |
| **Acceptable** | No detector classification is **Bad**, and at least one classification is **Acceptable**. |
| **Excluded** | Run is **Unknown** or otherwise does not satisfy the Golden or Acceptable criteria. |
