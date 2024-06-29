# 1. Introduction
The prupose of this project was to implement a staffing plan for the upcoming Influenza season based on the data collected from previous years.
The findings are then presented in a presentation to stakeholders.

# 2. Busniess understanding

## Project overview
* Motivation: The United States has an influenza season where more people than usual
suffer from the flu. Some people, particularly those in vulnerable populations, develop serious
complications and end up in the hospital. Hospitals and clinics need additional staff to
adequately treat these extra patients. The medical staffing agency provides this temporary
staff.</br >
* Objective: Determine when to send staff, and how many, to each state.</br >
* Scope: The agency covers all hospitals in each of the 50 states of the United States, and
the project will plan for the upcoming influenza season. </br >

Before going into preparing and analyzing the data to find the insights needed and present them to the stake holders a project management plan was set-up to give a clear guidance of how the project will be handled.
This project management plan was presented to the applicable stake holders which are:
* Medical agency frontline staff (nurses, physician assistants, and doctors)</br >
* Hospitals and clinics using the staffing agency’s services</br >
* Influenza patients</br >
* Staffing agency administrators</br >

Below you find some pages of the project management plan:
![stakeholder communication](<screenshots/Stakeholder communication.png>)
![Schedule and milestones](<screenshots/Schedule and milestones.png>)
![Project deliverables](<screenshots/Project deliverables.png>)
![Hypothesis](<screenshots/Hypothesis.png>)</br >
See here for the full [Project Management Plan](<Project Management plan - Influenza season.pdf>)

# 3. Data understanding
## Data sets
* CDC_Influenza_Deaths.xlsx ->  Holds Influenza deaths data from 2009 till 2017 including state, date, Age Groups and death count. Source of this data set is [CDC](https://wonder.cdc.gov/ucd-icd10.html)</br >
* Census_Population_transformed_202101.csv -> Population data by geography, time, age, and gender. Source of this data set is the US Census Bureau [Download data set](<https://coach-courses-us.s3.amazonaws.com/public/courses/data-immersion/A1-A2_Influenza_Project/Census_Population_transformed_202101.csv>)
* CDC_Influenza_Visits.xlsx -> Counts of influenza laboratory test results by state (survey). Source of this data set is [CDC (Fluview)(<https://gis.cdc.gov/grasp/fluview/fluportaldashboard.html>) [Download data set](<https://images.careerfoundry.com/public/courses/data-immersion/A1-A2_Influenza_Project/CDC_Influenza_Visits.xlsx>)
* CDC_Lab_Tests.xlsx -> Counts of influenza laboratory test results by state (survey). Source of this data set is [CDC (Fluview)(<https://gis.cdc.gov/grasp/fluview/fluportaldashboard.html>) [Download data set](<https://images.careerfoundry.com/public/courses/data-immersion/A1-A2_Influenza_Project/CDC_Lab_Tests.xlsx>)
* NIS_Flu_Shot_Survey_reduced.xlsx -> Survey of flu shot rates in children. Source of this data set is [CDC](<https://www.cdc.gov/vaccines/imz-managers/nis/about.html>) [Download data set](<https://images.careerfoundry.com/public/courses/data-immersion/A1-A2_Influenza_Project/NIS_Flu_Shot_Survey_reduced.xlsx>)

## Relevance and limitation of the data sets
Below some relevance and limitations of the Population data set as an example:
### Relevance
* External data source
* US government owns the data
* Since the data is sourced by the government its supposed to be trust worthy

### Data collection method
* Administrative collection.
* Manual collection. Collected by many ways of registration of households. In an instance when its
* Higher up the chain it could be automated. For example when collection of one town is succeeded it can be emailed or send to a database on a state level.
* The time lag is somehow significant since its collected mainly manually and it has to go through many instances till its on state level.

### Limitations
* The limitation is that it cant be updated very frequently since people are always moving and changing their lives. So there is a certain lag in data up to date status.

# 4. Data preparation
## Data cleaning
Before starting any Analysis we need to scan the data for its integrity. Below as an example the integrity check of the CDC_Influenza_Deaths.xlsx data set.
![Data cleaning](<screenshots/Cleaning.png>)
![Data integrity](<screenshots/Data integrity.png>)

### Find and eliminate duplicates
Duplicates are idnetified by producing a pivot table for each year by state and county. After applying the "delete duplicates" function in excel the pivot table to indentify the duplicates was refreshed to check if all duplicates were eliminated.
In this example below the "Census_population_transformed_202101" data set is shown.</br >
![Duplicates](<screenshots/eliminate duplicates.png>)</br >

### Data integration
After cleaning and integrity checks are excecuted its time to ontegrate the two cleaned data sets "Influenza deaths" and "Population" with eachother so they can be used in further Analysis and visualizations.
Before the integration can be executed a data mapping has to be done for evaluating on which variable to combine the two data sets.
![Data integration](<screenshots/Data integration.png>)</br >







