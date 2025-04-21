# PBL2-ESC-DXM
This project models the drug-drug interaction between escitalopram (ESC) and dextromethorphan (DXM) and their effects on brain serotonin levels and risk of serotonin syndrome development. The code was written as part of the second project-based learning project for the Spring 2025 BME 260 course at Duke University and serves to provide insight into the pharmacokinetics behind serotonin regulation in the brain. 

The main assumptions for this simulation are outlined below. Additional assumptions can be found in Appendix A of our corresponding written report. 
* The body is representative of that of an average adult man with lower serotonin levels but otherwise healthy . (Used to estimate blood volume, plasma volume, brain weight, etc.)
* The human body is comparable in terms of biology and physiological function to rats. (Allows for the inclusion of data from research conducted with rodents).
* ESC and DXM are the only molecules that bind to SERT. DXM is the only molecule that can bind to sigma-1 receptors. 
* The system is at steady-state with respect to the concentration of ESC throughout the body.


A list of Python files and their use is below.
* ESC-Tracking.py: Calculates steady-state values of brain and plasma escitalopram levels due to escitalopram dose. When provided with an input dose, this file returns and plots the brain and plasma concentration of escitalopram. 
* DXM-Tracking.py: Simulates the pharmacokinetics of dextromethorphan at various doses. Returns and generates plots for percentage of occupied sigma-1 receptors and serotonin release rate as a function of dextromethorphan concentration
* DDI-Integration.py: Combines processes from ESC-Tracking.py and DXM-Tracking,py to simulate the competitive binding of escitalopram and dextromethorphan to SERT and the impact of the drug-drug interaction on time-dependent serotonin concentrations in the synaptic cleft of the brain. When provided with an input dose of escitalopram and dextromethorphan, this file returns calculations and visualizations of serotonin concentration over time. 


