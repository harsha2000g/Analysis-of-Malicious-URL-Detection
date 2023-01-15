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

![Alt text](D:\Projects\"Analysis of Malicious URL Detection"\"Images for ReadMe"\"Data Distribution.png"?raw=true "Title")


