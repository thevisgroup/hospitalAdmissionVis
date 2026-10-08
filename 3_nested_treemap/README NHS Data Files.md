# README: NHS Data Files



This folder contains the Excel files used for the analysis and visualisation of NHS admissions data presented in the accompanying research paper.



\----------------------------------------------------------------------------------------------------



### Files Included



sortingData.xlsx

FinalNHSData\_Vertical.xlsx



\----------------------------------------------------------------------------------------------------



##### sortingData.xlsx: 



This file contains the raw NHS records after being transcribed and standardised for analysis. Where inconsistencies occurred between source records, headings were amended to ensure consistency across years.



Where only total admissions and male admissions were available in earlier records, female admissions were calculated as:



Female Admissions = Total Admissions − Male Admissions



The file was used to organise the data, identify and resolve inconsistencies, and prepare the dataset for subsequent visualisation.



The workbook contains two worksheets:



All years by code

Records are organised by diagnosis, with diagnoses presented in the same order for each year and sorted according to their summary code.



All years by admissions

Records for each year are ordered according to the total number of admissions for each diagnosis, from highest to lowest. This structure was used as the basis for the subsequent Tableau dataset.



Both worksheets contain the following variables, where available:



* Summary Code
* Description
* Admissions
* Male
* Female
* Gender Unknown
* Emergency Admissions
* Waiting List
* Planned Admissions
* Mean Age



The Gender Unknown category reflects records containing unidentified or inconsistent gender information however is missing from 2016–2017 due to errors in the source records



\----------------------------------------------------------------------------------------------------



##### FinalNHSData\_Vertical.xlsx



This file contains the prepared dataset imported into Tableau for data visualisation. It is derived from the All years by admissions worksheet in sortingData.xlsx.



Unlike sortingData.xlsx, where individual years are presented in separate sections for ease of human interpretation, this file uses a vertical data structure. Each observation occupies a separate row, with the corresponding year explicitly recorded for each observation.



This restructuring was necessary to provide Tableau with a consistent tabular format suitable for data visualisation and analysis. Although the vertical format is less convenient for direct manual inspection, it allows the visualisation software to correctly interpret year, diagnosis, and admission variables as dimensions and measures.



\----------------------------------------------------------------------------------------------------



##### Data Preparation Summary



The overall data preparation process therefore consisted of:



Transcribing and consolidating the NHS source records.

Standardising headings and variable names across years.

Resolving inconsistencies within the source data.

Calculating female admissions where these could be derived reliably from total and male admissions.

Organising records by diagnosis code and, separately, by admission volume.

Restructuring the admission-ordered data into a vertical format compatible with Tableau.

Importing the resulting FinalNHSData\_Vertical.xlsx dataset into Tableau for visualisation.



These files are provided to document the data preparation and transformation process underlying the analysis reported in the research paper.



\----------------------------------------------------------------------------------------------------



Kerry Clifford

University of Nottingham

2026



\----------------------------------------------------------------------------------------------------

