# Analysis-of-Malicious-URL-Detection

## PROJECT OVERVIEW
### MALICIOUS URLs
Malicious URLs are essentially malicious websites hosted by attackers to bait users into their sites for malevolent purposes. These purposes include phishing, spam, or malware dropping. As the purpose varies, the working and intent of the websites differ, classifying them into various categories. The following types of malicious URLs and their classifications are explored during the research.
Phishing: Luring ignorant users into revealing their confidential information such as passwords, credit card numbers, bank details, etc by pretending to be authentic and impersonating them for personal gain.
Malware: Dropping various kinds of malware such as viruses, worms, trojans, etc into the system when a user clicks the URL.
Defacement: URLs that have been defaced for motives such as political agendas, ruining an organization’s image, gaining popularity, etc.
Spam: Spamming URLs to a large number of users for commercial gain, self-promotions, etc.

### URL CLASSIFICATION
A machine learning multi-class classification model has been developed to classify whether a given URL is benign, that is a safe/legitimate site or a malicious site. If it is a malicious website, the model detects the type of malicious URL it is using a 5-Class Classification. Several preprocessing steps have been used in conjunction with the machine learning model to obtain the desired output.

### RESEARCH ELEMENT
Although the main objective of the project is to build a model to detect and identify malicious URLs, another goal is to compare and gauge the methodologies used to build models and assess their performances while achieving the primary objective.
To identify the best system, different feature groups and data analysis techniques have been used in conjunction. This analysis gave various insights into the detection of malicious URLs. The models are evaluated based on how accurate they are in classifying the URLs.


## TOOLS AND TECHNOLOGY
### OVERVIEW 
This section discusses the tools and technologies used during the course of the project. The following items were preferred after thorough consideration of the system design and implementation.

### PYTHON
Python, being an interpreted and high-level language can be used for many purposes which can be contributed to the fact that it is easy to use and is open-source. It can be used to implement a wide range of concepts from artificial intelligence and data science to web development.

### ANACONDA
Anaconda is a distribution of python that provides libraries, tools, and softwares required for projects based on machine learning, deep learning, data science, etc. It also gives access to interactive development environments like Jupyter Notebook and Spyder. It also provides a multitude of libraries such as Numpy, Pandas, Tensorflow, and Matplotlib.

### NUMPY
NumPy is a python library that is distinctively used for the purpose of numerical computations. This is because of its ability to carry out mathematical operations quickly and efficiently. This can be attributed to the fact that NumPy integrates C and C++  functions into the python framework, giving it exceedingly higher speeds compared to normal python libraries. Different kinds of data pre-processing techniques are performed using NumPy such as vectorizing the feature embeddings, splitting data, saving large arrays of data, etc.

### MATPLOTLIB AND SEABORN
Seaborn and Matplotlib are python libraries used for the purpose of visualization. It helps plot the data into meaningful and easy-to-understand visualizations. These libraries provide a wide range of plots and visuals that integrate well with the Jupyter environment as well as libraries like NumPy.

### SKLEARN
Sklearn is a machine learning library that provides straightforward and efficient data analytics and machine learning tools. It supports various tasks such as Classification, Regression, Clustering, Preprocessing, Model Selection, and Dimensionality Reduction. Various data pre-processing functions, machine learning algorithms, and metrics were used from this library.

### PYRQA
PyRQA is a python library that helps implement RQA in an efficient manner. It uses the OpenCL framework to parallelize the processes and speed up the operations so that it is time-efficient. It is able to do so with the help of OpenCL which uses both GPU and CPU for faster computations.

### JUPYTER NOTEBOOK IDE
Anaconda platform provides various multi-purpose software and services under Anaconda Navigation such as Visual Basic, Spyder, RStudio, PyCharm, etc. Jupyter Notebook is one such web-hosted application that provides an interactive interface for python with a large set of functions.

## DATASET
### The development of models that employ character-level embedding and a 5-class classification requires a proper distribution of the classes along with differing lexical styles. This is because the machine learning algorithms need to identify the patterns that differentiate between the classes and provide legitimate outputs. The Canadian dataset, ISCX-URL2016 has over one lakh sixty-five thousand data points where five classes are distributed in an uneven distribution.

![Alt text](https://github.com/harsha2000g/Analysis-of-Malicious-URL-Detection/blob/master/Analysis%20of%20Malicious%20URL%20Detection/Data%20Distribution.PNG?raw=true "Title")

## DATA HANDLING AND PRE-PROCESSING
This section involves loading, cleaning, and organizing the data. Since there are three kinds of classification implemented and evaluated, data preparation becomes the key. The classification types are

Benign Vs Malicious URLs: This is a direct binary classification where benign URLs are assigned the integer 0 while all the malicious URLs (phishing, malware, spam, and defacement) are assigned the integer 1.

Benign Vs Malicious URLs Class-wise: This is also a binary classification but instead of taking all the malicious URLs, each individual class is pitted against benign URLs.

5-Class Classification: This is a multi-classification where each URL class is assigned a unique integer from zero to four.

## FEATURE EXTRACTION / FEATURE EMBEDDINGS
For machine learning algorithms to work, the input features are to be provided, so it is crucial to extract features that best showcase and preserve the information from the raw data which in this case are the URLs. As the raw data is textual, the limelight of this project was on the lexical aspect of the URLs. Three different kinds of feature groups were chosen for analysis as shown below.

![Alt text](Features Table?raw=true "Title")

## FEATURE ANALYSIS AND MODEL SELECTION
This stage is the most important stage of the project as the feature inputs are selected and the models are finalized here. All three features are compared and additional features are also added as the input on top of the selected feature group.
After thorough research, the best data analysis technique usable and producing considerable improvements in the performance of the model is RQA. RQA (Recurrence Quantification Analysis) is a non-linear data analysis technique that focuses on the recurrence aspect of the characters. The RQA measures are able to bring out significant information about occurrences of characters within a URL. The following fifteen measures were used during the analysis:
-Recurrence rate
-Determinism
-Average diagonal line length
-Longest diagonal line length
-Divergence
-Entropy diagonal lines
-Laminarity
-Trapping time
-Longest vertical line length
-Entropy vertical lines
-Average white vertical line length
-Longest white vertical line length
-Entropy white vertical lines 
-Ratio determinism / recurrence rate 
-Ratio laminarity / determinism 

## EVALUATION AND HYPER-PARAMETER TUNING
Once the feature analysis is completed, the models will be evaluated based on the metrics accuracy, precision, recall, F1 score, and log loss. These metrics for both training and testing will be observed after performing a 5-fold cross-validation. This is done so as to confirm the performance of a model instead of taking just one test set and judging the model’s ability. With five folds the training and the testing split will be 80:20 which is optimal. Once the best models for various features are finalized, hyper-parameter tuning is executed to identify the model’s best state. The exhaustive grid search is used for hyper-parameter tuning.

## Results
### BENIGN VS MALICIOUS URLS Best Models

![Alt text](R1.1?raw=true "Title")
![Alt text](R1.2?raw=true "Title")
![Alt text](R1.3?raw=true "Title")

### BENIGN VS MALICIOUS URLS CLASS-WISE Best Models

![Alt text](R2?raw=true "Title")

### 5-CLASS CLASSIFICATION Best Models

![Alt text](R13.1?raw=true "Title")
![Alt text](R3.2?raw=true "Title")

### RQA

![Alt text](R4?raw=true "Title")

