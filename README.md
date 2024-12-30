# Hospitalization Hypothesis Testing

## Overview
This project aims to analyze the factors influencing hospitalization charges across different regions. Through statistical hypothesis testing, we identify and quantify the significance of variables such as smoking status, viral load, and severity level in predicting hospitalization costs. The analysis is conducted using Python and various data science tools.

## Business Requirements
1. **Determine the primary factors influencing hospitalization charges:**
   - Evaluate the significance of the `smoker` variable in predicting hospitalization costs.
   
2. **Assess the contribution of other key variables:**
   - Analyze the influence of `viral load`, `smoking status`, and `severity level` on hospitalization charges.

## Dataset
The dataset provided includes information on patients' hospitalization charges, along with variables such as:
- `smoker`: Indicates whether the patient is a smoker.
- `viral load`: The viral load measurement of the patient.
- `severity level`: A categorical representation of the patient’s condition severity.
- Hospitalization charges and other demographic and regional variables.

## Key Findings
- **Smoking Status:**
  - Patients who smoke incur significantly higher hospitalization charges compared to non-smokers.
  - The coefficient for non-smokers is `-30,180`, indicating a reduction in charges by approximately $30,180. Conversely, for smokers, charges increase by around $29,440.
  - Confidence intervals for smokers and non-smokers:
    - Non-smokers: [$31,600, $28,800]
    - Smokers: [$27,900, $31,000]

- **Viral Load:**
  - Each unit increase in viral load results in an approximate $2,544 increase in hospitalization charges.
  - Confidence interval: [$2,123, $2,965]

- **Severity Level:**
  - Each unit increase in severity level leads to an increase of around $1,188 in hospitalization charges.
  - Confidence interval: [$513, $1,864]

## Tools and Techniques
- **Data Analysis:** Pandas, NumPy
- **Statistical Testing:** Statsmodels
- **Visualization:** Matplotlib
- **Hypothesis Testing:** p-values and confidence intervals to determine variable significance

## Steps to Run the Project
1. **Clone the repository:**
   ```bash
   git clone <repository_url>
   cd hospitalization-hypothesis-testing
   ```

2. **Install dependencies:**
   Ensure Python 3.7+ is installed, then run:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the analysis:**
   Open the `hospitalization_analysis.ipynb` file in Jupyter Notebook or execute the Python script directly:
   ```bash
   python hospitalization_analysis.py
   ```

4. **View results:**
   Outputs include statistical summaries, confidence intervals, and visualizations to support the findings.

## Future Improvements
- Expand analysis to include additional variables such as age, gender, and region-specific effects.
- Implement predictive modeling using regression techniques to estimate hospitalization charges.
- Automate data cleaning and preprocessing steps for scalability.


## Contributors
- **Eeshan Agarwal**

## Acknowledgments
This project is inspired by the dataset and problem statement from StrataScratch's platform. Special thanks to their team for providing the dataset and support for this analysis.

---
For any queries or contributions, please contact [Eeshan Agarwal](mailto:eeshan.agarwal6@gmail.com).
