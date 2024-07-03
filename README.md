# EOG-BASED-ARROWS-INTERFACE
A human computer interface based on EOG


Data Preparation and Preprocessing: 


1) We began with a dataset comprising 278 text files. Initially, we utilized Python 
code to assign classes to these files based on the following mappings: "Yukari" 
corresponds to "Up", "Asagi" to "Down", "Sag" to "Right", "Sol" to "Left", and "Kirp" 
to "Blink". Through this process, we identified 223 text files that were categorized 
into the five classes, while 55 files remained unassigned to any class. 
Subsequently, we created separate folders for each class and organized the files 
accordingly. Finally, we performed a split of the data within each class into two 
folders: "Train" and "Test", following an 80% to 20% ratio allocation for training and 
testing data, respectively.

2) Preprocessing

  
1) Butterworth band pass filter to preserve EOG band from 0.5 to 20 HZ. 
2) Resampling (we used it at first but removed it: because data is small) 
3) Normalization: Let values be between 0 and 1. 
4) DC component removal: Remove shift effect if exists.


![image](https://github.com/BadrAhmed05/EOG-BASED-ARROWS-INTERFACE/assets/93046762/fdb3555f-b077-4d33-9864-323a213c0429)




Feature Extraction Methods: 
In addition to traditional statistical features extracted directly from the raw 
EOG samples, we explored wavelet-based feature extraction techniques. 
These techniques involved decomposing the EOG signals into different 
frequency bands using wavelet transforms and then extracting statistical 
features from each band. This approach provided a more detailed 
representation of the EOG signals. 
Classifier used and its parameters. 


1) Statistical Features
2) DWT with Statistical Features
3) DWT only



![image](https://github.com/BadrAhmed05/EOG-BASED-ARROWS-INTERFACE/assets/93046762/a877b7a3-4587-44c1-a3f4-fa37e38cf94d)




GUI:


![image](https://github.com/BadrAhmed05/EOG-BASED-ARROWS-INTERFACE/assets/93046762/f1ace024-8f8d-4a54-9fd0-6abda159d8fe)


