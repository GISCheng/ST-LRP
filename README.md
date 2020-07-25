# ST-LRP

## Title: A method to assess spatio-temporal units for specific tasks based on explainable artificial intelligence

## Abstract
Big geo-data are commonly aggregated into spatio-temporal units before the analysis of human activities and urban environments. Many applications categorize these data into groups and compare data characteristics across groups. The intergroup differences vary with spatio-temporal units, and the key is to identify the spatio-temporal units with apparent differences in data characteristics across groups. However, spatio-temporal dependence, data variety, and the complexity of tasks impede effective unit assessment. Inspired by the applications to extract critical image components based on explainable artificial intelligence (XAI), we propose a spatio-temporal layer-wise relevance propagation method to assess spatio-temporal units as a general solution. The method organizes input data into an extensible three-dimensional tensor form. We provide two means of labeling the spatio-temporal tensor data for typical geographical applications, using temporally or spatially relevant information. Neural network training proceeds to extract the global and local characteristics of data for corresponding analytical tasks, and then the method propagates classification results backward into units as evaluated importance. We validate the method through a case study with taxi trajectory data in Beijing. The results prove that the proposed method can assess spatio-temporal units with dependence for specific tasks. This study also attempts to discover task-related knowledge using XAI.

## Statement
The program of the ST-LRP is developed based on the previous work of LRP in Github ([TensorFlow LRP Wrapper](https://github.com/VigneshSrinivasan10/interprettensor)) (Lapuschkin et al. 2016).
Lapuschkin, S., et al., 2016. The LRP toolbox for artificial neural networks. The Journal of Machine Learning Research, 17 (1), 3938-3942.

## Code description
1. The file "interprettensor(revision).zip" is the zip package of the main programs in this study. All the programs are the Jupyter Notebook files in python (.ipynb):
(1) The file "Holiday_revise_2019.ipynb" is the program of neural network model training and the spatio-temporal unit evaluation.
(2) The file "Validation1_revise_Replaced zones.ipybb" is the program of the first validation experiment (replace the zone value of input).
(3) The file "Validation2_Regression_POI.ipynb" is the program of the second validation experiment (interpretation of unit importance measure difference based on POI data).
(4) The file "Validation3_Random forests.ipynb" is the program of the third validation experiment (use random forests to evaluate units).
(5) The file "Validation4_Cluster.ipynb" is the program of the fourth validation experiment (data compression application).
2. The file "Trained Parameters.zip" is the zip package of trained neural network parameters.

## Data
The data that support the findings of the study are available in [figshare.com](http://doi.org/10.6084/m9.figshare.9981314) with the permanent link. The data include the training set, validation set, and test set of the model training (i.e. taxi origin point distributions collected in the years of 2016 and 2017) and the inputs for the subsequent validation experiments.

## Cite
