# Title: "Prediction of thermogravimetric data in bromine capture from Brominated Flame Retardants (BFRs) in e-waste treatment using Machine Learning approaches"


# Authors: Ali, Labeeb; Sivaramakrishnan, Kaushik; Kuttiyathil, Mohamed Shafi; Chandrasekaran, Vignesh ; Ahmed, Oday; Al-Harahsheh, Mohammad; Altarawneh, Mohammednoor

Thermal treatment of bromine-contaminated polymers (i.e., as in e-waste) with metal oxides is currently deployed as a mainstream strategy in recycling and resources recovery from these objects. The principal aim in this treatment is to release and capture the bromine from the brominated flame retardants (BFRs) added to the polymeric constituents of printed circuits boards (PCBs) and to produce pure bromine-free hydrocarbons. Tetrabromobisphenol A (TBBA) is the most commonly utilized model compound as a representative for BFRs. Among notable deployed metal oxides is calcium hydroxide, i.e., Ca(OH)2 that has shown to exhibit high debromination capacity. Our co-authors have previously studied the pyrolytic and oxidative decomposition of TBBA:Ca(OH)2 mixture at four different heating rates 5, 10, 15, and 20 °C/minusing a Thermogravimetric (TGA) analyzer and reported the mass loss data between room temperature and 800 oC. In the kinetic literature, models such as Starink iso-conversional model-free methods were able to find the key kinetic parameters such as activation energy (Ea), pre-exponential factor (A), and the accuracy of the models. However, in the current work, we applied different machine learning (ML) and chemometric techniques involving regression models to predict the TGA data at different heating rates. The objective here was to reproduce the TGA data with high accuracy by eliminating the physical need of the instrument so that this saves experimental time involving sample preparation and minimizing human errors. The number of datapoints in the conditions of pyrolysis and the oxidation were 18626, 9319, 6217, and 4672, at heating rates of 5, 10, 15 and 20 oC/min, respectively. Three ML models were employed in our work, namely: Linear, random forest (RF) and support vector regression (SVR), out of which the RF method exhibited the highest coefficient of determination (R2) of 0.999 and least error of prediction as estimated by the root mean squared error (RMSEP) at all the 4 heating rates. An 80:20 split was used for calibration and validation data sets. Furthermore, for showing versatility and robustness of the best-predicting RF model, it was also trained using all the data points in the lower heating rates of 5 and 10 oC/min and predicted on all the data points for the higher heating rates of 15 and 20 oC/min to again obtain a high R2 of 0.999. The excellent performance of the RF model showed that ML techniques can be used to eliminate the physical use of TGA equipment and thus, saving experimental time and potential human errors and can be applied in other real-time recycling scenarios.  


1. You can find the wrangling script [here](https://github.com/vigchandra/TGA_ANN_pred/blob/master/wrangling/Data_Engineering_n2.ipynb)

   Data input can be found [here](https://github.com/vigchandra/TGA_ANN_pred/blob/master/data/TGA%20data%20with%20graphs%20(N2).xlsx)
   
   Data output can be found [here](https://github.com/vigchandra/TGA_ANN_pred/blob/master/data/consolidated_2022-10-13_v1]) 
   
2. You can find the modelling script [here](https://github.com/vigchandra/TGA_ANN_pred/blob/master/model/Modelling.ipynb)

   Model input can be found [here](https://github.com/vigchandra/TGA_ANN_pred/blob/master/data/consolidated_2022-10-13_v1)
   
   Model output can be found [here](https://github.com/vigchandra/TGA_ANN_pred/tree/master/output)
