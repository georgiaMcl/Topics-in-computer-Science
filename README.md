# Blazar Classification

Project Name: Random Forests in High-Energy Astrophyics

The goal of this project was to develop a machine learning algorithm, using the Random Forest model, to classify Blazar Candidates of Uncertain Type (BCUs) from the Fermi-LAT point source catalogues, into the two subclasses of blazars, BL Lacertae (BL Lacs) and Flat-Spectrum Radio Quasars (FSRQs).

The two catalogues analysed were the 3FGL (data from 2008 to 2012 containing 3000 data entries) and 4FGL-DR4 (data from 2008 to 2022 containing 7000 data entries) catalogues.

The Random Forest model was trained on 70% 3FGL BL Lac and FSRQ data, and tested against the remaining 30% BL Lac and FSRQ data.

Another Random Forest model was trained on 100% of the 3FGL BL Lac and FSRQ data, and tested against the 3FGL BCUs with 4FGL-DR4 BL Lac or FSRQ associations.

The files used to develop the model are described below: 

- The yaml file, initialFermi.yaml, contains the details on the conda environment used to run the below Python code files.

- InitialTesting: contains the code and graphs created that were used to analyse the different features of the 3FGL catalogue. This was used to conduct pre-feature selection.

- fermiAnalysis: contains code on feature selection and hyperparameter tuning of the model for the 3FGL data set. This file also contains the Random Forest model evaluation on the 3FGL test set data.

- Compare4FGL: contains code on the 3FGL BCUs with 4FGL BL Lac or FSRQ associations, evaluations and model performance.