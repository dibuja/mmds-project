# Detecting changes in Cropland
Due to Climate Change, crop yield scarcity and decreased crops are threatening crop yields all around the world. According to some studies, the probability of crop yield failures is projected to increase 4.5 times by 2030 and up to 25 times by 2050 [1]. The crop yields are expected to significantly decrease in the future years, with expected losses of 9–28% for maize, 7-22% for wheat, 4-12% for soy or 3-11% for rice [2]. 

Is it possible to detect changes in cropland using satellite images? We have tried to answer this question so by using satellite images of croplands and trying to implement

- unsupervised clustering methods; and 
- supervised classification 

in order to detect changes in croplands that could help in providing insights related to crop yields.

### Tools
The big data tools used were mainly Apache Spark and its MLLib library for the loading of data and training of the algorithm through distributed training. It is suitable for scaling the project since Apache Spark distributes the processing and storage of data in different units so it parallelizes the processing and allows to use several machines with a theoretically unlimited amount of CPU, GPU processing capacity and RAM.

When it comes to the code, the project has been divided into three different Google Colab notebooks.

- The notebook «Spark PCA + K-means» contains the code developed to apply PCA and K-means clustering to a pair of images from the dataset by using Apache Spark.  
- The notebook «PCA + K-means» implements both PCA and K-means clustering but not using big data tools.  
- The notebook «Classification» implements the supervised classification algorithm to detect cropland changes.  
