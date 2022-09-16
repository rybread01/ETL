# Project-2 - Group 2
## GROUP MEMBERS: Kellimarie Cooper, Ryan Kim, Natalia Moreno, Myles Browne
## Observations:
  After analyzing the data, the maximum number of deaths was 760 from Fetanyl in 2018 from durg overdose.  From 2012-2016, heroin caused the highest number of overdose
  deaths at 174, 257, 325, 416, and 494 from 2012-2016 respectively.  From 2017-2018, fetanyl was the leading cause of death at 676 and 760.  Overall, there is no      major association between over-all per capital income in the United States.  A better comparison of income and drug overdose deaths would best be done with neighborhood or county income and employment rates.
 
 
![income and overdose](https://customsitesmedia.usc.edu/wp-content/uploads/sites/59/2019/02/16042905/Opioids-in-America-web-824x549.jpg)


## Data sets:
* [Drug Overdose Deaths CSV File](https://www.kaggle.com/datasets/ruchi798/drug-overdose-deaths)
* [U.S.A. Income Data Csv file](https://apps.bea.gov/iTable/iTable.cfm?reqid=70&step=1&ac)
 
## Context:
According to the Center for Disease Control and Prevention, in 2020 Drug overdoses from substances such as opioids, cocaine, psychostimulants, and others, were the leading cause of injury-related death in the United States. While the ongoing drug overdose crisis has primarily been fueled by opioid use, it is important to note that overdoses related to other drug categories are also on the rise.

The demand-side perspective argues that the drug overdose epidemic is a consequence of changes in the economy that leaves behind working-class people who lack a college education. In contrast, the supply-side perspective maintains that the epidemic is primarily due to changes in the licit and illicit drug environment. A third distinct perspective argues that income inequality is likely a key driver of the epidemic considering that Socioeconomic status and the vulnerability it creates contributes immensely to the overdose health crisis.

While overdose deaths are preventable, there are still barriers remaining due to the lack of understanding of these different perspectives. The goal of the present project is to contribute to the studies of these perspectives by providing a consolidated database with useful information from trustworthy sources that can help uncover patterns and relationships between income per capita and overdoses.
 
## Proposal:
 
The objective of this project is to analyze deaths from varying drug overdoses from 2012 through 2018 in relation to per capita personal income by integrating the data found utilizing the ETL approach.
 
  ### EXTRACT:
  - In a jupyter notebook, we loaded in both of our necessary datasets from the original CSV files to get them ready for transformation.

  ### TRANSFORM

  - As we transformed our csv files into working dataframes, we encountered many different problems such as wrong datatypes, null data, and different date formats used in each source. 
  - One thing that we as a group had to discuss was how exactly we wanted our dataframes to be related to one another. At first the tables were related  by state; but, it was too troublesome attempting to get them ready for our analysis, so we ended up going by the year.


  ### LOAD
  - Using postgres and sqlalchemy we uploaded our cleaned tables into postgres so we could query our data. 
