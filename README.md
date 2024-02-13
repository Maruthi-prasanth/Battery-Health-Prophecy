# Battery-Health-Prophecy
### TABLE OF CONTENTS

1. [ABSTRACT](#abstract)
2. [DATASET](#dataset)
3. [OBJECTIVE](#objective)
4. [EXTRACTION](#extraction)
   - [HI1 Extraction](#hi1-extraction)
   - [HI2 Extraction](#hi2-extraction)
   - [HI3 Extraction](#hi3-extraction)
5. [CORRELATION](#correlation)
6. [CONTRIBUTIONS](#contributions)
7. [LICENSE](#license)
8. [CONCLUSION](#conclusion)

---

#### ABSTRACT

This project utilizes battery datasets from NASA, focusing on measured variables like Voltage, Charge, Current, Temperature, Time, and Capacity. It extracts health indices (HI’s) from battery datasets, emphasizing Charge and Discharge cycles. The project involves capacity extraction, health indices extraction, and correlation analysis to predict battery State of Health (SOH).

---

#### DATASET

The research uses NASA's battery data, analyzing the aging of different batteries (B0005, B0006, B0007, B0018) through charging, discharging, and impedance tests. Each cycle, including charge, discharge, and impedance testing, provides data on voltage, time, charge, current, and temperature. The project focuses on organizing and understanding these cycles for comprehensive battery analysis.

---

#### OBJECTIVE

The main objective is to find correlation values between Health Indices (HI’s) and Capacity values. Using Pearson and Spearman methods, the project evaluates the applicability of specific health indices for prediction. Creating a correlation table for all datasets is crucial for predicting the State of Health (SOH) of a battery.

---

#### EXTRACTION

The project extracts capacity values from the discharging process and three specific Health Indices from the charging processes (HI1, HI2, HI3). The focus is on clean data preparation and choosing HI’s related to battery health. Correlation values help identify relevant HI’s strongly linked to battery health, aiding accurate predictions.

---

#### HI1 Extraction

HI1 involves time differences related to voltage values. Specific voltage values (3.9 and 4.2) in each charging cycle are used to calculate time differences, showing a decreasing trend across cycles.

---

#### HI2 Extraction

HI2 focuses on voltage differences related to time values. By updating time values corresponding to 3.9 voltage points, new indexes are found in each cycle, revealing fluctuations between starting and ending points.

---

#### HI3 Extraction

HI3 is based on current and time, considering the drop in current between 1.5A and the current after 1000 seconds during the constant voltage charging phase.

---

#### CORRELATION

Correlation analysis is conducted using Pearson and Spearman methods to understand connections between Health Indices and battery capacity. A correlation value of 0.95 or higher indicates the importance of specific HI’s for predicting battery health. This threshold guides the focus on relevant HI’s strongly linked to battery health.

---

#### LICENSE

This project is licensed under the [MIT License](LICENSE).

---

#### CONCLUSION

The project concludes by exploring the relationship between Health Indices and battery capacity. Both Pearson and Spearman correlation analyses reveal a correlation ranging between -0.9 and 0.9 concerning HI and battery capacity. The findings provide insights into the complex relationship between HI and battery capacity, enhancing battery usage efficiency across diverse applications.
