# 🚗 Road Accident Analysis Dashboard

## 📊 Project Overview

The **Road Accident Analysis Dashboard** is an interactive **Power BI** dashboard developed to analyze road accident casualties and identify patterns across vehicle types, road types, locations, weather conditions, light conditions, and time.

The project focuses on transforming accident data into meaningful insights using **Power BI, DAX, data modeling, and data visualization**.

---

## 🎯 Project Objectives

- Analyze total road accident casualties
- Track total accidents and casualties for the current year
- Compare current-year performance with the previous year
- Analyze casualties by severity
- Identify casualty patterns by vehicle type
- Analyze monthly casualty trends
- Compare urban and rural casualties
- Analyze casualties by road type
- Analyze casualties by light conditions
- Analyze casualties by weather conditions
- Build a structured Power BI data model
- Create custom DAX KPIs and measures
- Develop an interactive and user-friendly dashboard

---

## 🛠️ Tools & Technologies

- **Power BI Desktop**
- **DAX**
- **Power Query**
- **Data Modeling**
- **Data Visualization**
- **Microsoft Excel / CSV**

---

## 🗂️ Dataset

The project uses a road accident dataset containing information related to accidents, casualties, vehicles, road conditions, environmental conditions, and locations.

Key fields include:

- Accident Date
- Accident Index
- Accident Severity
- Vehicle Type
- Road Type
- Light Conditions
- Weather Conditions
- Day of Week
- Junction Control
- Junction Detail
- Carriageway Hazards
- Latitude
- Location-related attributes

The dataset was cleaned and transformed before being used for analysis in Power BI.

---

## 🧹 Data Preparation

The data preparation process included:

- Data inspection
- Data cleaning
- Handling missing and inconsistent values
- Standardizing categorical fields
- Preparing date-related information
- Creating a dedicated Calendar table
- Establishing relationships between tables
- Creating DAX measures
- Preparing data for visualization

---

# 📌 Dashboard Requirements

The dashboard was designed based on defined **Primary KPIs** and **Secondary KPIs**.

### Primary KPIs

- Total Casualties and Total Accident values for Current Year and YoY growth
- Total Casualties by Accident Severity for Current Year and YoY growth

### Secondary KPIs

- Total Casualties with respect to vehicle type for Current Year
- Monthly trend comparing Current Year and Previous Year
- Casualties by Road Type for Current Year
- Current Year casualties by Area/Location and Day/Night
- Total Casualties and Total Accidents by Location

<p align="center">
  <img src="Road accident analysis/KPI's.PNG" alt="Road Accident Analysis KPI Requirements" width="90%">
</p>

---

# 🗃️ Data Modeling

A dedicated **Calendar table** was created to support time-based analysis.

The Power BI model consists primarily of:

### Sheet1

The main accident dataset containing accident and casualty information.

### Calender

The date dimension containing:

- Date
- Month
- Year

The Calendar table is connected to the main accident table through the accident date.

The model enables:

- Current Year analysis
- Previous Year analysis
- Monthly trends
- Year-over-Year comparisons
- Date-based filtering

<p align="center">
  <img src="Road accident analysis/Modeling.PNG" alt="Power BI Data Model" width="90%">
</p>

---

# 🧮 KPI Development

Custom **DAX measures** were created to calculate the key performance indicators displayed on the dashboard.

The main KPIs include:

- **Total CY Casualties**
- **Total CY Accidents**
- **CY Fatal Casualties**
- **CY Serious Casualties**
- **CY Slight Casualties**

The dashboard also includes **Year-over-Year (YoY)** comparisons to track changes in accident and casualty performance.

### YoY Calculation

The basic calculation follows:

