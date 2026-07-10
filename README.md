# HFOV during neonatal transport

Jupyter Notebooks used for processing and analysis of clinical and ventilator parameters.


This repository contains the Python code used for data processing, statistical analysis and visualization described in the following paper:

Balog V, Liszkay G, Lantos L, Jermendy A, Belteki G. High-frequency oscillatory ventilation with or without volume guarantee during neonatal transport. *J Perinatol.* 2025 Jan;45(1):43-49. doi: 10.1038/s41372-024-02109-9. Epub 2024 Sep 6. PMID: 39242946.


Contact: gbelteki@aol.com; gusztav.belteki@nhs.net 

____


The outputs (numbers, tables, graphs) of the cells of the Jupyter Notebooks (.ipynb files) have been suppressed in order to comply with copyrights.
Some of the corresponding data and graphs can be found in the paper and its supplementary material.

This code can be viewed in any web browser. If the code is displayed (rendered) in Github, copy and paste the URL (web adress) of the Notebook into [nbviewer](https://nbviewer.jupyter.org) for a read-only display.

To run the code, you can use Jupyter installed locally on your computer or [Google Colab](https://colab.research.google.com).

Raw data are not shared but users can run the code on their own data obtained in the same format.

____

Packages required to run this Notebook: numpy, pandas, matplotlib, scipy. For versions of Python and the add-on packages see the Notebooks. 

I recommend downloading these packages using the freely availably Anaconda built: [https://anaconda.org](https://anaconda.org)

____

# Jupyter Notebooks


### A. Initial processing of raw ventilator slow (0.5 Hz) data

These notebooks perform the initial processing of ventilator data (including ventilator parameters, settings, alarms (0.5Hz sampling rate). Dictionaries containing the processed ventilator data exported as pickle archives: **data_pars_xxx_xxx.pickle** 

Data downloaded from the **fabian +HFOi ventilator**:           cases AT000001 - AT000818
1. [ventilator_data_new_1_150](ventilator_data_new_1_150.ipynb):          AT000001 - AT000150
2. [ventilator_data_new_151_300](ventilator_data_new_151_300.ipynb):      AT000151 - AT000300
3. [ventilator_data_new_301_450](ventilator_data_new_301_450.ipynb):      AT000301 - AT000450
4. [ventilator_data_new_451_600](ventilator_data_new_451_600.ipynb):      AT000451 - AT000600
5. [ventilator_data_new_601_750](ventilator_data_new_601_750.ipynb):      AT000601 - AT000750
6. [ventilator_data_new_751_900](ventilator_data_new_751_900.ipynb):      AT000751 - AT000900
7. [ventilator_data_new_751_900](ventilator_data_new_901_1050.ipynb):     AT000901 - AT001050
8. [ventilator_data_new_1051_1200](ventilator_data_new_1051_1200.ipynb):  AT001051 - AT001200
9. [ventilator_data_new_1201_1350](ventilator_data_new_1201_1350.ipynb):  AT001201 - AT001350 (Only recordings up to AT001251 were included in this study)


### B. Processing clinical data

[clinical_data_new_1_1397](clinical_data_new_1_1397.ipynb): Processing of clinical data related to recordings AT000001 - AT001397. (Only cases up to AT001251 were included in this study). 

### C. Processing of blood gases

II. [blood gases_new_1_1397](blood_gases_new_1_1397.ipynb): Processing of clinical data related to recordings AT000001 - AT001397. (Only cases up to AT001251 were included in the study).

### D. Further processing of slow (0.5Hz) ventilator data

[ventilator_data_processing_new_1_1305](ventilator_data_processing_new_1_1305.ipynb):  Further processing of the 0.5 Hz ventilator data (measurements, settings and alarms) for recordings AT000001 - AL001305. (Only recordings up to AT001251 were included in this study) 
 
### E. Manual trimming of the recordings

[ventilator_data_trimming_new_1_1305](ventilator_data_trimming_new_1_1305.ipynb): In this Notebook, recordings have been individually inspected and trimmed to remove periods when the ventilator was working but the patient was not connected. (Only recordings up to AT001251 were included in this study) 


### F. Analysis of clinical and ventilator data of infants transferred on HFOV with or without VG

1. [HFOV_processing](HFOV_processing.ipynb): Processing of recordings containing HFOV during neonatal transport.
2.  [HFOV_processing_2](HFOV_Processing_2.ipynb): Further processing and analysis of ventilator data in HFOV recordings.
3.   [HFOV_analysis](HFOV_analysis.ipynb): Analysis of ventilator data and blood gases of the included HFOV cases (**n=51**). Export statistics as Excel files and graphs. Produce graphs for the figures of the paper.  
