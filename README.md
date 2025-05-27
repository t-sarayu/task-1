# task-1
# Data Cleaning for KaggleV2-May-2016 Dataset

## 📁 Dataset
This dataset contains medical appointment records, including patient demographics, appointment details, and whether a patient showed up.

**Source File:** `KaggleV2-May-2016.csv`

---

## 🧹 Data Cleaning Tasks

The following preprocessing steps were performed using Python (pandas):

### ✅ 1. Identify and Handle Missing Values
- Used `.isnull().sum()` to detect missing values.
- No missing values were found in the dataset.

### ✅ 2. Remove Duplicate Rows
- Used `.drop_duplicates()` to eliminate any exact duplicate entries.

### ✅ 3. Standardize Text Values
- Converted the `Gender` column to lowercase (`male`, `female`).

### ✅ 4. Convert Date Formats
- Converted `ScheduledDay` and `AppointmentDay` to consistent `datetime` format (`dd-mm-yyyy`).
- Then, converted these columns to proper datetime objects for further analysis.

### ✅ 5. Rename Column Headers
- Cleaned column names:
  - Converted to lowercase
  - Removed leading/trailing whitespaces
  - Replaced spaces with underscores

### ✅ 6. Fix Data Types
- Ensured `age` is of type `int`.
- Converted `scheduledday` and `appointmentday` to `datetime64`.

---

## 📤 Output Files
- `cleaned_KaggleV2-May-2016.csv` – Fully cleaned dataset
- `raw_KaggleV2-May-2016.csv` – Original dataset

---

## 📌 Notes
- No null values or duplicates were found, but cleaning was performed for consistency and robustness.
- This cleaned data is now ready for further exploratory analysis, modeling, or visualization.

---

## 📚 Requirements
```bash
pandas >= 1.0.0
