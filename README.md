# 📊 Smartphones Data Cleaning  

## 📝 Overview  
This project focuses on cleaning and preprocessing a raw smartphone dataset to ensure accuracy, consistency, and usability for further analysis.

---

## ❓ Problem Statement   
Raw scraped datasets often contain duplicates, missing values, misplaced data, and formatting errors, leading to inaccurate insights. To prevent this, we apply structured data-cleaning techniques, ensuring the dataset is well-structured and ready for further analysis. 

---

## 🛠️ Solution Approach  
1. **Data Loading & Initial Exploration**  
   - Load the raw dataset.  
   - Check for missing values, duplicates, and data types.  

2. **Data Cleaning**  
   - Convert the `price` column from string to integer.  
   - Remove unnecessary symbols and characters.  
   - Fix incorrect row alignments and shift misplaced values.  
   - Drop irrelevant or erroneous rows.  

3. **Feature Engineering**  
   - Extract and create new features like `brand_name`, `processor details`, `RAM capacity`, and `storage`.  
   - Identify whether a smartphone has **5G, NFC,** or an **IR blaster**.  
   - Parse numerical values from text fields (e.g., `battery_capacity`, `camera megapixels`, `screen_size`).  
   - Standardize categorical values such as `operating_system`.  

4. **Final Adjustments & Exporting Cleaned Data**  
   - Ensure correct data types for each column.  
   - Handle missing values appropriately.  
   - Export the cleaned dataset as `smartphone_cleaned_v2.csv`.  

---

## 🔑 Key Findings  
- Some rows had **misaligned values**, requiring careful shifting of column data.  
- Certain features such as **RAM and internal memory** were combined in a single column and needed to be **separated**.  
- Several smartphones were missing information on **operating systems** and **camera specifications**.  
- The dataset contained **inconsistent formatting**, especially in numerical columns, which required cleaning and standardization.  

---

## 🛠️ Libraries & Tools Used  
- **Pandas** → Data manipulation and cleaning  
- **NumPy** → Numerical operations  
- **Regular Expressions (RegEx)** → Extracting numerical values from text
## ⚙️ How It Works  
1. The script **loads** the raw dataset.  
2. It performs **various cleaning operations**, including **value shifting, missing data handling, and formatting corrections**.  
3. It extracts relevant features and **creates new columns**.  
4. The cleaned dataset is **saved** for use in the **EDA phase**.  

---
