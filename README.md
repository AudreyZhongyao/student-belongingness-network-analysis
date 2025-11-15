Student Belongingness Network Analysis
Psychological network analysis examining the relationship between student belongingness and mental health in university settings. This project is part of PhD research at University College London investigating how different aspects of belongingness relate to mental health outcomes across diverse student populations.
Overview
This repository contains R code and outputs for analyzing psychological networks of student belongingness and mental health using data from 18,000+ university students. The analysis employs network theory to understand:

Central belongingness and mental health constructs
Network stability and consistency across different measurement approaches
Variation in network structure across demographic groups (school year, race/ethnicity, gender)

Repository Contents
Analysis Scripts

Healthy_Mind_Network2.Rmd - Main R Markdown file containing the complete network analysis pipeline, including data processing, network estimation, stability analysis, and visualization generation

Results and Outputs

centrality_rankings_table.csv - Summary table of centrality measures for all network nodes, showing which variables are most central in the psychological network

Visualizations
Network Structure

overall_network.png - Complete psychological network showing relationships between belongingness and mental health variables
school_year_networks.png - Network comparisons across different school years to examine developmental patterns
race_networks_all.png - Network comparisons across racial/ethnic groups
male_female_networks.png - Gender-based network comparison

Stability and Robustness

network_stability_combined.png - Network stability analysis showing robustness of centrality estimates
stability_results.png - Additional stability coefficients
consistency_plots_grid.png - Consistency analysis across different measurement approaches

Methods
This analysis uses psychological network analysis to model belongingness and mental health as a system of interconnected variables rather than latent constructs. Key analytical approaches include:

Network estimation: Regularized partial correlation networks using graphical LASSO
Centrality analysis: Strength, betweenness, and closeness centrality measures
Stability analysis: Case-dropping bootstrap procedures to assess robustness
Network comparison: Testing for structural differences across groups

Required R Packages
r# Network analysis
library(qgraph)
library(bootnet)
library(NetworkComparisonTest)

# Data manipulation and visualization
library(dplyr)
library(tidyr)
library(ggplot2)

# Additional packages (install as needed)
library(igraph)
library(psychonetrics)
Usage

Ensure all required packages are installed
Open Healthy_Mind_Network2.Rmd in RStudio
Note: Raw data is not included in this repository due to privacy and ethical considerations
The code can be adapted for similar psychological network analyses with appropriate data

Research Context
This work contributes to understanding how different dimensions of belongingness (individual, interpersonal, organizational, and community levels) relate to mental health outcomes in higher education settings. The analysis examines whether network structures vary across demographic groups and measurement approaches.
Data Privacy
In accordance with research ethics protocols, individual-level student data is not included in this repository. The code and visualizations demonstrate the analytical approach and can be adapted for similar research questions.
Citation
If you use or adapt this code for your research, please cite:
Zhang, A. (2025). Student Belongingness Network Analysis [R]. GitHub. https://github.com/AudreyZhongyao/student-belongingness-network-analysis

Contact
For questions about the methodology or potential collaborations:
zhongyao.zhang.19@ucl.ac.uk
PhD Candidate, Experimental Psychology, University College London
Education Policy Intern, UNESCO Paris

License
This project is available for academic and educational purposes. Please contact for commercial use inquiries.