```text
YoY % Change =
(Current Year Value - Previous Year Value)
÷ Previous Year Value
× 100
````

---

# 📊 Dashboard

The final Power BI dashboard brings together the developed KPIs and analytical visualizations into a single interactive report.

<p align="center">
  <img src="Road accident analysis/Dashboard.PNG" alt="Road Accident Analysis Dashboard" width="100%">
</p>

---

## 📈 Dashboard Analysis

### 🚗 Casualties by Vehicle Type

The dashboard analyzes casualties across different vehicle categories:

* Agricultural
* Bike
* Bus
* Car
* Other
* Van

Cars account for the highest number of casualties among the vehicle categories displayed.

---

### 📅 CY Casualties vs PY Casualties Monthly Trend

The monthly trend compares casualties between the current year and previous year across January to December.

This visualization helps identify:

* Monthly fluctuations
* Seasonal patterns
* High-casualty months
* Low-casualty months
* Year-over-year changes

---

### 🏙️ Casualties by Urban / Rural

The dashboard compares casualties between urban and rural areas.

The displayed dashboard shows:

* **Urban: 61.87%**
* **Rural: 38.13%**

---

### 🛣️ Casualties by Road Type

Casualties are analyzed across different road types:

* Single carriageway
* Dual carriageway
* Roundabout
* One way street
* Slip road

Single carriageways contribute the highest number of casualties in the displayed analysis.

---

### 🌧️ Casualties by Weather Conditions

The dashboard provides a breakdown of casualties by weather conditions, including:

* Fine
* Rain
* Other
* Snow
* Fog or Mist

Fine weather represents the largest category in the displayed dashboard.

---

### 🌙 Casualties by Light Condition

The dashboard compares casualties occurring under:

* Daylight
* Dark

The displayed analysis shows approximately:

* **Daylight: 73.91%**
* **Dark: 26.09%**

---

## 🔑 Key Dashboard Metrics

The dashboard displays the following current-year metrics:

| KPI                   |  Value |
| --------------------- | -----: |
| Total CY Casualties   | 191.7K |
| Total CY Accidents    | 141.2K |
| CY Fatal Casualties   |  2,807 |
| CY Serious Casualties |  26.7K |
| CY Slight Casualties  | 162.2K |

The KPI cards also display the corresponding YoY percentage change.

---

## 🔄 Project Workflow

```text
Raw Accident Dataset
        │
        ▼
Data Cleaning & Transformation
        │
        ▼
Power Query
        │
        ▼
Calendar Table Creation
        │
        ▼
Data Modeling
        │
        ▼
DAX Measures & KPIs
        │
        ▼
Power BI Visualizations
        │
        ▼
Interactive Dashboard
        │
        ▼
Accident Analysis & Insights
```

---

## 📊 Dashboard Components

| Component          | Purpose                                        |
| ------------------ | ---------------------------------------------- |
| KPI Cards          | Current-year accident and casualty performance |
| Vehicle Type       | Analyze casualties by vehicle category         |
| Monthly Trend      | Compare Current Year vs Previous Year          |
| Urban / Rural      | Analyze casualty distribution by area          |
| Road Type          | Identify high-casualty road types              |
| Weather Conditions | Analyze casualties by weather                  |
| Light Conditions   | Analyze daylight vs dark casualties            |

---

## 💡 Business Value

The dashboard provides a consolidated view of road accident data that can help users:

* Monitor accident and casualty performance
* Identify high-casualty vehicle categories
* Identify high-casualty road types
* Compare urban and rural accident patterns
* Analyze casualty severity
* Identify monthly trends
* Understand environmental factors
* Compare current-year and previous-year performance
* Support data-driven road safety decisions

---

## 🚀 Future Enhancements

Potential improvements include:

* Geographic accident hotspot analysis
* Interactive map visualizations
* Location-level drill-through
* Accident severity prediction
* Accident trend forecasting
* Population-based accident rates
* Traffic-volume-based accident rates
* Age and demographic analysis
* More detailed location analysis
* Automated data refresh

---

## 🧠 Skills Demonstrated

* Power BI
* DAX
* Power Query
* Data Modeling
* Data Cleaning
* KPI Development
* Data Visualization
* Time-Series Analysis
* Business Intelligence
* Dashboard Design
* Analytical Storytelling

---

## 📁 Project Structure

```text
Road-Accident-Analysis/
│
├── README.md
│
├── Dataset/
│   └── accident_data.xlsx
│
├── PowerBI/
│   └── Road_Accident_Analysis.pbix
│
└── Images/
    ├── dashboard.png
    ├── kpi.png
    └── data-model.png
```

---

## 📌 Conclusion

The **Road Accident Analysis Dashboard** demonstrates an end-to-end Power BI workflow covering **data preparation, data modeling, DAX KPI development, and interactive visualization**.

The project combines a structured data model with custom KPIs and multiple analytical visualizations to provide a comprehensive view of road accident casualties.

By analyzing **vehicle type, road type, urban/rural areas, weather conditions, light conditions, and monthly trends**, the dashboard transforms raw accident data into an interactive analytical solution for understanding road safety patterns.

---

## 👨‍💻 Author

**Tanmay Shevale**

Aspiring Data Analyst | Business Analytics | SQL | Power BI | Data Visualization
