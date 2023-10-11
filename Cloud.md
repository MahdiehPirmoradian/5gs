### Project: ML22/23 28 Improve Unit Test Spatial Pooler
|   |   |  
|---|---|
| Issue  | [Issue 89](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/issues/89)  |  
| Team  |  Team_Codec  |  
|  Author |  [Jasim](https://github.com/MJ1307)
|  Author |  [Faizan](https://github.com/SyedFaizan18) 
| Source Code  |  [Project](https://github.com/MJ1307/neocortexapi/tree/Team_AP/source/MySEProject/MultiSequenceLearning) |   
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/Team_Codec/MyProject/Improve%20Unit%20Test(Spatial%20Pooler%20and%20Temproal%20Memory)/Documentation/Improve%20Unit%20Test%20(%20Spatial%20Pooler%20and%20Temporal%20Memory).pdf)|
## Project Title : ML 21/22 28 Improve Unit Test Spatial Pooler
--------------------------------------------------------------------------------------------

**Project Description**
========================



﻿
# Software Engineering Batch Projects (2019-2023): Documentation and Code Links

*  [Project_ML22-23](#projects_22-23)
*  [Project_ML21-22](#projects_21-22)
*  [Project_ML20-21](#projects_20-21)
*  [Project_ML19-20](#projects_19-20)


# Projects_22-23 
*  [Score ✯✯✯](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#score-)
*  [Score ✯✯](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#score--1)
*  [Score ✯](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#score--2)



## Score ✯✯✯
* [ML22/23- 1 Scalar Encoder with Buckets](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2223--1-scalar-encoder-with-buckets)
* [ML22/23- 2 Investigate and Implement KNN Classifier](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2223--2-investigate-and-implement-knn-classifier)
</br></br>  
### Project: ML22/23- 1 Scalar Encoder with Buckets

|   |   |  
|---|---|
| Issue  | [Issue 80](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/issues/80)  |  
| Team  |  Team_SpiralGanglion  |  
|  Author |  [Singari Sahith Kumar](https://github.com/sahithkumar1999)
|  Author |  [Anil Kumar Gadiraju](https://github.com/anilkumargadirajuFraUas) 
|  Author |  [Vinay Kumar Bandaru](https://github.com/Vinaykumarbandaru1999)
| Source Code  |  [Scalar Encoder](https://github.com/sahithkumar1999/neocortexapi_Team_SpiralGanglion/blob/test-cases/source/UnitTestsProject/EncoderTests/ScalarEncoderTests.cs) |   
| Documentation  |  [Readme](https://github.com/sahithkumar1999/neocortexapi_Team_SpiralGanglion/blob/test-cases/source/Documentation(Scalar%20Encoder%20With%20Buckets-%202022-2023)/Readme.md) |   


#### Abstract
Scalar encoders with buckets are useful in a variety of real-world scenarios where continuous values must be represented as discrete values. This is frequently used in the case of machine learning and data analysis like converting a continuous characteristic such as age, temperature, or height into a categorical feature that may be used in a model or algorithm. Sensor data analysis is one common application for scalar encoders. The buckets approach overcomes limitations such as limited precision, flexibility, and Periodic Encoding. This means that the scalar encoder's accuracy will be limited due to the mapping of continuous input values to a discrete set of data, and it will be less adaptable and more difficult to modify to different datasets because it requires the user to set parameters such as the number of min/max values and radius. Furthermore, non-periodic encoding is a Scalar Encoder constraint that may be problematic for specific input data. As a result, this paper analyses the Scalar Encoder's shortcomings and how they might be overcome by combining the Scalar Encoder with Buckets.
</br></br>


### Project: ML22/23- 2 Investigate and Implement KNN Classifier
|   |   |  
|---|---|
| Issue  | [Issue 77](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/issues/77)  |  
| Team  |  Team_KNN  |  
|  Author |  [Ankush Patil](https://github.com/ankush-patil22)
|  Author |  [Ayan](https://github.com/ayan1948) 
|  Author |  [NasirIshaq](https://github.com/NasirIshaq)
| Source Code  |  [IClassifier.cs](https://github.com/ayan1948/neocortexapi/blob/master/source/NeoCortexApi/Classifiers/IClassifier.cs) |   
| Source Code  |  [Predicator.cs](https://github.com/ayan1948/neocortexapi/blob/master/source/NeoCortexApi/Predictor.cs) |
| Source Code  |  [SDRClassifier.cs](https://github.com/ayan1948/neocortexapi/blob/master/source/NeoCortexApi/Classifiers/SDRClassifier.cs) |
| Source Code  |  [HtmUnionClassifier.cs](https://github.com/ayan1948/neocortexapi/blob/master/source/NeoCortexApi/Classifiers/HtmUnionClassifier.cs) |
| Documentation  |  [Readme](https://github.com/ayan1948/neocortexapi/blob/master/source/MySEProject/README.md) |   



#### Abstract
Machine learning (ML) has grown over a wide range of sectors such as finance, education, communication, transportation, retail, and healthcare. In response to this, researchers have developed a variety of algorithms to analyze a large amount of data and derive quantifiable insights from that data. Subsequently, ML has a different range of algorithms to support text, image, audio, video, and numeric formats, and based on the application ML can predict the outcomes. Supervised learning, a machine learning type, uses classification and regression to analyze the data. In general, several types of classifiers are present under supervised machine learning, such as decision trees, support vector machines, naive Bayes, and K-nearest neighbors (KNN) designed under this section. In this paper, we have proposed the implementation of the most widely used k-nearest neighbor (KNN) machine learning algorithm used to predict the outcome variable or dependent variable based on the input variables or independent variables. KNN classifier can be used with HTM by incorporating it as a sub-module for classification tasks. Precisely, HTM models can learn to represent the input data in a high-dimensional feature space and then use the KNN classifier to classify the data based on the closest neighbors in this feature space. This can be useful in situations where the input data has a complex temporal structure and requires a more sophisticated approach to classification than simple threshold-based methods. So, the developed kNN model is also integrated with the Neocortex API to get the input dataset from Hierarchical temporal memory (HTM).  The designed KNN model gets a stream of sequences as input from HTM and then classifies whether the predicated sequence matches or mismatches with the input data sequence with 80% accuracy. Additionally, the design procedure, challenges, and enhancements to improve model accuracy are discussed in the paper.
</br></br>


## Score ✯✯
* [ML22/23- 7 Implement UnitTests for AdaptSegments](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2223--7-implement-unittests-for-adaptsegments)
* [ML22/23- 9	Implement Serialization of HtmClassifier](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2223--9implement-serialization-of-htmclassifier)
* [ML22/23- 11 Improve UnitTests for Temporal Memory Algorithm](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2223--11-improve-unittests-for-temporal-memory-algorithm)
* [ML22/23- 12 Implement Anomaly Detection Sample](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2223--12-implement-anomaly-detection-sample)
* [ML22/23- 15 Approve Prediction of Multisequence Learning](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2223--15-approve-prediction-of-multisequence-learning)

</br></br>


### Project: ML22/23- 7 Implement UnitTests for AdaptSegments 
|   |   |  
|---|---|
| Issue  | [Issue 99](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/issues/99)  |  
| Team  |  Team_UnitTestAS  |  
|  Author |  [Jishnu Shivaraman](https://github.com/jishnuS-GitHub)
|  Author |  [Kavya Hirebelaguli Chandrashekar](https://github.com/kavyahc-github) 
|  Author |  [Madhushree Manjunatha Lakshmidevi](https://github.com/Madhulakshmi)
| Source Code  |  [Project](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/tree/Team_UnitTestAS/SE%20Project%20-%20Team_UnitTestAS) |   
| Documentation  |  [Documentation](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/tree/Team_UnitTestAS/SE%20Project%20-%20Team_UnitTestAS/Documentation%20of%20project) |   


#### Abstract
Hierarchical temporal memory is the technique that works on the principles of neocortex. A computational model called Temporal Memory is based on how the neocortex of the brain organizes and stores information. The process of updating Temporal Memory's representation of a segment in response to fresh data is referred to as adapting segments.  Adapt Segment checks to see if a new input pattern matches any of the pre-existing segments before acting on it. The primary goals of the project involve developing comprehensive unit test cases for the AdaptSegment method, to ensure its correct functionality in the HTM algorithm and also achieving full code coverage by utilizing the Code Coverage tool. The team created a set of unit tests for the AdaptSegment method, which is a critical component of the Temporal Memory class. Through rigorous testing and modification, the team was able to develop highly effective unit tests that covered all possible tests. The "AdaptSegment" method in the HTM class is responsible for adjusting the permanence values of synapses in a given distal dendrite segment based on the activity of their presynaptic cells in the previous cycle. When a synapse's permanence drops below a threshold, it is eliminated, and if all synapses in a segment are eliminated, the entire segment is also eliminated. Unit Tests have been designed and implemented in the project SE Project - Team_UnitTestAS.
</br>
#### Keywords
Neo Cortex, Hierarchical Temporal Memory, Temporal Memory, Adapt Segments, Unit Test.
</br></br>




### Project: ML22/23- 9	Implement Serialization of HtmClassifier
|   |   |  
|---|---|
| Issue  | [Issue 75](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/issues/75)  |  
| Team  |  Team_Alpha  |  
|  Author |  [Amith Nair](https://github.com/antonyaneeta/neocortexapi/commits/amith_nair)
|  Author |  [Rohit Suresh](https://github.com/antonyaneeta/neocortexapi/commits/rohit_suresh) 
|  Author |  [Aneeta Antony](https://github.com/antonyaneeta/neocortexapi/commits/aneeta_antony)
| Source Code  |  [Project-Serialize method](https://github.com/antonyaneeta/neocortexapi/blob/98ca46e17b8efe842471deaed73c530068ded8ef/source/NeoCortexApi/Classifiers/HtmClassifier.cs#L501) | 
| Source Code  |  [Project-Deserialize method](https://github.com/antonyaneeta/neocortexapi/blob/98ca46e17b8efe842471deaed73c530068ded8ef/source/NeoCortexApi/Classifiers/HtmClassifier.cs#L522) | 
| Documentation  |  [Readme](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/team_alpha/MySEProject/Documentation/README.md)|   


#### Abstract
Serialization is the act of transforming an object or data structure into a format that is simple to store, send, or exchange with other systems or applications. A text-based format, a binary stream, or any other structured file format can be used for the serialized representation. This paper focuses on the implementation of serialization in the Hierarchical Temporal Memory (HTM) classifier and demonstrates how the parameters of the HTM classifier can be serialized. A machine learning method called the HTM classifier learns and anticipates patterns in time-series data using the neocortex's structural layout. In this project, the serialization functionality of HTM Classifier in C#/.NET Core is implemented for Neocortex API. Serialization in the HTM classifier enables the classifier to preserve its state and structure as a file, enabling it to maintain its state over different runs or transfer its state to a different machine. It is helpful for picking up where training stopped off and incorporating the classifier into different programs or frameworks. We have carried out several unit tests by comparing the serialization and deserialization results in order to validate our methods.
</br>

#### Keywords
Classifier, Hierarchical Temporal Memory, Sparse Distributed Representation, neocortex.
</br></br>


### Project: ML22/23- 11 Improve UnitTests for Temporal Memory Algorithm
|   |   |  
|---|---|
| Issue  | [Issue 83](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/issues/83)  |  
| Team  |  variable-i  |  
|  Author |  [Syed Mostain Ahmed](https://github.com/Mostainahmed)
|  Author |  [Farjana Akter](https://github.com/farjana-akter-shifa) 
|  Author |  [Md. Shamsir Doha](https://github.com/shamsirdoha2118)
|  Author |  [Md. Nabuat Al Jahid](https://github.com/MdNabuatAlJahid)
| Source Code  |  [Project](https://github.com/Mostainahmed/variable-i/blob/master/source/UnitTestsProject/TemporalMemoryTest2.cs) |   
| Documentation  |  [Readme](https://github.com/Mostainahmed/variable-i/blob/master/source/MySEProject/Documentation/ImproveUnitTestsforTemporalMemoryAlgorithm.md)|



#### Abstract
Temporal memory algorithms have gained popularity as a promising approach for modeling temporal sequences in machine learning. This project aims to improve the unit test for the given temporal memory algorithm, which is based on the principles of the cortical column and the neocortex. The algorithm uses a sparse distributed representation of data and incorporates temporal context to predict future values in a sequence. We implemented improvements to the existing unit test, including the addition of more test cases with varying complexity and the implementation of cross-validation techniques for better evaluation of the algorithm's performance. We also optimized the implementation of the algorithm for improved efficiency and scalability.
</br>

#### Keywords
Temporal memory algorithm, Cortical column, Neocortex, Sparse distributed representation.
</br></br>



### Project: ML22/23- 12 Implement Anomaly Detection Sample
|   |   |  
|---|---|
| Issue  | [Issue 90](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/issues/90)  |  
| Team  |  Team_Anomaly  |  
|  Author |  [Anurag De](https://github.com/anuragdeFUAS)
|  Author |  [Sourav Paul Sumit](https://github.com/SouravPaulSumit) 
| Source Code  |  [Project](https://github.com/SouravPaulSumit/Team_anomaly/tree/master/mySEProject/AnomalyDetectionSample) |   
| Documentation  |  [Documentation](https://github.com/SouravPaulSumit/Team_anomaly/tree/master/mySEProject/Documentation)|




#### Abstract
HTM (Hierarchical Temporal Memory) is a machine learning algorithm, biologically inspired, both structurally and functionally, by the neocortex of a human brain, which uses a hierarchical network of nodes to process time-series data in a distributed way. Each node, or column, can be trained to learn and recognize patterns in input data. This can be used to process information, recognize, and identify patterns, and make future predictions based on past learning. It is a promising approach for anomaly detection and prediction in a variety of applications in sectors, such as healthcare, finance, etc. We have implemented an anomaly detection sample using HTM, such that it learns multiple simple numeric integer sequences given to the HTM model as input and tries to learn patterns in it. It will then try to identify anomalies by comparing the real data with the predicted data from learning, with a certain threshold of tolerance.
</br>
#### Keywords
HTM, anomaly detection, machine learning, multi-sequence learning
</br></br>





### Project: ML22/23- 15 Approve Prediction of Multisequence Learning
|   |   |  
|---|---|
| Issue  | [Issue 89](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/issues/89)  |  
| Team  |  Team_AP  |  
|  Author |  [Jasim](https://github.com/MJ1307)
|  Author |  [Faizan](https://github.com/SyedFaizan18) 
| Source Code  |  [Project](https://github.com/MJ1307/neocortexapi/tree/Team_AP/source/MySEProject/MultiSequenceLearning) |   
| Documentation  |  [Readme](https://github.com/MJ1307/neocortexapi/blob/Team_AP/source/MySEProject/MultiSequenceLearning/Documentation/README.md)|


#### Abstract
Current artificial networks mostly rely on dense representations, whereas biological networks rely on sparse representations. Hierarchical Temporal Memory is a specific realization of the Thousands Brains Theory that generates motor commands for interacting with the environment and testing predictions. In our research paper, we demonstrate how a sequence is learned using Multsequence Learning algorithms. A subsequence is used to calculate accuracy and how we calculate the accuracy. To perform the experiment, some tasks have been automated such as creating a synthetic dataset as per configuration, saving the dataset to a file, reading the dataset, and writing the results to a file performed to support our results.
</br>

#### Keywords
Hierarchical Temporal Memory, Spatial Pooler, Temporal Memory, encoder, sparse dense representation, AI, ML, HTM.
</br></br>







## Score ✯
* [ML22/23- 6 Implement Unit-Tests for the SpatialPooler AdaptSynapses Method](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2223--6-implement-unit-tests-for-the-spatialpooler-adaptsynapses-method)
* [ML22/23- 11 Improve UnitTests for Temporal Memory Algorithm](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2223--11-improve-unittests-for-temporal-memory-algorithm-1)






### Project: ML22/23- 6 Implement Unit-Tests for the SpatialPooler AdaptSynapses Method
|   |   |  
|---|---|
| Issue  | [Issue 88](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/issues/88)  |  
| Team  |  Project_X  |  
|  Author |  [Jenny Nadar](https://github.com/jennadar)
|  Author |  [Sriram Karunanithi](https://github.com/Sriram-Karunanithi) 
|  Author |  [Kumar Satyam](https://github.com/Kumarsatyam1) 
| Source Code  |  [AdaptSynapses.cs](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/Project_X/Source/MySEProject/Project_X/UnitTest/AdaptSynapses.cs) |   
| Documentation  |  [Readme](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/Project_X/Source/MySEProject/Project_X/Readme.md)|




#### Abstract

Implementing unit tests in software development is significant because it helps ensure that individual components of the software function correctly and reliably. However, unit testing is often considered to be an arduous task. This study employs the implementation of unit tests for the AdaptSynapses method in the Spatial Pooler (SP) algorithm used in the Hierarchical Temporal Memory (HTM) architecture, which is a computational framework inspired by the structure and function of the neocortex. To ensure the reliability and robustness of the method in different situations, we created a diverse range of test case scenarios to test the provided AdaptSynapses method with changing threshold values and Permanence values. During the task accomplishment, we gained valuable insights into how this method connects mini-columns and sensory input. As part of our efforts, we also analyzed many existing unit tests by introducing a range of inputs with varying complexity. Finally, with the visual studio feature, we did cross-validation of the test cases to evaluate the algorithm's performance. We observed all the test cases successfully cover the complete test AdaptSynapses method in the SpatialPooler class. Hence all of them resulted in 100% code coverage. The study effectively motivated us to write unit tests that are more comprehensive and of higher quality.
</br></br>




### Project: ML22/23- 11 Improve UnitTests for Temporal Memory Algorithm
|   |   |  
|---|---|
| Issue  | [Issue 84](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/issues/84)  |  
| Team  |  Shinigami_developer  |  
|  Author |  [Md Maruf Hossain](https://github.com/ryanmaruf615)
|  Author |  [Mousumi Parvin tonni](https://github.com/MousumiTonny) 
|  Author |  [Aktari Sadia Sabah](https://github.com/SadiaSabah) 
| Source Code  |  [TemporalMemory.cs](https://github.com/ryanmaruf615/neocortexapi/blob/dev/source/NeoCortexApi/TemporalMemory.cs) |   
| Documentation  |  [Readme](https://github.com/ryanmaruf615/neocortexapi/blob/dev/source/MySEProject/Documentation/Readme.md)|



#### Abstract

Temporal memory algorithms have gained popularity as a promising approach for modeling temporal sequences in machine learning. This project aims to improve the unit test for the given temporal memory algorithm, which is based on the principles of the cortical column and the neocortex. The algorithm uses a sparse distributed representation of data and incorporates temporal context to predict future values in a sequence. We implemented improvements to the existing unit test, including the addition of more test cases with varying complexity and the implementation of cross-validation techniques for better evaluation of the algorithm's performance. We also optimized the implementation of the algorithm for improved efficiency and scalability. Moreover, running this project on Azure Cloud, we explored and got to use very useful features of Azure Cloud services.
</br></br></br></br>







# Projects_21-22 
*  [Score ✯✯✯](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#score--3)
*  [Score ✯✯](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#score--4)
*  [Score ✯](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#score--5)





## Score ✯✯✯
*  [ML21/22- 1.2.Analyse Image Classification](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2122--12analyse-image-classification)
*  [ML21/22- 1.2.Analyse Image Classification (MNIST)](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2122--12analyse-image-classification-mnist)
*  [ML21/22- 1.2.Analyse Image Classification (Fruits 360 dataset)](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2122--12analyse-image-classification-fruits-360-dataset)
*  [ML21/22- 24. Investigate Label Prediction from the time-series sequence (Power Consumption))](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2122--24-investigate-label-prediction-from-the-time-series-sequence-power-consumption)





 
### Project: ML21/22- 1.2.Analyse Image Classification
|   |   |  
|---|---|
| Issue  | [Issue 189](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/issues/189)  |  
| Team  |  Metaverse  |  
|  Author |  [MahdiehPirmoradian](https://github.com/MahdiehPirmoradian)
|  Author |  [Omid Nikbakht](https://github.com/onikbakht) 
| Source Code  |  [Code](https://github.com/MahdiehPirmoradian/neocortexapi-classification/blob/167ab147593348c16c4813e33e2d91be72a928db/MySEProject/ImageClassification/Experiment.cs#L153) |   
| Documentation  |  [Readme](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/blob/Metaverse/MySEProject/Documentation/README.md)|


#### Abstract
The purpose of this paper is to investigate a new approach to image classification based on an open HTM version algorithm, a revolutionary biologically inspired model of the mammalian neocortex's structure, to maximize crucially influencing parameters of the HTM model predicting more precisely when applied to the categorized Hand Drawn Shapes. The primary goal was to investigate the open-source implementation of the Hierarchical Temporal Memory in C#/.NET Core. By conducting more than 100 experiments for different HTM configurations, the behavior of the system is observed and documented using diagrams to get a vivid overview of
the dependency of HTM on each of the modified parameters. Afterward, a set of parameters, which have shown better results of HTM functionality are discussed and proposed. Followed by, implementing a prediction code in the project, which enables the HTM system to anticipate the category of an entered test input image.
Keywords—Hierarchical Temporal Memory (HTM), Sparse Distributed Representation (SDR), Spatial Pooler (SP), Inhibition, Global Inhibition, Local Inhibition, Potential Radius, Local Area Density, Active Column, Inhibition Area, Neocortex, Visual Pattern Recognition.
</br></br>



### Project: ML21/22- 1.2.Analyse Image Classification (MNIST)
|   |   |  
|---|---|
| Issue  | [Issue 188](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/issues/188)  |  
| Team  |  CodeCube  |  
|  Author |  [Aiman Zehra](https://github.com/AimanZehra)
|  Author |  [Alam Sher Khan](https://github.com/Alam-Sher-Khan) 
|  Author |  [Soundarya Talawai](https://github.com/SoundaryaTa) 
| Source Code  |  [Code](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/tree/Team_CodeCube/MySEProject) |   
| Documentation  |  [Readme](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/blob/Team_CodeCube/MySEProject/Documentation/README.md)|


#### Abstract
This paper gives the evaluation of HTM when applied to image classification and the prediction of images. HTM (hierarchical temporal memory) is a cognitive learning
system that aims to replicate the neocortex's operating principles. The primary objective of this paper is to examine the HTM parameters that result in the highest similarity for the image of the same label/class and the lowest similarity between images of different classes for the MNIST (Modified National Institute of Standards and Technology) dataset. Another objective is to provide the prediction code for image classification so that after learning, the system can classify the image based on the training dataset. To achieve these goals, we have conducted experiments for training the MNIST images using the previously implemented Image Classification solution as a library and also implemented the prediction code for image classification using similarity threshold.

#### Keywords 
Hierarchical Temporal Memory (HTM), Image classification, Sparse Distributed Representation (SDR), Prediction code, Local Area Density, Potential Radius, Local/Global Inhibition, Spatial Pooler (SP)
</br></br>



### Project: ML21/22- 1.2.Analyse Image Classification (Fruits 360 dataset)
|   |   |  
|---|---|
| Issue  | [Issue 192](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/issues/192)  |  
| Team  |  CodeChasers  |  
|  Author |  [Veena Alphonsa Jose](https://github.com/VeenaAlphonsa)
|  Author |  [Anu Maria Varghese](https://github.com/Anumari) 
|  Author |  [Tiniya Vinod Puthanpurayil](https://github.com/TiniyaVinod) 
| Source Code  |  [Code](https://github.com/VeenaAlphonsa/neocortexapi-classification/tree/main/MySEProject) |   
| Documentation  |  [Readme](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/blob/veenajose/Documentation/README.md)|


#### Abstract
Image classification is the process of categorizing and labeling groups of pixels or vectors within an image based on specific rules. It is the most important part of digital image analysis. This paper aims to change various Hierarchical Temporal Memory (HTM) learning parameters to find the best fit that shows the image classification and to demonstrate how these parameters influence learning. Our objective is to improve the input prediction and to implement the highest similarity of the input images. The HTM Cortical Learning Algorithm (HTM CLA) Spatial Pooler (SP) is a neocortical-inspired Cortical Learning Algorithm for learning. In this project, NeoCortex API focuses implementation of the Hierarchical Temporal Memory Cortical Learning Algorithm in C#/.NET Core. Its purpose is to understand the spatial pattern by creating the input's Sparse Distributed Representation code (SDR). HTM is based on the biological functions of the brain as well as its learning mechanism. To achieve our goals, we have conducted various tests using the Fruit360 dataset with the previously implemented image classification solution as a library and implemented the prediction code with the highest similarity of input images.
</br>

#### Keywords
Spatial Pooler, Hierarchical Temporal Memory, Sparse Distributed Representation, neocortex.
</br></br>




### Project: ML21/22- 24. Investigate Label Prediction from the time-series sequence (Power Consumption)
|   |   |  
|---|---|
| Issue  | [Issue 170](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/issues/170)  |  
| Team  |  PredictionWarriors  |  
|  Author |  [Mandar](https://github.com/i-am-mandar)
|  Author |  [Amar](https://github.com/Amarfrauas) 
|  Author |  [Chandanl](https://github.com/chandandevsingh) 
| Source Code  |  [NeoCortexApi.sln](https://github.com/i-am-mandar/neocortexapi/blob/master/source/NeoCortexApi.sln) |   
| Documentation  |  [Readme](https://github.com/i-am-mandar/neocortexapi/blob/master/source/MySEProject/Documentation/README.md)|



#### Abstract
Most artificial networks today depend upon dense representations, whereas biological networks rely on sparse representations. The term hierarchical temporal memory describes a specific realization of the thousands Brain Theory, and it generates motor commands to interact with the surroundings and test the predictions. In the time-series, datetime is converted to a fixed time frame as a segment. In this paper, we show how we encode segments as Sparse Distributed Representations (SDRs) for use in HTM systems. It uses the field of AI to predict the label according to the time-series sequence. The task here is to implement sequence learning and prediction code that learns the sequence. The date and time are to be encoded in order to be used in spatial pooler and HTM. The temporal memory then learns the multi-sequence learning according to the date and time as well as the power consumed at that specific segment.
</br></br>





## Score ✯✯
*  [ML21/22- 24. Investigate Label Prediction from the time-series sequence (Taxi Passenger)](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2122--24-investigate-label-prediction-from-the-time-series-sequence-taxi-passenger)
*  [ML21/22- 25.Multi-Sequence Learning Project (WS21/22) Project](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2122--25multi-sequence-learning-project-ws2122-project)
*  [ML21/22- 23. Implement Trace SDR Method](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2122--23-implement-trace-sdr-method)
*  [ML21/22- 24. Improve Unit Test ( Spatial Pooler and Temporal Memory)](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2122--24-improve-unit-test--spatial-pooler-and-temporal-memory)
*  [ML21/22- 30. Test and Investigation of Video Learning Project(WS21/22)](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2122--30-test-and-investigation-of-video-learning-projectws2122)




  

### Project: ML21/22- 24. Investigate Label Prediction from the time-series sequence (Taxi Passenger)
|   |   |  
|---|---|
| Issue  | [Issue 179](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/issues/179)  |  
| Team  |  CodeWarriors  |  
|  Author |  [Md Rizwanul Islam](https://github.com/Rizwanul-Islam)
|  Author |  [MD Rabiul Islam](https://github.com/rabiul64) 
|  Author |  [Md Jubayar Hossain](https://github.com/jubayar) 
| Source Code  |  [Code](https://github.com/rabiul64/neocortexapi/tree/master/source/MySEProject/TimeSeriesSequence) |  
| Documentation  |  [Readme](https://github.com/rabiul64/neocortexapi/blob/master/source/MySEProject/Documentation/README.md)|



#### Abstract
Label prediction from time-series sequence has been widely applied to the finance industry in applications such as stock market price and commodity price forecasting. In recent years, machine learning algorithms have become increasingly popular in label prediction from time-series sequences. There is a time-series sequence of values in many industrial scenarios, for example, a sequence that shows the number of taxi pick-ups at a specific time. A popular problem is how to label time series data to measure the forecast accuracy of machine learning models and, as a result, ultimate investment returns. Existing time series labeling approaches mostly label data by comparing current data to data from a short period in the future. This paper represents an investigation of label prediction from the time series sequence and implements the code for multisequence learning and prediction to address the above problem. The sequence in HTM is learned by the htmClassifier.Learn() method. For this approach, it assumes that the label can be the number of passengers and the second argument of the Learn function is the encoded time-series value. Then it encodes the date and time as a combined encoding of two scalar values and reduces the time precision to a specific time using segmentation of one hour. After that, it predicts using the trained model, then examines the outcome and calculates the accuracy. The results of the paper also proved that the label prediction from the time series data set using multisequence learning is the best choice for dealing with the prediction of a specific time.
</br></br>



### Project: ML21/22- 25.Multi-Sequence Learning Project (WS21/22) Project
|   |   |  
|---|---|
| Issue  | [Issue 180](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/issues/180)  |  
| Team  |  Team Noobies  |  
|  Author |  [Gaurav Honnavara Manjunath](https://github.com/gauravhm96)
|  Author |  [Harish Palanivel](https://github.com/harishpalani12) 
|  Author |  [Prajwal Praveen](https://github.com/prajwalpraveen97) 
| Source Code  |  [Code](https://github.com/harishpalani12/neocortexapi/tree/gauravhonnavara_ProjectWork/source/MySEProject/SimpleMultiSequenceLearning/SimpleMultiSequenceLearning) |  
| Documentation  |  [Readme](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/blob/harish_palanivel_se_2021-22/Documentation/README.md)|


#### Abstract
In real-life situations, the prediction and perception of temporal sequences for sensory inputs are helpful/critical. Based on multiple known features of neurons, a theoretical framework known as HTM (hierarchical temporal memory) is used for sequence learning. The HTM model replicates the neocortex's operating principles which handle learning of sequences and storing the trained data in the memory and can perform prediction Operations until the right match. This paper evaluates the HTM Prediction Engine when applied to a sequence of Numbers, Sequence of Alphabets (Anti – anti-cancer peptide Cells), and Set of Images to predict the sequences of numbers, Sequence of Alphabets, and Images. The primary objective is to examine the HTM prediction Engine and understand Multi sequence Learning for a Sequence of Numbers, upon which, A prediction algorithm is developed for a Sequence of Alphabets for predicting a set of alphabets that belong to a particular sequence (To Predict Anti–Cancer Peptide Cells) and also to develop Multi Sequence Learning for Image Data sets can predict whether a specific Image belongs to the Training Image data Sets.
</br></br>



### Project: ML21/22- 23. Implement Trace SDR Method
|   |   |  
|---|---|
| Issue  | [Issue 201](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/issues/201)  |  
| Team  |  Infinity  |  
|  Author |  [Aishin Abdulla Yoosufali](https://github.com/aishincp)
|  Author |  [Ang Ngawang Sherpa](https://github.com/Angnawang) 
| Source Code  |  [Code](https://github.com/aishincp/neocortexapi/tree/Infinity/My_Project/Trace_SDR_Method) |  
| Documentation  |  [Readme](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/blob/Aishin_AbdullaYoosufali/My_Project/Documentation/Implement_Trace_SDR_Method.md)|


#### Abstract
In Hierarchical Temporal Memory, the underlying Spatial Pooler algorithms generate continuous SDR which are encoded with some input or sequence. The activation of neurons is not always the same for every sequence. This experiment aims to describe the two SDR sequences taken to investigate the two slightly different sets of encoded inputs by using a new method that will differentiate the SDR values and manifest the dissimilarity in both the traced sequences SDR. The different sets of inputs in both SDR lists have semantic similar inputs. Every bit in SDR is not designated with any value or name, but it has a semantic meaning that is to be learned. The experiment we did here, shows the work of the two SDRs which have the active bits in similar locations, and in some locations, there are dissimilar or inactive bits and both SDR sets allot the same semantic attributes because of the active bits in the same place. In the investigation we proposed here, there is an overlap between both the SDRs as they have somewhere same set of active bits, so we can immediately compare the two representations which are semantically similar, and differentiate the parts or bits that are dissimilar. Within one set of neurons, an SDR at one point in time can associatively link to the next occurring SDR. 
</br>

#### Keywords 
Hierarchical Temporal Memory, Sparse
Distributed Representation, Spatial Pooler
</br></br>




### Project: ML21/22- 24. Improve Unit Test ( Spatial Pooler and Temporal Memory)
|   |   |  
|---|---|
| Issue  | [Issue 190](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/issues/190)  |  
| Team  |  UnitCodeMaster  |  
|  Author |  [Ali Haider](https://github.com/alihaidershafique)
|  Author |  [Naveed Ahmed](https://github.com/naveed401) 
|  Author |  [Ali Raza Kharl](https://github.com/alirazakharl) 
| Source Code  |  [SpatialPoolerTests.cs](https://github.com/alihaider4189/neocortexapi/blob/UnitCodeMaster/source/UnitTestsProject/SpatialPoolerTests.cs) | 
| Source Code  |  [TemporalMemoryTests.cs](https://github.com/alihaider4189/neocortexapi/blob/UnitCodeMaster/source/UnitTestsProject/TemporalMemoryTests.cs) |
| Documentation  |  [Readme](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/blob/UnitCodeMaster/MyProject/Improve%20Unit%20Test(Spatial%20Pooler%20and%20Temproal%20Memory)/README.md)|


#### Abstract

Hierarchical temporal memory is the technique that works on the principles of neocortex. Spatial Pooler and Temporal Memory are the important components of HTM. It
transforms the binary input patterns into the sparse distribution representation which then acts as an input to the temporal memory algorithm to make predictions. Temporal Memory learns sequences of Sparse Distributed Representations (SDRs) formed by the Spatial Pooling algorithm and makes predictions of what the next input SDR will be. Unit tests run to maintain code health, ensure code coverage, and find errors and faults before your customers do. Run your unit tests frequently to make sure your code is working properly.
</br>

### Keywords 
Neo Cortex, Spatial Pooler, Temporal Memory, Sparse Distribution Representations, Unit Test
</br></br>



### Project: ML21/22- 30. Test and Investigation of Video Learning Project(WS21/22)
|   |   |  
|---|---|
| Issue  | [Issue 185](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/issues/185)  |  
| Team  |  Seeker  |  
|  Author |  [Nghia Nguyen](https://github.com/notuni109)
|  Author |  [Kandil Khaled](https://github.com/KandilKhaled) 
| Source Code  |  [Code](https://github.com/notuni109/neocortexapi/tree/master/source/GroupSEProject/HTMVideoLearning) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/blob/Nghia/Documentation/Investigation%20of%20Video%20Learning%20Project%20Report.pdf)|


#### Abstract
The main purpose of the project is to test and investigate the Video Learning project. In order to do that, different video inputs were provided to the program and applied with various parameters in the configuration. Afterwards, the results are carefully documented for each experiment, which are demonstrated as data tables. It is observed that the project performed decently on average, along with some great exceptions under specific conditions. Overall, the Video Learning process has been developed properly, and only a few adjustments to the configuration in the code of the program are required so that the trained model can achieve even better performance.
</br></br>





## Score ✯
*  [ML21/22- 1.1 Analyze and Describe Boosting Algorithm](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2122--11-analyze-and-describe-boosting-algorithm)
*  [ML21/22- 1.2.Analyse Image Classification](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2122--12analyse-image-classification-1)
*  [ML21/22- 1.8.Improve UnitTests (HTMClassifier)](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2122--18improve-unittests-htmclassifier)
*  [ML21/22- 1.2.Analyse Image Classification (use simple artificial images 1)](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2122--12analyse-image-classification-use-simple-artificial-images-1)




### Project: ML21/22- 1.1 Analyze and Describe Boosting Algorithm
|   |   |  
|---|---|
| Issue  | [Issue 181](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/issues/181)  |  
| Team  |  Devil_Coders  |  
|  Author |  [Sandhya-Bagadi](https://github.com/sandhyabagadi)
|  Author |  [Kiran-Atirala](https://github.com/kirankumar-Athirala) 
|  Author |  [Chinmaya-Dimmiti](https://github.com/Chinmaya-Dimmiti) 
| Source Code  |  [Code](https://github.com/sandhyabagadi/neocortexapi/tree/Devil_Coders/source/MySEProject) | 
| Documentation  |  [Readme](https://github.com/sandhyabagadi/neocortexapi/blob/Devil_Coders/source/MySEProject/Documentation/ReadMe.md)|


#### Abstract
This paper represents Analysing and Describing of Boosting Algorithm that uses Spatial Pooler and Spatial Pattern Learning. This algorithm uses a boosting algorithm that makes sure that the unused mini columns and weak synapses periodically get boosted. The main idea behind boosting is that the SDRs of symbols use a wider range of cells by making the most active cells less active and the least active cells more active. This is done via scalar multiplication of a boosting matrix over the spatial pooler to change the permeances of each cell. It may be concluded that the boosting process has an impact on the SP stability. The SP can reach a stable state, but SDRs with a drastically different number of active mini-columns will result. If boosting is turned on, the SP will activate mini-columns equitably, but the learning will be unstable. We also performed experiments to obtain stability of Spatial Pooler output by tuning the boost and duty cycles. We evaluated each of these parameters based on the theoretical and practical framework and summarized the results in graphical diagrams.
</br></br>





### Project: ML21/22- 1.2.Analyse Image Classification
|   |   |  
|---|---|
| Issue  | [Issue 186](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/issues/186)  |  
| Team  |  Acroaticus  |  
|  Author |  [Niloy Sarker](https://github.com/Niloy-Sarker96)
|  Author |  [Samsil Arefin](https://github.com/samsil2) 
| Source Code  |  [Code](https://github.com/Niloy-Sarker96/neocortexapi-classification/tree/Team_Acroaticus) | 
| Documentation  |  [Readme](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/blob/Niloy-Sarker/Documentation/README.md)|


#### Abstract
The method of categorizing and labeling bunches of pixels or vectors inside a picture utilizing particular rules is known as image classification. It is the foremost significant component of advanced image analysis. The objective of this paper is to look into an approach to image classification that’s based on an open Hierarchical Temporal Memory (HTM) form algorithm. The HTM Cortical Learning Algorithm (HTM CLA) Spatial Pooler (SP) could be a learning calculation propelled by the neocortical framework. Its objective is to comprehend the spatial design by producing a Sparse Distributed Representation code from the input (SDR). HTM may be a cognitive learning framework and a progressive naturally propelled show of the neocortex’s structure that’s utilized to maximize basic affecting parameters of the HTM demonstrated in arrange to anticipate more accurately when connected to encoder output pictures. We performed a set of tests in this paper to decide the most excellent parameter combination for accomplishing great and exact likeness between encoder output pictures.
</br></br>





### Project: ML21/22- 1.8.Improve UnitTests (HTMClassifier)
|   |   |  
|---|---|
| Issue  | [Issue 193](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/issues/193)  |  
| Team  |  CodeBD  |  
|  Author |  [Debasish Dutta](https://github.com/debasishdtt)
| Source Code  |  [Code](https://github.com/Arup-gope/neocortexapi/tree/codebd/MyProject/HtmClassifierUnitTest) | 
| Documentation  |  [Readme](https://github.com/Arup-gope/neocortexapi/blob/codebd/MyProject/HtmClassifierUnitTest/Documentation/22-1.8.%20Improve%20UnitTests(HtmClassifier).md)|


#### Abstract
This study provides Hierarchical Temporal Memory (HTM), a machine learning approach that uses Spatial Pooler, Scalar Encoder, and Temporal memory where Unit Tests
are done on the learned data to be congruent with the expected output. Hierarchical Temporal Memory (HTM) theory, which represents the structural and algorithmic aspects of the neocortex, has recently developed a new paradigm in machine intelligence. There is still a lot of work to be done on the HTM algorithm's inference of patterns and structures recognized by the algorithm. The agility after testing the sequentially learned data while coinciding them with the input and output is the actual goal
</br>

### keywords
scalar encoder, spatial pooler, neocortex, and temporal memory.
</br></br>



### Project: ML21/22- 1.2.Analyse Image Classification (use simple artificial images 1)
|   |   |  
|---|---|
| Issue  | [Issue 191](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/issues/191)  |  
| Team  |  Team_SmartCoders  |  
|  Author |  [Bodhisatta Ghosh](https://github.com/Bodhisatta75)
|  Author |  [Hindol Debnath](https://github.com/Hindol2016)
|  Author |  [Al Rahat Hossain](https://github.com/alrahat17)
| Source Code  |  [Code](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/tree/Team_SmartCoders/MySEProject/ImageClassification) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2021-2022/blob/Team_SmartCoders/MySEProject/ImageClassification/Documentation/DocumentationSEproject.pdf)|

#### Abstract
The purpose of this study is to change different Hierarchical Temporal Memory (HTM) learning parameters to find the best fit showing the image classification and to demonstrate how these factors affect learning. Our goal is to improve the input prediction and implement the highest similarity between the input images. We used four common shapes - circle, square, star, and triangle for this experiment.
</br>

Keywords
Hierarchical Temporal Memory (HTM), Sparse Distributed Representation (SDR), Spatial Pooler (SP), Temporal Memory (TM), Inhibition, Global Inhibition, Local Inhibition, Potential Radius, Local Area Density, Active Column, Inhibition Area, neocortex.
</br></br></br></br>








# Projects_20-21
*  [Score ✯✯✯](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#score--6)
*  [Score ✯✯](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#score--7)
*  [Score ✯](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#score--8)
*  [Discussed later](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#discussed-later)




## Score ✯✯✯



## Score ✯✯
*  [ML20/21- 5.4 Investigate stability of Homeostatic Plasticity Controller](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2021--54-investigate-stability-of-homeostatic-plasticity-controller)
*  [ML20/21- 5.4 Investigate stability of Homeostatic Plasticity Controller](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2021--54-investigate-stability-of-homeostatic-plasticity-controller-1)







### Project: ML20/21- 5.4 Investigate stability of Homeostatic Plasticity Controller
|   |   |  
|---|---|
| Issue  | [Issue 94](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/issues/94)  |  
| Team  |  Elite-group  |  
|  Author |  [Paween Pongsomboon](https://github.com/paweenp)
|  Author |  [Onyema Kizito Nnaemeka](https://github.com/onyemakn)
|  Author |  [Joseph Itopa Abubakar](https://github.com/JosephItopa)
|  Author |  [Md. Tanzeem Hasan Mahmud](https://github.com/TanzeemHasan)
| Source Code  |  [Code](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/tree/ML20/21-5.4.-Investigate-stability-of-Homeostatic-Plasticity-Controller-Elite-group/Source/MyProject) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/blob/ML20/21-5.4.-Investigate-stability-of-Homeostatic-Plasticity-Controller-Elite-group/Source/MyProject/Documents/ML20-21-5.4%20Investigate%20stability%20of%20Homeostatic%20Plasiticty%20Controller.pdf)|



#### Abstract
Homeostatic Plasticity Controller (HPC) is a developed algorithm inspired by the Homeostatic Plasticity Mechanism in neuron networks. It controls the boosting mechanism in the Hierarchical Temporal Memory (HTM) – Spatial Pooler (SP) Learning algorithm. The Spatial Pooler (SP) learning generates the Sparse Distributed Representative (SDR) of the inputs. The SDR of the inputs is expected to be unchanged in the long run. This experiment investigated the effect of a boosting factor on the minimum unchanged SDR in the SP-Learning iteration required for HPC.
</br></br>




### Project: ML20/21- 5.4 Investigate stability of Homeostatic Plasticity Controller
|   |   |  
|---|---|
| Issue  | [Issue 80](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/issues/80)  |  
| Team  |  Aspire  |  
|  Author |  [Sabin Bir Bajracharya](https://github.com/sabinbajracharya)
|  Author |  [Haritha Lakshmi Gopinathan ](https://github.com/harytha6)
| Source Code  |  [Code](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/tree/ML2021-5.4-Investigate-stability-of-Homeostatic-Plasticity-Controller-By-Team-Aspire/MyProject) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/blob/ML2021-5.4-Investigate-stability-of-Homeostatic-Plasticity-Controller-By-Team-Aspire/MyProject/Documentation/Documentation.pdf)|



#### Abstract
The HTM Spatial Pooler (operating at L2), with the extended Homeostatic Plasticity Controller (HPC), generates the Sparse Distributed Representation (SDR) for the input. But this SDR pattern is stable for a while, then changes exactly for only one input in one learning iteration, causing momentary―instability‖. Thus, this problem is hereafter referred to as the―one-cycle problem and this paper discusses what causes the one-cycle problem and how it is remedied. The causes are examined from various angles – is it just the wrong feeding of values to configuration parameters for the Spatial Pooler or HPC? Or is it a fundamental execution issue? 
</br>
#### Keywords 
Homeostatic Plasticity, Spatial Pooler, instability, boosting, SDR, stability, Scalar Encoder  
</br></br>







## Score ✯
*  [ML20/21- 5.14 Background removing algorithm for learning API ](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2021--514-background-removing-algorithm-for-learning-api)
*  [ML20/21- 5.1. Investigate Spatial Similarity](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2021--51-investigate-spatial-similarity)
*  [ML20/21- 5.9. Investigate SpatialPooler noise robustness](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2021--59-investigate-spatialpooler-noise-robustness)
*  [ML20/21- 5.12. Analyze and document boosting algorithm](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2021--512-analyze-and-document-boosting-algorithm)





### Project: ML20/21- 5.14 Background removing algorithm for learning API  
|   |   |  
|---|---|
| Issue  | [Issue 85](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/issues/85)  |  
| Team  |  ---  |  
|  Author |  [Muhammad Usman](https://github.com/usmann2023)
| Source Code  |  [Code](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/tree/usman62/MyProject/Background_Removal) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/blob/usman62/MyProject/Background_Removal/Project_Documentation/BackgroundRemoval_Report.pdf)|


#### Abstract
Background removal is the most common technique used in image processing nowadays, to remove unnecessary objects from the background of an image or video. The goal of background removal is to focus on the main object of the image. In this project, I worked on an algorithm that removes the background of 24-bit images of different formats i.e., jpg, png, tiff, gif. The algorithm works on averaging the edge RGB pixel of a 24-bit image and then compares it to the preset threshold value to extract the foreground. The performance of the designed algorithm is not very impressive for complex background images, but the algorithm shows good results for solid background images.
</br>   
#### Keywords 
Image processing, Background Removal, Threshold, Foreground.
</br></br>



### Project: ML20/21- 5.1. Investigate Spatial Similarity
|   |   |  
|---|---|
| Issue  | [Issue 84](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/issues/84)  |  
| Team  |  ---  |  
|  Author |  [Mandar Hate](https://github.com/MandarH)
|  Author |  [Bilal Shaikh](https://github.com/bryan26-xyz)
|  Author |  [Shivam Kaushik](https://github.com/ShivamKaushik007)
| Source Code  |  [Code](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/tree/Pitchers_ML-20/21-ML5.1-Investigate-Spatial-Similarity/MyProject) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/blob/Pitchers_ML-20/21-ML5.1-Investigate-Spatial-Similarity/MyProject/Documentation/ML20-21%20Investigate%20Spatial%20Similarity.pdf)|


#### Abstract
Spatial Similarity between the images is the degree to which the images are correlated or similar in nature. This paper examines the output of the Spatial Pooler, a component of the HTM, and the Spatial Similarity between different images which is affected by its parameters. The images are fed as arbitrary binary input patterns which are represented by a sparse distribution called Sparse Distribution Representation. The sparse distribution is analysed by a correlation function which measures the degree of similarity and outputs it into a matrix format. The key parameters that impact the similarity between the generated SDRs of the images are observed and their influence is noted.  
</br>
#### Keywords 
Correlation matrix, Spatial Pooler, Similarity, Binarization, Homeostatic Plasticity Controller.  
</br></br>

 




### Project: ML20/21- 5.9. Investigate SpatialPooler noise robustness  
|   |   |  
|---|---|
| Issue  | [Issue 72](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/issues/72)  |  
| Team  |  Seekers  |  
|  Author |  [Syed Ali Jaffar](https://github.com/SyedJaffar1)
|  Author |  [Usman Ali](https://github.com/Usmanali3599)
|  Author |  [Usama Shakoor](https://github.com/UsamaShakoor)
|  Author |  [Syed Mashood-ul-Hassan](https://github.com/syedkai)
| Source Code  |  [Code](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/tree/Seekers-ML20/21-5.9) | 
| Documentation  |  [Readme](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/blob/Seekers-ML20/21-5.9/MyProject/Readme.md)|


#### Abstract
This project analyzes different parameters that affect the noise robustness of the SDRs generated. The main goal is to analyze the factors that affect the performance of spatial poolers to generate similar SDRs in case different percentages of noise are added to the input.  
</br>
#### Keywords 
different parameters, noise robustness, performance of spatial pooler.  
</br></br>



### Project: ML20/21- 5.12. Analyze and document boosting algorithm  
|   |   |  
|---|---|
| Issue  | [Issue 119](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/issues/119)  |  
| Team  |  HIGHLAND  |  
|  Author |  [Isfaq Ahmad Jadoon](https://github.com/ishfaq2235)
| Source Code  |  [Code](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/tree/HIGHLAND/MyProject) | 
| Documentation  |  [Readme](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/blob/HIGHLAND/MyProject/Boosting%20Algorithm/Documentation/README.md)|


#### Abstract
“Boosting” is a term that refers to a branch of algorithms that changes weak learners to strong learners. Boosting is a group strategy for improving the model forecasts of some random learning algorithm. Boosting is to prepare weak learners consecutively, each attempting to address its predecessor. This work shows the boosting algorithm that boosts the columns in the spatial pooler (SP). The boosting algorithm tracks the column activity in spatial pooler(SP) and it makes sure that all columns are uniformly used across all seen patterns. This paper shows several experiments like Adapting synapses, Updating duty cycle, Bumping up weak columns, Update boost factors, inhibition radius, and min duty cycle of the boosting algorithm. Each experiment is evaluated based on the theoretical and practical framework and then summarized the results in graphical diagrams.
</br>
#### Keywords 
Boosting Algorithm, Synapses, Boost Factor, Duty Cycle. 
</br></br>





## Discussed later
*  [ML20/21- 5.10Investigation of Sequence Learning of SP&TM](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2021--510investigation-of-sequence-learning-of-sptm)
*  [ML20/21- 5.11-Implement a correlation diagram ](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml2021--511-implement-a-correlation-diagram)



### Project: ML20/21- 5.10Investigation of Sequence Learning of SP&TM
|   |   |  
|---|---|
| Issue  | [Issue 107](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/issues/107)  |  
| Team  |  Vikings_2021  |  
|  Author |  [Snigdha Kantamuneni](https://github.com/SnigdhaKantam)
|  Author |  [Manoj Marigowda](https://github.com/ManojMarigowda)
|  Author |  [Sudhakar Vundavalli](https://github.com/Sudhakar3377)
|  Author |  [Shivakumar Haralahalli Mariyappa](https://github.com/Shivakumar-hm)
| Source Code  |  [Code](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/tree/Vikings_2021/MyProject) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/blob/Vikings_2021/MyProject/Documentation/ML2021-5.10Investigation%20of%20Sequence%20Learning%20of%20SP%26TM_Updated.pdf)|

#### Abstract
Hierarchical Temporal Memory (HTM) is based on the supposition that the world has a structure and is therefore predictable. The development of HTM for Artificial Neural Networks has led to an advancement in the field of artificial intelligence and leading computing intelligence to a new age. In this paper, we studied various learning parameters like Width(W), Input Bits(N), Max, Min values, Cells per Column, HTM Sparsity, Activation Threshold, Permanence Increment, Permanence Decrement, Max Boost and Duty Cycle, and the number of columns, that majorly contribute to optimizing the sequence learning behavior of spatial pooler and temporal memory layer. We also performed experiments to obtain stability of Spatial Pooler output by tuning the boost and duty cycles. we have used the Spatial pooler algorithm with an extension of the homeostatic plasticity component that controls the boosting and deactivates it after entering the stable state. We evaluated each of these parameters based on the theoretical and practical framework and summarized the results in graphical diagrams.
</br>
#### Keywords 
Temporal memory, sequence learning,     Spatial pooler, stability, sparse distributed representations, Encoders.  
</br></br>




### Project: ML20/21- 5.11-Implement a correlation diagram 
|   |   |  
|---|---|
| Issue  | [Issue 107](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/issues/107)  |  
| Team  |  ---  |  
|  Author |  [Jayshri Taywade](https://github.com/Jayshri137)
|  Author |  [Chhavi Sareen](https://github.com/chhavi120)
| Source Code  |  [Code](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/tree/ML20/21-5.11-Implement-a-correlation-diagram/My%20Project/MyProject) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2020-2021/blob/ML20/21-5.11-Implement-a-correlation-diagram/My%20Project/MyProject/Documentation/ML2021-5.11-Implement%20a%20correlation%20diagram%20(2).pdf)|


#### Abstract
A correlation matrix is a table that displays the coefficients of correlation between two variables. The correlation between the two variables is shown in each table cell. A correlation matrix can be used to summarize data, as an input for a more sophisticated study, or as a diagnostic tool for advanced analyses. This project proposes an image similarity computing method, image identification, and classification from a defined set of images using a Spatial pooler for learning and classifying visual data. The research shows that we have a 
correlation matrix from where we can see the similarities of one image with any other image and with the same image. The result we got while comparing with the same image is 1. 
</br>
#### Keywords 
Correlation Matrix, Hamming Distance, Similarity, Binarization, Spatial Pooler  
</br></br>








# Projects_19-20
*  [Score ✯✯✯](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#score--9)
*  [Score ✯✯](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#score--10)
*  [Score ✯](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#score--11)



## Score ✯✯✯
*  [ML19/20- 5.6. Implement SDR Classifier](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml1920--56-implement-sdr-classifier)
*  [ML19/20- 5.10. Validate Memorizing capabilities of SpatialPooler](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml1920--510-validate-memorizing-capabilities-of-spatialpooler)
*  [ML19/20- 5.12. Investigate SpatialPooler noise robustness](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml1920--512-investigate-spatialpooler-noise-robustness)
*  [ML19/20- 5.2. Improving of implementation of the Scalar encoder in HTM](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml1920--52-improving-of-implementation-of-the-scalar-encoder-in-htm)
*  [ML19/20- 5.4. Investigation of Sequence Learning of SP/TM Layer](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml1920--54-investigation-of-sequence-learning-of-sptm-layer)
*  [ML19/20- 5.5. Implement CLA Classifier](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml1920--55-implement-cla-classifier)


### Project: ML19/20- 5.6. Implement SDR Classifier
|   |   |  
|---|---|
| Issue  | [Issue 73](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/issues/73)  |  
| Team  |  GroupA2020  |  
|  Author |  [Chetan Chadha ](https://github.com/chetan2510)
|  Author |  [Jagdeep Singh](https://github.com/jssidhu94)
|  Author |  [Maria Majid](https://github.com/Mariakhanmm92)
|  Author |  [Sidra Hussain](---)
|  Author |  [Sanjana Sharma](https://github.com/sanjana-sharma-uas)
|  Author |  [Vishakha Babulal](https://github.com/vishakhc)
| Source Code  |  [Code](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/tree/GroupA2020/Source/HTM) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/blob/GroupA2020/Source/HTM/GroupA2020DocumentationAndVideo/SDR_Classifier_Research_Paper.pdf)|


#### Abstract
The development of Hierarchical Temporal Memory (HTM) for Artificial Neural Networks has led to an advancement in the already-known Cortical Learning Algorithm (CLA) classifier. The improved classifier is called the Sparse Distributed Representation (SDR) classifier which unlike the CLA classifier uses a feed-forward neural network with maximum likelihood estimation for prediction and classification. In this paper, the SDR Classifier is implemented using Numenta’s documented and tested approach. The SDR Classifier, unlike the CLA Classifier, is established for continuous learning to reinforce correct predictions in its updating weight matrix and additionally to penalize incorrect predictions. This is executed using the Softmax algorithm and Learning in the current case. The results show the proposed classifier updates its weight matrix to reach accurate prediction probability.
</br></br>



### Project: ML19/20- 5.10. Validate Memorizing capabilities of SpatialPooler
|   |   |  
|---|---|
| Issue  | [Issue 84](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/issues/84)  |  
| Team  |  PRD1  |  
|  Author |  [Rina Yadav](https://github.com/rina-yadav08)
|  Author |  [Pradosh Kumar Panda](https://github.com/pradosh2442)
|  Author |  [Dipanjan Saha](https://github.com/dsaha1991)
| Source Code  |  [Code](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/tree/PRD1/PRD1%20Group%20SE%20Project(WS-2019)) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/blob/PRD1/PRD1%20Group%20SE%20Project(WS-2019)/NoiseTestSpatialPooler/Group_PRD1_Valdating%20Memorizing%20Capabilites%20of%20Spatial%20Pooler-Updated1.pdf)|



#### Abstract
The main objective of the project is to describe memorizing capabilities as the ability to recall the last impression of the input sequence. It utilizes Hierarchical temporal memory (HTM) to generate SDR’s. We have described how input vectors are generated for different learning sequences and shown the output for the learning sequences using an encoder. We have discussed different test cases to verify the memorizing capabilities of the Spatial Pooler using different learning sequences. To check the similarities of these sequences we have used hamming distance and overlap plotting.
</br></br>




### Project: ML19/20- 5.12. Investigate SpatialPooler noise robustness
|   |   |  
|---|---|
| Issue  | [Issue 94](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/issues/94)  |  
| Team  |  VNGroup  |  
|  Author |  [Sang Nguyen](https://github.com/SangNguyen-97)
|  Author |  [Duy Nguyen](---)
| Source Code  |  [Code](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/tree/VNGroup/Source/MyProject) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/blob/VNGroup/Source/MyProject/Documentation/SangNguyen_1185021_SE-19-20_SpatialPooler_NoiseRobustness.pdf)|


#### Abstract
The Thousand Brains Theory of Intelligence is a new and rising approach to understanding human intelligence. The theory attempts to explain the fundamental principles behind human intelligence through many discovered biological evidence and logical reasoning. This theory lays the foundation for Hierarchical Temporal Memory (HTM) - an AI framework, which has many applications in practice. In this paper’s HTM model, the building block of a basic HTM structure comprises an Encoder, a Spatial Pooler, and a Temporal Memory. This fundamental component has two prominent features: noise robustness and prediction. The Spatial Pooler is mostly responsible for the noise-handling function of the complete structure. This paper provides some experimental data and comments about the reliability of the Spatial Pooler’s noise-handling function. Specifically, the level of noise robustness is measured by the similarity between outputs of the Spatial Pooler when it takes the original data set and then the additive Gaussian noisy data sets as inputs, provided that it is only trained with the original data set.
</br></br>





### Project: ML19/20- 5.2. Improving of implementation of the Scalar encoder in HTM
|   |   |  
|---|---|
| Issue  | [Issue 91](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/issues/91)  |  
| Team  |  Group3  |  
|  Author |  [Sahana Prasad](https://github.com/PrasadSahana)
|  Author |  [Prajwal Nagaraja](https://github.com/rprajwaln)
|  Author |  [Komala Balakrishna](https://github.com/Komala-Balakrishna)
| Source Code  |  [ScalarEncoderTests.cs](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/tree/Group3/Source/HTM/UnitTestsProject/EncoderTests) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/blob/Group3/Source/HTM/UnitTestsProject/EncoderTests/Documentation/Project%20Report.pdf)|


#### Abstract
Scalar Encoder is one of the encoding techniques and is a part of Hierarchical Temporal Memory (HTM). HTM is a machine intelligence technology that is trying to imitate the process and architecture of the neocortex. The main purpose of the scalar encoder is to encode numeric or floating-point values into an array of bits, where the output has 0s with an adjacent block of 1s. The location of the block of 1’s varies continuously depending on the input value.
</br></br>






### Project: ML19/20- 5.4. Investigation of Sequence Learning of SP/TM Layer
|   |   |  
|---|---|
| Issue  | [Issue 85](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/issues/85)  |  
| Team  |  GT4  |  
|  Author |  [Ghulam Mustafa](https://github.com/gmustafa95)
|  Author |  [Muhammad Mubashir Ali Khan](https://github.com/Mubashir2994)
|  Author |  [Abdul Samad](https://github.com/abdul152)
|  Author |  [Mehdi Diab](https://github.com/diabelmehdi)
|  Author |  [Tresa Thomas](https://github.com/treesathomas)
| Source Code  |  [HTM](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/tree/GT4/MyProject/HTM) | 
| Documentation  |  [Documentation](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/tree/GT4/MyProject/HTM/Documentation/Final%20Report)|



#### Abstract
It is necessary for survival in the natural environment to be able to identify and predict the temporal sequence of sensory input. Based on numerous common properties of the cortical neurons, the theoretical framework for sequence learning in the neocortex recently proposed hierarchical temporal memory (HTM). In this paper, we analyze the sequence learning behavior of spatial pooler and temporal memory layer in dependence on HTM Sparsity. We found the ideal value of HTM Sparsity that will have optimal learning for the given input sequence. We also showed the effect of changing Width and Input Bits on learning such that the value of HTM Sparsity remains constant. We devised a relation between HTM Sparsity and max for optimal learning of the given sequence.
</br></br>





### Project: ML19/20- 5.5. Implement CLA Classifier
|   |   |  
|---|---|
| Issue  | [Issue 78](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/issues/78)  |  
| Team  |  super6  |  
|  Author |  [Anik Saha](https://github.com/saha-anik)
|  Author |  [Kazi Md Wahidul Gani](https://github.com/WahidulGani)
|  Author |  [Meem Shahrin](https://github.com/shahrin-meem)
|  Author |  [Mou Saha](https://github.com/mousaha)
|  Author |  [Riyad Ul Islam](https://github.com/sudo-riyad)
|  Author |  [Sami Patwary ](https://github.com/samipatwary)
| Source Code  |  [HTM](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/tree/super6/Source/HTM) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/blob/super6/Source/HTM/Super6DocumentationAndVideo/Implement%20CLA%20Classifier.pdf)|


#### Abstract
HTM CLA is a new method of machine learning, a cognitive approach that is scientifically influenced, based on the concepts of how the human brain functions. CLAs are an effort by Numenta Inc. to generate a computational prototype of perceptual analysis and learning inspired by the neocortex in the human brain. The approach welcomes the hierarchical structure and suggests a system for memory prediction of what will happen in the near future. This paper presents a detailed description of HTM’s Cortical Learning Algorithm (CLA). The algorithm is implemented using three classes in the dotnet Core 3.0 platform. The results are observed for different iterations and inputs in the classifier.
</br></br></br>






## Score ✯✯
*  [ML19/20- 3.31. Migrate 18.2 Implement Image Binarizer(ML 18/19-2.5)](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml1920--331-migrate-182-implement-image-binarizerml-1819-25)
*  [ML19/20- 5.1 Implementation of Geo-Spatial Encoder](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml1920--51-implementation-of-geo-spatial-encoder)
*  [ML19/20- 5.11. Schema Image Classification](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml1920--511-schema-image-classification)
*  [ML19/20- 5.7. Performance Spatial Pooler Global vs. Local Inhibition](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml1920--57-performance-spatial-pooler-global-vs-local-inhibition)
*  [ML19/20- 5.8 Serialization of Spatial Pooler](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml1920--58-serialization-of-spatial-pooler)




### Project: ML19/20- 3.31. Migrate 18.2 Implement Image Binarizer(ML 18/19-2.5)
|   |   |  
|---|---|
| Issue  | [Issue 78](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/issues/78)  |  
| Team  |  SEIV-X  |  
|  Author |  [Daniel Okoyo](https://github.com/nakwhite)
|  Author |  [Uchechukwu John Emenike](https://github.com/uchemenike)
|  Author |  [Arinze Okpagu](https://github.com/Rinzx)
| Source Code  |  [ImageBinarizer](https://github.com/UniversityOfAppliedSciencesFrankfurt/LearningApi/tree/image-binarizer/SEIV-X/ImageBinarizer) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/LearningApi/blob/image-binarizer/SEIV-X/Documentation/Image%20Binarizer.pdf)|


#### Abstract
One of the key features of binarization is converting pixel images to binary images. It
provides sharper and clearer contours of various objects present in the image. This feature extraction has proven helpful in the learning of
AI models, optical character recognition, facial recognition, document analysis, quality inspection of materials, and various image processing tasks. The use of binary images decreases the computational load for these applications. The accuracy of binarization methods
is affected by factors such as shadows, nonuniform illumination, low contrast, large signal-dependent noise, etc This paper aims to present some of the more recent approaches in the field and compare their results with some of the classic algorithms.
</br></br>



### Project: ML19/20- 5.1 Implementation of Geo-Spatial Encoder
|   |   |  
|---|---|
| Issue  | [Issue 88](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/issues/88)  |  
| Team  |  wise2019  |  
|  Author |  [Gouthaami Sukadore Ramesh](https://github.com/gouthaamisr)
|  Author |  [Lakshmi Alekya Chittem](https://github.com/Alekya09)
|  Author |  [Ravi Kumar Solanki](https://github.com/rvsolanki97)
| Source Code  |  [GeoSpatialEncoderTests.cs](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/tree/wise2019/SE%20Project/GeoSpatialEncoder/Encoders) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/blob/wise2019/SE%20Project/GeoSpatialEncoder/Encoders/Documentations%20and%20video/Geo-Spatial%20Encoder_%20Final%20Documentation3.pdf)|


#### Abstract
For implementing a geospatial encoder, this application utilizes Hierarchical Temporal Memory (HTM), a biologically inspired computational theory based on the neocortex, to automatically model typical travel patterns for larger areas and smaller areas. Travel patterns are learned by encoding latitude and longitude data plus speed into Sparse Distributed Representations (SDRs). In this, we describe how to encode data as SDRs for use in HTM systems. How an encoder can capture geospatial data. We explain the scalar encoders, and we discuss the test cases implemented in Geospatial encoders for various locations.
</br>
#### Keywords
HTM, SDRs, Scalar Encoder, Latitude, Longitude
</br></br>



### Project: ML19/20- 5.11. Schema Image Classification
|   |   |  
|---|---|
| Issue  | [Issue 86](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/issues/86)  |  
| Team  |  trozanHorse  |  
|  Author |  [Md Abu Syeem Dipu](https://github.com/Syeem007)
|  Author |  [Md Mahbub Ul Alam](https://github.com/Leon-Mahbub)
|  Author |  [Tanvir Hasan](https://github.com/tanvirBsmrstu)
|  Author |  [Mir Mehedi Hasan Rayhan](https://github.com/mirrayhan08)
|  Author |  [Md Mijanur Rahaman](https://github.com/Mijanice)
|  Author |  [Md Zahidul Islam](https://github.com/jahidkaysar)
| Source Code  |  [Schema_Image_Classification](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/tree/trozanHorse/Schema_Image_Classification) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/blob/trozanHorse/Schema_Image_Classification/Schema%20Image%20Classification.pdf)|


#### Abstract
Image classification is a classical problem of image processing; and machine learning fields and it is a complex process that may be affected by many factors. In this paper, we study image classification using deep learning, and emphasis is placed on the summarization of major advanced classification approaches and the techniques used for improving classification accuracy. In this paper, we are trying to categorize the images by their similarity of them Based on Hierarchical Temporal Memory.
</br></br>


### Project: ML19/20- 5.7. Performance Spatial Pooler Global vs. Local Inhibition
|   |   |  
|---|---|
| Issue  | [Issue 89](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/issues/89)  |  
| Team  |  GroupA1   |  
|  Author |  [Tran Quang Trung](https://github.com/QuangTrungFHFF)
|  Author |  [Nguyen Thanh Quang](https://github.com/thanhquangNg)
| Source Code  |  [GlobalLocalInhibitionResult](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/blob/GroupA1/Source/HTM/UnitTestsProject/GlobalLocalInhibitionResult/README.md) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/blob/GroupA1/Source/HTM/UnitTestsProject/GlobalLocalInhibitionResult/Documentation/Performance%20Spatial%20Pooler%20between%20Global%20and%20Local%20Inhibition.pdf)|


#### Abstract
Each region in the cortex receives input through millions of axons from sensory organs and from other cortical regions. It remains a mystery how cortical neurons learn to form specific connections from this large number of unlabeled inputs in order to support further computations. Hierarchical temporal memory (HTM) provides a theoretical framework for understanding the computational principles in the neo-cortex. HTM spatial pooler was created to model how neurons learn feed-forward connections. The spatial pooler method converts the arbitrary binary input patterns into sparse distributed representations (SDRs) using competitive Hebbian learning’s rules and homeostasis excitability control mechanisms. In this paper, one of the Spatial Pooler’s key parameters, which is the “inhibition”, will be described. The main part is to show the differences between the “local” and “global” inhibition and how and what kind of effects they contribute to the process of the Spatial Pooler learning algorithm.
</br></br>




### Project: ML19/20- 5.8 Serialization of Spatial Pooler
|   |   |  
|---|---|
| Issue  | [Issue 87](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/issues/87)  |  
| Team  |  GroupSW   |  
|  Author |  [Anik Biswas](https://github.com/aniklog)
|  Author |  [Yarlagadda Raghavendra](https://github.com/raghavfrauas)
|  Author |  [Lakshmi Mounika  Kolisetty](https://github.com/MounikaKolisetty)
|  Author |  [Manash Chakraborty](https://github.com/Manash-UAS)
| Source Code  |  [HTM](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/tree/GroupSW/Source/HTM) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/blob/GroupSW/Source/HTM/UnitTestsProject/Spatial%20Pooler%20Serialization%20Documentation%20Group%20SW/Serialization%20of%20Spatial%20Pooler%20Group%20SW.pdf)|



#### Abstract
Hierarchical temporal memory (HTM) is a machine intelligence model that is inspired by the Neocortex and provides a framework to potentially perform learning and prediction of spatiotemporal data. Spatial Pooler (SP) is an important component of HTM, that models how neurons learn from connections and make an effective representation of input by converting binary input patterns into Sparse Distributed Representations. The current implementation of the Spatial Pooler model does not support Serialization. This paper attempts to provide a best-fit Serialization Model for the Spatial Pooler Software Module in a .NET environment.
</br></br></br>





## Score ✯
*  [ML19/20- 3.13. Validate and improve Tests of existing algorithms](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml1920--313-validate-and-improve-tests-of-existing-algorithms)
*  [ML19/20- 5.2. Improving of implementation of the Category encoder in HTM](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml1920--52-improving-of-implementation-of-the-category-encoder-in-htm)
*  [ML19/20- 5.11. Image classification with Spatial Pooler](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2022-2023/blob/master/Projects/process.md#project-ml1920--511-image-classification-with-spatial-pooler)




### Project: ML19/20- 3.13. Validate and improve Tests of existing algorithms
|   |   |  
|---|---|
| Issue  | [Issue 103](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/issues/103)  |  
| Team  |  GroupK3.1   |  
|  Author |  [Hafiz Maaz Ahmed](https://github.com/maaz06)
|  Author |  [Abdul Saboor](https://github.com/saboor3333)
| Source Code  |  [LearningApi](https://github.com/UniversityOfAppliedSciencesFrankfurt/LearningApi/tree/GroupK3.1/LearningApi) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/LearningApi/blob/GroupK3.1/LearningApi/Documentation/LogisticRegression_SelfOrganizing%20Map_UnitTest_Project.pdf)|

#### Abstract
Machine learning algorithms, namely, Logistic Regression and Self-Organizing Map were used on the previously
available and new experimental datasets to validate the existing algorithms. For Logistic Regression we created
new tests such as Breast Cancer Diagnosis and Social Network Ads leading to Purchase, to model a logistic
regression function (system) using the existing algorithm to produce positive test cases. For Self-Organizing maps
new datasets of more than two dimensions were employed. The experiment was done by including new UnitTests
using the MSTest testing platform of Microsoft Dot Net Core Framework. From the successful implementation of tests,
we verified the efficiency of existing Logistic regression and Self-Organizing Map algorithms. Keywords—Logistic Regression, Self-Organizing Map, Machine Learning, Unit Test, MSTest Framework
</br></br>





### Project: ML19/20- 5.2. Improving of implementation of the Category encoder in HTM
|   |   |  
|---|---|
| Issue  | [Issue 90](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/issues/90)  |  
| Team  |  Netriderss   |  
|  Author |  [Muhammad Basaier](https://github.com/muhammadbasaier)
|  Author |  [Syed Faizan Khursheed](https://github.com/faizan123760)
|  Author |  [Syed  Muhammad Rah](https://github.com/syedrahim1996)
| Source Code  |  [CategoryEncoderTests.cs](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/blob/Netriderss/Source/HTM/UnitTestsProject/EncoderTests/CategoryEncoderTests.cs) | 
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/blob/Netriderss/Project%20Report/Category_Encoder_Project_Report.pdf)|


#### Abstract
HTM (Hierarchical Temporal Memory) can be defined as a memory of sequences. This theory hypothesizes that every excitatory neuron in the neocortex is learning transitions of patterns and that the majority of synapses on every neuron are dedicated to learning these transitions. Temporal Memory is therefore the substrate upon which all neocortical functions are built. HTM starts with the assumption that everything the neocortex does is based on memory and recall of sequences of patterns. There are two major techniques of HTM which are
category and scalar encoders. Based on the technique we have implemented a category encoder which is the fundamental block of HTM. Category Encoder encodes the string into a Sparse Distributed Representations (SDR) on the basis of bits we have to distinguish elements in the list. An array of output binary bits can be used in the HTM system.
</br></br>




### Project: ML19/20- 5.11. Image classification with Spatial Pooler
|   |   |  
|---|---|
| Issue  | [Issue 92](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/issues/92)  |  
| Team  |  ---   |  
|  Author |  [Mandeep Singh](https://github.com/mandeepsinghsherry)
| Source Code  |  [Code](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/tree/Mandeep_Singh) |
| Documentation  |  [PDF](https://github.com/UniversityOfAppliedSciencesFrankfurt/se-cloud-2019-2020/blob/Mandeep_Singh/Source/HTM/Documentation/Documentation.pdf)|



#### Abstract
This paper presents an emerging machine learning algorithm Hierarchical Temporal Memory (HTM) which uses using Spatial pooler for learning and classifying visual data. The SP models how neurons learn feedforward connections and form efficient representations of the input. It converts arbitrary binary input patterns into sparse distributed representations (SDRs), using a combination of competitive Hebbian learning rules and homeostatic excitability control, and we also describe a key parameter of the SP.
</br></br>





Spatial Pooler (SP) is a learning algorithm that is designed to replicate the neuron functionality of the human brain. Essentially, if a brain sees one thing multiple times, it is going to strengthen the synapses that react to the specific input resulting in the recognition of the object. Similarly, if several similar SDRs are presented to the SP algorithm, it will reinforce the columns that are active according to the on bits in the SDRs. If the number of training iterations is big enough, the SP will be able to identify the objects by producing different sets of active columns within the specified size of SDR for different objects.

### Link to Project Code  [Link](https://github.com/alihaider4189/neocortexapi/blob/UnitCodeMaster/source/UnitTestsProject/SpatialPoolerTestsNEWByAliRazaKharl.cs) <br>
