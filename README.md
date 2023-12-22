# Multi-class-gender-emotion-classfication

In my project, I encountered the challenge of working with two distinct datasets: one classified images by gender (male/female), and the other by emotion (happy/sad). To effectively train a model capable of predicting all four required classes - HappyMale, HappyFemale, SadMale, SadFemale - I devised a unique strategy.

Initially, I developed two separate models. The first model was trained exclusively on the gender dataset, while the second focused on the emotion dataset. The key to integrating these datasets lay in cross-utilizing the models for predictions. I used the emotion model to predict the emotional states (happy or sad) of the images in the gender dataset. Conversely, I applied the gender model to the emotion dataset to determine the gender (male or female) of each image.

By combining these newly predicted labels with the existing labels, I was able to construct a comprehensive dataset encompassing all four desired categories. This amalgamated dataset, containing the refined classifications, served as the foundation for training a final, more robust model that could accurately predict the categories of HappyMale, HappyFemale, SadMale, and SadFemale. This approach not only enhanced the accuracy of the predictions but also streamlined the process of handling disparate datasets in a unified manner.

![288146417-9ecf5b71-47d4-4ccc-95e4-7a84259aa227](https://github.com/NeuraNoir/Gender-emotion-classfication/assets/113393377/e75de888-c597-4476-86b9-a827ab0f6f84)

