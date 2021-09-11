# Image_Search_Engine
The main goal of this project is to create an algorithm able to match the images in a query set with the images in a much larger set called gallery. 
Google Colab is helpful to run all the notebooks as it provides free GPU.

# Applied Machine Learning Challenge - University of Trento (2020/2021)
This is a team project: each member focussed on a particular model to achieve the given task, while collaborating with the other members to fix issues.
Further information reguarding the division of tasks, the models and the project in general can be find in the report.


# Objectives: 
The main objective of this project is to create an algorithm able to match the images in a query set with the images in a much larger set called gallery.
The problem can be viewed as an extension of the identity verification task to places/buildings and can be thought of as a kind of image search engine. 
The output should report the top-k matches. 
It is important to define how a match can be defined. Among all the possibilities, one of the most used method is the definition of a similarity/distance metric on top of extracted image features. 
Please, note that the algorithm is not trained on the gallery data, otherwise this would be a simple classification.

The secondary objective of the project is to practice in the acquisition of the data, as collecting a large amount of data is crucial for ML applications. 
Only an initial small amount of data was provided:
The training set is composed of 697 images belonging to 21 different buildings/places and 1 distractor class. 
The validation set is divided into a gallery of 534 images among 15 classes and a query of 70 images (5 for each of the 14 classes). 
Finally, during the challenge day the test set will be realased to measure the performance of the algorithm.

# How to add data: 
let’s say you want to add a new class for the Duomo di Milano in the training set. First, collect multiple instances of the Duomo di Milano. 
Second, place your instances in the same folder and name it with an ID not already used in the set you want to expand. Finally, move your new folder inside the training set folder. Note that in case you want to add a class to the query set, you have also to add it to the gallery set in order to be able to retrieve it.

# Initial data 
In the ”dataset” folder you will find 2 sub-folders, one for each split. 
In the training folder, you will find a small amount of data that you are required to expand by adding data you will mine from external sources. 
In the validation folder you will find a gallery and a query. 

# How to measure the performances: 
To measure the performance of your algorithm we will use the top-1, top-3 and top-10 accuracy metric. The top-k accuracy metric allows to measure how often the correct match/label falls in the top-k matches/predictions a
