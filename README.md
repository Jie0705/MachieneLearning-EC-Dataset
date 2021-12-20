# MachieneLearning-EC-Dataset
This is the repository for dataset that were used in paper:
Physics-Informed XGBoost Model forElectrocaloric Temperature Change Predictions in Ceramics

The data sets were gathered from published papers. The material composions are epanded into 145 Magpie features [*Ward, L., Agrawal, A., Choudhary, A., & Wolverton, C. (2016). A general-purpose machine learning framework for predicting properties of inorganic materials. npj Computational Materials, 2(1), 1-7.*] 
and are stored along with the extracted data in the csv files. Below are the data descriptions for separate files. 

## 1. EC_data_DeltaT.csv
The electrocaloric (EC) ceramics dataset for EC temperature changes. The first column is the index, followed by the 145 Magpie features from the elemental chemical properties, then the material composition (in comma-separated Magpie format), 
the Curie temperature (*T<sub>Curie</sub>*), characterization temperature (*T*) and electric field (*E*), EC temperature change (*ΔT<sub>EC</sub>*), and the measurement conditions (*pol* and *method*). 
The source of the data (figure number and the paper from which the data are extracted) are also included as two separate columns, *PaperID* (denoted as year_first author last name_first two words from title_material abbreviation) and *FigID*. 


## 2. EC_data__DielectricConstant.csv
The extracted dielectric constant for materials in EC_data_DeltaT.csv (if the values are reported in original literature). 
The first column records the material composition and the following columns are *T<sub>Curie</sub>*, *T*, dielectric constant (*ε*), measured frequency, and *PaperID*. 

## 3. ferroelectrics_data.csv
This file contains ferroelectrics ceramics whose are not reported for the EC effect. This file takes a similar format as EC_data_DeltaT.csv, except they do not have columns related to EC temperature change measurement 
(i.e., *E*, *pol*, *method*, and *ΔT<sub>EC</sub>*). Instead, the frequency at which the dielectric constant is measured is recorded as *Frequency*. 

## 4. EC_FamilyGroups.csv
This file contains a full list of material compositions with their abbreviated family group for the EC materials. 

## 5. PaperID_references.csv
This file contains a full list of *PaperID* with corresponding literature DOI for the EC materials.
A similar list for ferroelectric ceramics are in the last two columns of ferroelectrics_data.csv.

### * Note: 
All temperatures in these files are in °C, the electric fields are in kV/cm, and the frequencies are in Hz. 

