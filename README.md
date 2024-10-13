# MS-Point
A Peak Quality Assessment Tool for Untargeted Metabolomics Data Employing Machine Learning


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
