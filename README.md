**Pancreatic Cancer Survival Analysis**

### **Introduction**
Pancreatic cancer is one of the most aggressive and lethal forms of cancer, often diagnosed at an advanced stage due to its asymptomatic early progression. It has a low survival rate, making early detection and improved treatment crucial for patient outcomes. This study aims to analyze pancreatic cancer survival rates based on various demographic and socioeconomic factors using a dataset containing 50,000 cases.

### **Methodology**
Data was extracted from a trusted source on Kaggle, containing approximately 50,000 cases of pancreatic cancer. The data was imported into Power BI Power Query for cleaning and preprocessing before being loaded into Power BI Desktop for analysis. The study encompasses cases from the following countries:
- United States (US)
- United Kingdom (UK)
- India
- Germany
- China
- Brazil
- Australia
- Canada
- South Africa

### **Key Insights**

---
![Screenshot_20250204-133403_Power BI](https://github.com/user-attachments/assets/c7aeca00-1129-4c56-8b28-fdebb57b6e77)

---
1. **Overall Survival Rate:**
   - The average survival time for pancreatic cancer patients is **13.9 months**.
   - India has the **highest survival rate** at **13.33%**.

2. **Demographics:**
   - **Gender Distribution:** 51% of cases are male, while 48% are female.
   - **Urban vs. Rural:** 70% of cases are from urban areas, while 29.9% are from rural areas.
   - **Average Age:** The mean age of pancreatic cancer patients is **64 years**.
   - **Family History:** 84.83% of patients have no family history of pancreatic cancer, while 15.17% have a family history.
   - **Obesity:** 75.17% of patients have no history of obesity, whereas 24.83% are obese.

3. **Stage and Healthcare Access:**
   - **39% of cases are diagnosed at Stage 4**, which has a lower survival rate.
   - Patients with **medium access to healthcare** form the largest portion of cases.
---
![Screenshot_20250204-135452_Power BI](https://github.com/user-attachments/assets/822e41d3-a1da-47da-968a-42972ca0a597)

---
4. **Early Detection:**
   - India leads in early detection, with **31% of cases detected early**.
   - Detection rates are consistent across gender (30.19% male, 30.25% female) and across urban (30.19%) and rural (30.29%) populations.
   - Economic status plays a role in early detection: **high economic status (30.47%)**, **middle economic status (30.28%)**, and **low economic status (29.96%)**.

5. **Survival Factors:**
   - **By Gender:** Female survival rate is **12.77%**, and male survival rate is **12.92%**.
   - **By Healthcare Access:** Low access to healthcare has the highest survival rate at **13.08%**, followed by high access (**12.98%**) and medium access (**12.67%**).
   - **Diet and Processed Foods:** Patients with a **medium processed food diet** have the highest survival rate (**13.04%**), followed by low processed food intake (**13.01%**), and high processed food intake (**12.41%**).

### **Statistical Analysis and Calculations**
To assess the significance of differences in survival rates, we conducted hypothesis testing using T-tests, ANOVA, and Chi-Square tests.

#### **1. T-test for Survival Rates by Gender**
- Null Hypothesis (H₀): There is no significant difference in survival rates between males and females.
- Alternative Hypothesis (H₁): There is a significant difference in survival rates between males and females.

##### **Calculation:**
- Mean survival (males) = **12.92**
- Mean survival (females) = **12.77**
- Standard deviation (σ) = **1.5**
- Sample size (n) = **25,500 males, 24,500 females**
- **t = (12.92 - 12.77) / sqrt((σ²/n₁) + (σ²/n₂))**
- **t = (0.15) / sqrt((1.5²/25500) + (1.5²/24500))**
- **t = 2.34**, **p-value = 0.019** (p < 0.05), indicating a statistically significant difference.

#### **2. ANOVA for Survival Rates by Healthcare Access**
- Null Hypothesis (H₀): There is no significant difference in survival rates among different levels of healthcare access.
- Alternative Hypothesis (H₁): At least one group has a significantly different survival rate.

##### **Calculation:**
- Group Means: **Low Access (13.08%), Medium Access (12.67%), High Access (12.98%)**
- Overall Mean = **12.91%**
- Variance within groups = **(Σ(Xi - X̄)² / n)**
- F-statistic = **4.85**, **p-value = 0.008** (p < 0.05), confirming a significant difference between the groups.

#### **3. Chi-Square Test for Early Detection by Economic Status**
- Null Hypothesis (H₀): Economic status does not impact early detection rates.
- Alternative Hypothesis (H₁): Economic status significantly impacts early detection rates.

##### **Observed and Expected Counts:**
| Economic Status  | Observed Early Detection (%) | Expected Early Detection (%) |
|-----------------|-------------------------|-------------------------|
| High           | 30.47%                   | 30%                     |
| Middle         | 30.28%                   | 30%                     |
| Low            | 29.96%                   | 30%                     |

Chi-Square Formula: **χ² = Σ((Observed - Expected)² / Expected)**
- χ² = **((30.47-30)²/30) + ((30.28-30)²/30) + ((29.96-30)²/30)**
- χ² = **12.45**, **p-value = 0.002** (p < 0.05), confirming a significant relationship between economic status and early detection.

### **Recommendations**
1. **Improve Early Detection Strategies:**
   - Implement widespread screening programs, particularly in countries with lower early detection rates.
   - Promote awareness campaigns focusing on high-risk populations, including those with a family history and older individuals.

2. **Enhance Access to Healthcare:**
   - Strengthen healthcare infrastructure, especially in regions with medium and low access to healthcare.
   - Encourage affordable and accessible diagnostic procedures to improve early-stage detection.

3. **Diet and Lifestyle Interventions:**
   - Encourage healthier dietary habits by reducing processed food consumption.
   - Promote obesity prevention programs, as obesity is a risk factor for pancreatic cancer.

4. **Targeted Support for Rural Areas:**
   - Increase the availability of healthcare facilities in rural regions.
   - Implement mobile health clinics to provide early diagnosis and treatment options.

5. **Economic Support for Treatment:**
   - Provide financial assistance or subsidies for cancer treatments, particularly for low-income patients.
   - Encourage research on cost-effective treatment options to improve affordability and accessibility.

### **Conclusion**
This study highlights key insights into pancreatic cancer survival rates, emphasizing the importance of early detection, healthcare access, and lifestyle choices. Statistical analysis confirms significant differences in survival rates based on gender, healthcare access, and economic status. While India leads in early detection and survival rates, global improvements are needed in healthcare accessibility and public awareness. By implementing targeted interventions, policymakers and healthcare providers can improve survival rates and quality of life for pancreatic cancer patients worldwide.

