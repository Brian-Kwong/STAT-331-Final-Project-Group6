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

## How to Run the Obtain a Copy of the Report

This report is stored on GitHub and can be accessed by cloning the repository using GitHub Desktop, R-Studio GUI environment, Git CLI or downloading the project as a ZIP

For GitHub Desktop simply hit the open in GitHub Desktop option under the green clone button from the main repository. Once it’s done click “Show in Folder” and take note of where the project has been cloned to. Then procced to R Studio and open the .Rproj file from the open project in the menu bar and open the Quarto Document of the report located in the Src Folder[^1]

[^1]: For some versions of GitHub desktop there may be a direct option to open in R Studio 


For R Studio users clone the project by creating a new project, then selecting the Version Control option from the menu.  Then copy the HTTPS URL from green clone button of the main repository [^2].
[^2]: You will need to already have established a connection with GitHub through R Studio ie: auth token before cloning.

For Git CLI users open your terminal and run `git –version` to make sure you have Git Installed. macOS and Linux users should have this installed by default while windows box users will need to obtain a copy of [Git](https://git-scm.com/downloads) from their official website.  Afterwards you can `cd`[^3], into your desired directory and run `git clone git@github.com:Brian-Kwong/STAT-331-Final-Project-Group6.git` to get a copy of the project[^4].  Then procced to R Studio and open the .Rproj file from the open project in the menu bar and open the Quarto Document of the report located in the Src Folder

[^3]: The cd or change directory command is the standard Unix commnand for changing around directories(folders) using the terminal.  It also works on Windows too!

[^4]: Since early 2022 GitHub CLI has required SSH authentication for cloning of repositories. [Learn how to set up SSH Keys for GitHub](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

Lastly you could just download the zip file, by clicking download as zip option from green clone button of the main repository, copy the folder to a desired location and unzip. Then procced to R Studio and open the .Rproj file from the open project in the menu bar and open the Quarto Document of the report located in the Src Folder

Please note to run this project successfully the following R Libraries will need to be installed all of which can be found in the Crayon Package Manager

1. Tidyverse
2. Here
3. Janitor
4. Styler
5. Reactablefmtr
6. Gganimate
7. Gifski
8. Formattable

This code chuck should do the trick in downloading all the necessary packages 
```{r}
install.packages(“tidyverse”)
install.packages("janitor")
install.packages("styler")
install.packages("reactablefmtr")
install.packages("gganimate")
install.packages("gifski")
install.packages("formattable")
```

Lastly please note as this project has quite a few graphics and one 5,000 simulation, rendering and running of the document could take upwards of 10 seconds depending on the processing performance of your computer.
