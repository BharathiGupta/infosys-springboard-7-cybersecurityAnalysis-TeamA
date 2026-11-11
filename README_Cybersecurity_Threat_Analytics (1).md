# Cybersecurity Threat Analytics Platform with Incident Visualization System

An interactive Power BI project using a Kaggle cybersecurity dataset.
The project covers data preprocessing, dashboard development, and
analysis of incident and network characteristics.

> **Project status:** Data Preprocessing and Dashboard Pages 1--2 are
> completed. Pages 3--5 are planned under the third development phase.
> Their visuals will be confirmed after validating the relevant dataset
> fields.

## Table of Contents

-   [Project Overview](#project-overview)
-   [Objectives](#objectives)
-   [Dataset](#dataset)
-   [Tools and Technologies](#tools-and-technologies)
-   [Project Workflow](#project-workflow)
-   [Work Completed](#work-completed)
-   [Dashboard Structure](#dashboard-structure)
-   [Team Responsibilities](#team-responsibilities)
-   [Suggested Repository Structure](#suggested-repository-structure)
-   [How to Open the Project](#how-to-open-the-project)
-   [Data Interpretation Notes](#data-interpretation-notes)
-   [Future Work](#future-work)

## Project Overview

The **Cybersecurity Threat Analytics Platform with Incident
Visualization System** uses Power BI to explore a Kaggle cybersecurity
dataset containing approximately 40,000 records and 25 original columns.

The project is organised into three phases:

1.  **Data Preprocessing** -- inspecting, cleaning, transforming and
    validating the dataset using Power BI Desktop and Power Query
    Editor.
2.  **Dashboard Development and Analysis** -- building the first two
    interactive dashboard pages to examine incident volume, attack
    categories, severity, time-based patterns, network protocols and
    anomaly scores.
3.  **Extended Dashboard Development** -- developing three additional
    dashboard pages with distinct analytical purposes. The exact visuals
    will be confirmed after checking field values, missingness and
    suitability.

The aim is to prepare the data for analysis and present its patterns
through clear, interactive visualisations.

## Objectives

-   Understand the structure and quality of the cybersecurity dataset.
-   Prepare the data using Power Query.
-   Create date-related fields and a date dimension for time-based
    analysis.
-   Create relevant DAX measures and KPIs.
-   Build interactive Power BI dashboards.
-   Explore incident categories, severity levels, network
    characteristics and anomaly scores.
-   Present findings clearly without making unsupported conclusions.

## Dataset

**Source:** Kaggle\
**Approximate size:** 40,000 rows\
**Original columns:** 25\
**Columns after preprocessing:** Approximately 30

The original dataset includes:

`Timestamp`, `Source IP Address`, `Destination IP Address`,
`Source Port`, `Destination Port`, `Protocol`, `Packet Length`,
`Packet Type`, `Traffic Type`, `Payload Data`, `Malware Indicators`,
`Anomaly Scores`, `Alerts/Warnings`, `Attack Type`, `Attack Signature`,
`Action Taken`, `Severity Level`, `User Information`,
`Device Information`, `Network Segment`, `Geo-location Data`,
`Proxy Information`, `Firewall Logs`, `IDS/IPS Alerts`, and
`Log Source`.

A separate **`Dim_Date`** table was created in Power BI for date-based
analysis. It includes fields such as Date, Year, Quarter, Month Name,
Month Number and Day Name.

## Tools and Technologies

  -----------------------------------------------------------------------
  Tool                                Purpose
  ----------------------------------- -----------------------------------
  Power BI Desktop                    Data modelling, DAX measures and
                                      dashboard development

  Power Query Editor                  Data inspection, cleaning and
                                      transformation

  DAX                                 KPI and analytical measure creation

  GitHub                              Version control and team
                                      collaboration
  -----------------------------------------------------------------------

## Project Workflow

1.  **Problem Understanding** -- identifying the project objective and
    the need for reliable, structured cybersecurity data.
2.  **Data Collection** -- obtaining the dataset from Kaggle and
    importing it into Power BI Desktop.
3.  **Data Understanding and Initial Inspection** -- reviewing columns,
    data types, values and data quality.
4.  **Data Cleaning and Preprocessing** -- cleaning text fields,
    standardising categorical values, checking duplicates and assessing
    missing values.
5.  **Data Transformation and Feature Creation** -- deriving
    date-related fields from `Timestamp` and preparing the data for
    analysis.
6.  **Data Validation and Quality Checking** -- reviewing data types,
    ranges, duplicate checks and consistency after transformations.
7.  **Data Modelling and DAX Measure Creation** -- preparing the
    `Dim_Date` table and measures for dashboard KPIs.
8.  **Dashboard Development and Visualisation** -- creating interactive
    pages with KPI cards, charts and slicers.
9.  **Testing, Validation and Insight Generation** -- checking visual
    behaviour, calculations, filters and patterns represented by the
    dataset.

## Work Completed

### Data Preprocessing

Data preprocessing was carried out in Power BI Desktop using Power Query
Editor. Activities included:

-   Inspecting column names and data types.
-   Assessing missing values.
-   Checking duplicate records.
-   Trimming and cleaning text fields.
-   Standardising selected categorical values.
-   Reviewing numeric fields and value ranges.
-   Creating date-related fields from `Timestamp`.
-   Validating the transformed dataset.

The processed dataset contains approximately 40,000 rows and 30 columns.
The `999+ rows` message in Power Query refers to the preview limit, not
the full dataset row count.

### Dashboard Development and Analysis -- Page 1

**Current dashboard title: Cybersecurity Incident Overview**

**KPI cards** 1. Total Incidents 2. High Severity Incidents 3. Average
Anomaly Score 4. Unique Source IPs

**Charts** 1. Incident Distribution by Severity -- Donut Chart 2.
Quarterly Incident Trend by Year -- Clustered Column Chart 3. Incident
Distribution by Attack Type -- Horizontal Bar Chart 4. Attack Type by
Severity Level -- Stacked Column Chart 5. Monthly Incident Comparison by
Year -- Clustered Column Chart 6. Incidents by Day of Week -- Column
Chart

**Slicers:** Attack Type, Year, Protocol, Severity Level and Date.

### Dashboard Development and Analysis -- Page 2

**Current dashboard title: Threat & Network Analysis**

**KPI cards** 1. Maximum Anomaly Score 2. Average Anomaly Score 3. Total
Attack Types 4. Unique Destination IPs

**Charts** 1. Packet Length Distribution -- Column Chart 2. Incident
Distribution by Protocol -- Donut Chart 3. Average Anomaly Score by
Attack Type -- Column Chart 4. Incident Distribution by Protocol and
Severity -- Stacked Column Chart 5. Anomaly Score Distribution -- Column
Chart

**Slicers:** Year, Attack Type, Protocol and Severity Level.

## Dashboard Structure

The project is planned to contain five dashboard pages.

  --------------------------------------------------------------------------
  Page              Page title        Focus                Status
  ----------------- ----------------- -------------------- -----------------
  1                 Cybersecurity     Incident volume,     Completed
                    Incident Overview attack types,        
                                      severity and         
                                      time-based trends    

  2                 Threat & Network  Network protocols,   Completed
                    Analysis          packet lengths and   
                                      anomaly scores       

  3                 Network Traffic & Traffic types, log   Planned
                    Communication     sources and port     
                    Analysis          usage                

  4                 Attack Pattern &  Source/destination   Planned
                    Source Analysis   IPs, attack          
                                      signatures and       
                                      network segments     

  5                 Security Risk &   Severity, anomaly    Planned
                    Response Analysis scores, alerts and   
                                      recorded response    
                                      actions              
  --------------------------------------------------------------------------

### Proposed visuals for the third development phase

The following lists are initial proposals, not completed or finally
approved visuals. The team will validate field values, missing data,
distinct counts and analytical usefulness before finalising them.

**Page 3 -- Network Traffic & Communication Analysis** - KPI: Unique
Source Ports - KPI: Unique Destination Ports - Incident Distribution by
Traffic Type - Incident Distribution by Log Source - Top 10 Source
Ports - Top 10 Destination Ports - Traffic Type by Protocol

**Page 4 -- Attack Pattern & Source Analysis** - KPI: Total Attack
Signatures - KPI: Total Network Segments - Top 10 Source IP Addresses -
Top 10 Destination IP Addresses - Attack Type by Network Segment - Top
Attack Signatures - Incident Distribution by Device Information

**Page 5 -- Security Risk & Response Analysis** - KPI: Incidents with
Security Alerts - KPI: Incidents with Malware Indicators - Severity
Distribution by Action Taken - Average Anomaly Score by Severity Level -
High Severity Incidents by Log Source - Incident Distribution by IDS/IPS
Alerts - Incident Distribution by Firewall Logs

**Target:** Seven main visuals per page, including KPI cards. Slicers
are additional and are not included in this count.

## Team Responsibilities

Proposed division of work for the third development phase:

  -----------------------------------------------------------------------
  Team member             Assigned page           Responsibility
  ----------------------- ----------------------- -----------------------
  Bharathi Gupta          Page 3 -- Network       Develop and validate
                          Traffic & Communication page visuals, KPIs and
                          Analysis                filters

  Shiva Sumedha           Page 4 -- Attack        Develop and validate
                          Pattern & Source        page visuals, KPIs and
                          Analysis                filters

  Gowshika                Page 5 -- Security Risk Develop and validate
                          & Response Analysis     page visuals, KPIs and
                                                  filters
  -----------------------------------------------------------------------

All team members should follow the agreed dashboard theme, use
consistent formatting, validate measures and review the integrated
report.

## Suggested Repository Structure

``` text
Cybersecurity-Threat-Analytics/
│
├── README.md
├── Dataset/
│   └── dataset-file-or-source-information
├── PowerBI/
│   ├── Cybersecurity_Dashboard.pbix
│   └── Dashboard_Screenshots/
│       ├── Page_1.png
│       ├── Page_2.png
│       ├── Page_3.png
│       ├── Page_4.png
│       └── Page_5.png
├── Documentation/
│   ├── Project_Report.pdf
│   └── Presentation.pptx
└── .gitignore
```

Adjust the names and folders to match the files actually present in the
repository. Do not create empty folders just to match this example.

## How to Open the Project

1.  Install or open Microsoft Power BI Desktop.
2.  Clone or download this GitHub repository.
3.  Open the `.pbix` file from the `PowerBI` folder.
4.  If Power BI requests the dataset location, update the source path to
    the dataset file available to you.
5.  Select **Refresh** if the data source is accessible and a refresh is
    required.
6.  Use the page tabs at the bottom of Power BI Desktop to navigate
    between dashboard pages.
7.  Use the slicers to filter the dashboard.

The `.pbix` file is the editable Power BI project. PNG screenshots are
provided for quick viewing and documentation.

## Data and Interpretation Notes

-   The dataset is sourced from Kaggle and should be used in accordance
    with its published description and licence.
-   The dataset is synthetic. Dashboard results describe patterns in the
    supplied dataset and should not be presented as verified real-world
    cyberattacks.
-   A high anomaly score is not, by itself, proof of a confirmed attack.
-   Severity categories and anomaly scores are different measures.
-   An IP address does not independently establish the identity of an
    attacker or victim.
-   Missing values should be handled according to their meaning; a blank
    should not automatically be treated as zero.
-   The selected date range can affect time-based comparisons. Partial
    quarters should not be described as complete quarters.

## Future Work

-   Complete and validate dashboard Pages 3, 4 and 5.
-   Improve alignment, readability and consistency across all dashboard
    pages.
-   Validate DAX measures and slicer interactions across the integrated
    dashboard.
-   Update screenshots, project documentation and presentation material.
-   Review the final Power BI file and repository before submission.

## Acknowledgement

This project was developed collaboratively as part of academic project
work. The team members contributed to data preprocessing, dashboard
development, analysis, validation and documentation.
