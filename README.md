# STAT-331-Final-Project-Group6
Statistical Analysis Project : D

## Group Members
  * Joey Bailitz 
  * Arneh Begi
  * Brian Kwong 
  * Connor Gamba 

## Abstract

There has often been a standing debate on how transparency and perceived corruption of national leaders has affected one’s economy.  Traditional economic policy would suggest that free democratic and honest governments like those in North America and Western Europe would have the highest GDP per Captia, but in the past 40 years countries in the Middle East and Asia have witness rapid economic growth and corresponding dramatically increasing GDP per Captia authoritarian and opaque government finances.  Is it the case then still that in the 21st century that lower absence of corruption leads to higher GDP per Captia?

## Data Used In Report

The data studied throughout this report is provided by [GapMinder's 2023 IDEA-Democracy Indices Data - v5](https://docs.google.com/spreadsheets/d/1jYUZFQOQrE0bAjV9XVgr_92nMT-_ukYBs4Uom4rfVtQ/edit#gid=501532268&range=B17) and we would be focusing on the following variables:

| Variable | Type | Description |
|--|--|--|
| 🔑Country | String | Full Name of a Country |
| 🔑Year | Int | Year This data was collected
| Country's Absence of Corruption Index | Optional(Double) | A index measuring how corrupt a perceived country's government is.  Lower value means less trust and more corruption.  NA means no data is unavailable for that year.  Please check the section about NA values for some possible reasons |
| GDP Per Captia | Double | Calculated GDP per Captia (GDP/Population) in USD

Entries from the dataset have been limited to the years of 1975-2021 inclusive as 2021 is the most recent available data for a country's Absence of Corruption Index

