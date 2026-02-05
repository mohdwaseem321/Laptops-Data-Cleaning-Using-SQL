# LaptopsData_Cleaning_Using_SQL
### Laptop Data Cleaning & Transformation using SQL
A structured SQL-based data cleaning project focused on transforming a raw laptops dataset into a clean, analysis-ready format by handling inconsistent text fields, mixed units, and unstructured columns.

### Short Description / Purpose
The Laptop Data Cleaning project is designed to clean, standardize, and restructure a real-world laptops dataset using SQL.
The purpose of this project is to demonstrate how raw, messy data can be converted into structured and reliable data that is ready for analysis, reporting, and visualization.

### Tech Stack
The project was built using the following tools and technologies:<br>
• 🗄 SQL (MySQL) – Core language used for data cleaning and transformation.<br>
• 🔤 SQL String Functions – Used for splitting, replacing, and extracting text values.<br>
• 🧮 Conditional Logic (CASE WHEN) – Applied for handling mixed units (GB/TB) and conditional extraction.<br>
• 🔄 Data Type Conversion – Converted text-based fields into numeric formats for analysis.<br>
• 📁 Relational Tables – Structured cleaned data into multiple meaningful columns.

### Data Source
Source: Kaggle

The dataset contains information about laptops, including hardware specifications, screen details, operating systems, and pricing.

Rows: 1300+

Original Columns: index, Unnamed: 0 ,Company,TypeName,Inches,ScreenResolution,Cpu,Ram,Memory,Gpu,OpSys,Weight,Price

### Features / Highlights
🔹 Business Problem

-  Laptop datasets collected from online sources often contain unstructured and mixed-format data.
-  Columns such as CPU, GPU, Memory, RAM, and Screen Resolution combine multiple attributes into a single field, making analysis difficult and error-prone.
-  Key challenges include:
-  Mixed units (GB & TB) in storage fields
-  Text-heavy columns storing multiple values
-  Inconsistent formats across rows
-  Poor suitability for aggregation and visualization

🔹 Goal of the Project

-  To build a clean, structured, and analysis-ready dataset by:
-  Breaking down complex columns into meaningful attributes
-  Standardizing numeric values
-  Improving data quality and usability
-  Demonstrating real-world SQL data cleaning skills

🔹 Walkthrough of Key Cleaning Steps

🧠 Data Safety & Validation

-  Created a backup table before starting transformations
-  Verified row counts to ensure no data loss
-  Checked memory consumption for reference

🧹 Structural Cleaning

-  Dropped non-important and redundant columns
-  Optimized data types for better performance

⚙️ Column-wise Transformations

-  RAM Column, Removed GB
-  Converted values into numeric format
-  CPU Column Split into:-  Cpu_Brand, Cpu_Speed
-  GPU Column Split into:-   Gpu_Brand, Gpu_Name
-  ScreenResolution Column Split into:-   Resolution_Width, Resolution_Height
-  Touch_Screen (Yes / No)
-  Memory Column Split into:-   Memory_Type (SSD / HDD / Hybrid), Primary_Storage, Secondary_Storage
-  Handled both GB and TB units using conditional logic

🔹 Business Impact & Insights

-  Analysis Ready Data: Enables accurate aggregation, filtering, and visualization
-  Improved Data Quality: Eliminates ambiguity from text-heavy columns
-  Scalable Design: Clean schema can be reused for dashboards and ML models
-  Real-World Skill Demonstration: Reflects practical SQL skills used in data analyst roles

### Screenshots / Demos

Below are example visuals from the project:

![Cleaned Dataset](https://github.com/mohdwaseem321/Laptops-Data-Cleaning-Using-SQL/blob/main/Before%20Cleaning.jpg)
![Cleaned Dataset](https://github.com/mohdwaseem321/Laptops-Data-Cleaning-Using-SQL/blob/main/After%20Cleaning.jpg)
