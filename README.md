# Project: Report Data Visualization 

This project analysis data of pharmaceutical research. They want to track a treatment onto 250 mice for skin cancer. Then the visualization will show the evaluation of some drugs treatment. In addition, the final purpose of this project is to show my skills to collect data and plot them using python libraries, for instance, matplotlib and pandas. 

## Getting Started

Download the files and run the pymaceuticals_starter.ipynb, which is a jupyter notebook extension. 

### Prerequisites
You must have Python installed in your machine; for this reason, the best option is to download Anaconda because it also installed some important libraries.

## Running this development

Perform this pymaceuticals_starter.ipynb file into your jupyter notebook

# Data Analysis
First of all, two csv files were imported  into a dataframe using pandas:
* File to Load (Remember to Change These)
> mouse_drug_data_to_load = "data/mouse_drug_data.csv"
> clinical_trial_data_to_load = "data/clinicaltrial_data.csv"

* Read the Mouse and Drug Data and the Clinical Trial Data
> mouse_drug_data = pd.read_csv(mouse_drug_data_to_load)
> clinical_trial = pd.read_csv(clinical_trial_data_to_load)

* Second, the two data frame were merged using a common field:
> merge_data = pd.merge(mouse_drug_data,clinical_trial,on="Mouse ID")

After the steps above, it was possible to create a specific Data frame to generate the plots below: 

1. Creating a scatter plot that shows how the tumor volume changes over time for each treatment.

![GitHub Logo](/Pymaceuticals/png/Tumor_response_treatment.png)

2. Creating a scatter plot that shows how the number of metastatic (cancer spreading) sites changes over time for each treatment.

![GitHub Logo](/Pymaceuticals/png/Metastatic_spread_during_treatment.png)

3. Creating a scatter plot that shows the number of mice still alive through the course of treatment (Survival Rate)

![GitHub Logo](/Pymaceuticals/png/Survival_during_treatment.png)

4. Creating a bar graph that compares the total % tumor volume change for each drug across the full 45 days.

![GitHub Logo](/Pymaceuticals/png/Tumor_change_over_45_day_treatment.png)

## Built With

Python

## Versioning

Version 1.0

## Acknowledgments

1.	Python
2.	Libraries: 
a.	Panda
b.	Matplotlib
3.	IDE - jupyter notebook
