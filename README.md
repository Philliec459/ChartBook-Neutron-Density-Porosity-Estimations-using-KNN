# Chart-Book-Neutron-Density-Porosity-using-KNN
The objective of this project is to calculate a Neutron log vs. Bulk Density log Cross-Plot Total porosity using, at this point, the Schlumberger CNL or TNPH Charts as shown below. It is important to use the proper Neutron log associated with the appropriate chart for either fresh or saline fluid densities as specified. The Neutron logs should also be on limestone matrix with these charts. 

![CNL_Image](CNL.png)

![TNPH_Image](TNPH.png)

The name of the Python code is NeutDen_chartbook_porosity_knn_testresults.py. This program uses as training data a matrix of Neutron Porosity (V/V) vs. Bulk Density (G/CC) with known porosities (see below). In this example we are using test data as our log data to observe how well the program is actually working. We have very good agreement between our log analysis chart book training values and the values estimated from this program. 

The porosity estimations are made using KNN. Before we begin any distance calculations, we first normalize the Neutron porosity and Bulk Density curves and then use a KNN of 3 to estimate our Cross-Plot porosity values from our test data set.   

![SMatrixCNL_Image](Matrix_CNL2.png)

![SMatrixTNPH_Image](Matrix_TNPH.png)

This program has been tested for the charts available so far showing good agreement with the training data for our calculated porosities. Further testing is recommended before using this program to better understand the uncertainties in the estimations and validate using a KNN of 3. Please provide feedback if you have any issues.

We are using CNL_1pt1_testdata.xls as log data for testing purposes, but you could use your own log data in lieu of this file to calculate Neutron-Density Total Cross-Plot porosities for your analysis.

We have 4 sets of data files representing 4 of the Schlumberger charts; 2 fluid densities for CNL and 2 for TNPH. Other vendor charts will also be included as needed in the future. 

Constructive criticism and any collaboration are both welcome. 
