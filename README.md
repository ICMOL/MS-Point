# Introduction
      Metabolomics investigates the complete set of small molecules within a biological system. Liquid chromatography coupled with tandem mass spectrometry (LC-MS/MS) is a powerful technique used in metabolomics to identify and quantify small molecules with high sensitivity and precision. Several software tools have been developed for metabolite quantification from LC-MS/MS-based metabolomics data, but few focus on peak quality evaluation. Therefore, we developed MS-Point, an innovative tool for automated peak quality evaluation.  MS-Point is a cross-platform, command-line tool developed in Java, designed to ensure broad compatibility and ease of use. It will automatically label the input data and generates the training dataset. Logistic regression is then applied using a five-fold cross-validation approach, utilizing nine quality metrics as features to ultimately produce a quality score ranging from -1 to 1 for each peak. A higher quality score indicates better quality of the detected features.
    
  ![image](https://github.com/ICMOL/MS-Point/blob/main/ms-point_workflow.png)
        Figure 1. The workflow of MS-Point, including automatically generating training dataset and producing quality score with logistic regression.
        
## nine quality metrics


## System Requirement
* [Java SE Runtime Environment 15(or above)](https://www.oracle.com/java/technologies/javase/jdk15-archive-downloads.html)
  
## Parameter Description

|parameter|description|
| ------------- | ------------- |
|input_folder_directory| contain the txt file(s) output from MS-Picker|
|output_folder_directory| the folder that all analyze results you want to put in|
|k_fold| "k" for k-fold cross-validation|

# How to Use
* java -jar MS-Point k_fold input_folder_directory output_folder_directory
* java -jar MS_Point_v1.2.jar 5 D:\\input_folder D:\\output_folder 
