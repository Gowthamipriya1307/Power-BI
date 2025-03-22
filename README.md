
# Employee Presence Dashboard - Power BI Project

## Project Overview
This Power BI project focuses on analyzing employee presence data based on HR requirements for a company. The dataset contains attendance details for employees from April, May, and June, each stored in separate Excel sheets. The dashboard provides insights into:

- **Trends in Work From Home (WFH) and Work From Office (WFO) percentages.**
- **Preferred WFH days** (e.g., mid-week vs. start of the week).
- **Identifying patterns in sick leaves** to take preventive measures for illnesses like COVID-19.

---

## 📊 Data Preparation

### **Challenges:**
- The dataset had **dates as column headers** and employee details as rows, making it difficult to merge data across months.
- The presence of **text values in the date columns** required data type transformation.

### **Solution:**
- Used **Power Query** to transform data by **unpivoting date columns** and standardizing the structure.
- Converted text values in the new **date column** to the correct format.
- Created a **reusable function** to apply the transformation across all three sheets (April, May, and June).
- Performed multiple **accuracy checks** against the original Excel sheets.

---

## 🛠 DAX Measures & Calculations

- Created key measures such as **Total Days, Working Days, and Present Days**.
- Accounted for different work modes:
  - **Work From Home (WFH)** counted as **full presence**.
  - **Half Work From Home (HWFH)** counted as **0.5 days**.
  - **Similar logic applied** for Sick Leave (SL) and Half Sick Leave (HSL).

---

## 📌 Dashboard Features

1. **KPI Cards:** Displaying Presence %, WFH %, and SL %.
2. **Tables:** Employee-wise breakdown of attendance data.
3. **Combination Charts:** Trends for Presence %, WFH %, and SL % over time.
4. **Day-wise Analysis:** Presence %, WFH %, and SL % distribution across weekdays.
   
   **Findings:**
   - ✅ **Presence% is highest on Mondays**.
   - ✅ **WFH% peaks on Fridays**.
   - ✅ **Sick Leave % is also higher on Mondays**.

---

## 💡 Insights & Business Impact

- Helps HR plan **client releases** and **team-building activities** when maximum employees are available.
- Supports **space utilization strategies** to **reduce infrastructure costs**.
- Identifies **sick leave trends**, allowing proactive measures to prevent illness outbreaks.

---

## 🔮 Future Enhancements

### **1️⃣ Automatic Data Refresh**
- Store source files in **SharePoint** or **Google Sheets**.
- Set up Power BI **scheduled refresh** to update data automatically.

### **2️⃣ Alert Notifications**
- Publish dashboard to Power BI **Cloud Service**.
- Pin key visuals and **set alerts** (e.g., if Presence% < 80%, trigger an email notification to HR).

### **3️⃣ Role-Based Security**
- Implement **Row-Level Security (RLS)** to restrict data access based on user roles.
- Allow management to view **summary dashboards** without accessing raw data.

---

## 🚀 How to Use This Project

1. **Download** the **Power BI (.pbix) file** from this repository.
2. **Open it** in **Power BI Desktop**.
3. **Replace dataset** with updated employee attendance files if needed.
4. **Publish to Power BI Service** for sharing and scheduling updates.

---

## 🔗 Repository Link

📂 **GitHub Repository:** [GitHub Repository](https://github.com/Gowthamipriya1307/Power-BI)

---


