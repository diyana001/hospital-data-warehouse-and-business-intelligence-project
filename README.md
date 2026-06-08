# Hospital Data Warehouse & Business Intelligence Solution

## Project Overview

This project was developed as part of the Data Warehousing and Business Intelligence module at Sri Lanka Institute of Information Technology (SLIIT).

The objective of the project was to design and implement a complete Business Intelligence solution using SQL Server technologies, starting from raw operational data and ending with analytical dashboards and reports.

The solution includes:

* Data Warehouse Design
* ETL Development using SSIS
* Slowly Changing Dimensions (SCD Type 1 & Type 2)
* Accumulating Fact Tables
* SSAS Multidimensional Cube
* OLAP Operations
* Excel-based Analytical Reporting
* Power BI Interactive Dashboards

---

## Dataset

The project uses a Hospital Management System dataset containing:

* Patients
* Doctors
* Appointments
* Treatments
* Billing Transactions

The original dataset was enhanced with additional records to simulate more than one year of operational activity.

---

## Technologies Used

* Microsoft SQL Server
* SQL Server Integration Services (SSIS)
* SQL Server Analysis Services (SSAS)
* SQL Server Management Studio (SSMS)
* Microsoft Excel
* Power BI Desktop
* Power BI Service

---

## Data Warehouse Design

A Star Schema was implemented.

### Fact Table

FactBilling

### Dimension Tables

* DimPatient
* DimDoctor
* DimTreatment
* DimAppointment
* DimDate

The grain of the fact table is defined as:

One billing transaction per patient per treatment.

---

## ETL Implementation

Data was extracted from multiple source formats:

* CSV Files
* TXT Files

The ETL pipeline performs:

* Data Extraction
* Data Cleansing
* Data Profiling
* Data Transformation
* Data Loading

### Slowly Changing Dimensions

DimPatient and DimDoctor were implemented using:

* SCD Type 1
* SCD Type 2

Historical tracking was maintained using:

* StartDate
* EndDate
* IsCurrent

---

## SSAS Cube

An OLAP cube was created using the data warehouse.

Cube features:

* Measures
* Dimensions
* Hierarchies
* Aggregations

### Implemented Hierarchies

Date Hierarchy

Year → Month → Day

Doctor Hierarchy

Branch → Specialization → Doctor

---

## OLAP Analysis

The cube was connected to Excel and used to demonstrate:

* Roll-up
* Drill-down
* Slice
* Dice
* Pivot

using Pivot Tables and Pivot Charts.

---

## Power BI Reports

### Report 1

Matrix visualization with row and column grouping.

### Report 2

Interactive dashboard with cascading slicers and multiple charts.

### Report 3

Drill-down report for hierarchical analysis.

### Report 4

Drill-through report for detailed transaction exploration.

---

## Key Learning Outcomes

* Dimensional Modeling
* Data Warehouse Design
* ETL Development
* SSAS Cube Design
* OLAP Operations
* Business Intelligence Reporting
* Power BI Dashboard Development

---

## Author

Diyana Kaluarachchi

BSc (Hons) Information Technology (Specialization in Data Science) 

Sri Lanka Institute of Information Technology (SLIIT)
