# CS 167 Project 1: 
## Learning Objectives: 
For this project, you will use the scikit-learn library to conduct machine learning experiments, and your write-up will ask you to explain what you did and interpret the results. This directly addresses two of the course learning objectives stated in the syllabus:
- Students will be able to create software which utilizes machine learning programming libraries in order to conduct machine-learning-based data analysis.
- Students will be able to develop and conduct machine-learning-based data analysis experiments, and they will be able to interpret and explain the results.

## Project Description:🚗
For this project, you will be working with a dataset consisting of over twenty features of cars manufactured in 1985 [source](https://archive.ics.uci.edu/ml/datasets/automobile). You'll be using the data to tune and develop two different models:
1. **Regression** predict the price.
2. **Classification** predict the car body type (e.g. convertible, hardtop, hatchback, sedan, wagon)

## Contest:
I have provided the data for you to use, but I have withheld a "competition testing set" consisting of random examples which will be used in a class-wide competition to see who has developed the best model. In class on Tuesday, November 1st (the Project #1 deadline), we will hold a brief competition to determine whose model will best predict the target variables in using the "competition testing set". In your project, you will create your own training and testing sets from the data, identify the best performing models and parameters, and submit your predictions to be run for the competition. The students achieving the best results (r^2 for regression and accuracy for classification) will win a prize! The code used to create the model will be handed in via a special question on the project submission via blackboard.

I have provided a skeleton of what I want your project to look like, but the rest of the experiment is up to you. **This project should read more like a lab report than a coding assignment.** I want to be able to see what you are thinking and how you are going about solving the problems and the tools that you have learned in this class so far. There are some basic guidelines as to what I want to see laid out below, but you are the machine learning engineer and it is your job to draw some meaningful conclusions about the data. 

## Project Expectations: ☑️
You will create a Colab notebook that includes your code and results to document your experiment. Most importantly, you will use text cells in the notebook to explain what you did, interpret the results, and make your recommendations. The written markdown portions must include the following things:
1. **Name**: Include your name at the top of the notebook. 
2. **Data Preparation**: Explain your data preparation. What did you have to do to get your data in shape for your experiments - creation of dummy variables, filling in missing values, etc.


**Part 1: Regression**

3. **Metrics**: Identify which metrics you will be using to test your model, and say why they are appropriate. Identify a baseline for your metrics - what would you expect to happen with this particular data if you always guessed the average or if you guessed randomly?
4. **Initial Models**: Develop basic code for kNN, weighted kNN, and Decision Trees. Make some experiments here, including graphs to help you identify which algorithm and parameters may be best. 
5. **Fine Tuning**: Create graphs to help you identify the optimal values of parameters you wish to use. Utilize different train/test splits. Full credit for thorough testing and documentation.
6. **Analysis**: What did you determine? What did you notice? How did you identify which learning algorithms you will try and which important parameters you will tune for each one? What is your predictions for the 'competition testing set'.


**Part 2: Classification**

7. **Metrics**: Identify which metrics you will be using to test your model, and say why they are appropriate. Identify a baseline for your metrics - what would you expect to happen with this particular data if you always guessed the average or if you guessed randomly?
8. **Initial Models**: Develop basic code for kNN and Decision Trees. Make some small experiments here. What do you notice? How did you identify which learning algorithms you will try and which important parameters you will tune for each one? 
9. **Fine Tuning**: Create graphs to help you identify the optimal values of parameters you wish to use. Utilize different train/test splits. Full credit for thorough testing.
10. **Analysis**: What did you determine? What is your predictions for the 'competition testing set'.

**Part 3: Conclusions**

11. **Bumps in the Road**: What challenges did you encounter? How did you overcome these challenges? Did you have to adapt your strategy to account for these challenges? Why or why not?
12. **Conclusions:** What insights/recommendations do you have? What did you find that was interesting? Which model was your best model, which models didn't work well? Why do you think this is? In general, I want a discussion of your experiment, the results, and what they mean.

### Your Experiments should Include:
- A **k Nearest Neighbors** model with a graph of at least 1 tuned parameter
- A **weighted k Nearest Neighbors** model with a graph of at least 1 tuned parameter
- A **Decision Tree** model with a graph of at least 1 tuned parameter
- **Normalized data** (for k Nearest Neighbors and weighted k Nearest Neighbors) 
- A **confusion matrix** (for final Classification model)

## Notes, Tips and Tricks

### What does it mean to tune parameters?
Tuning parameters means that you try your model with different values for that parameter and record how well the resulting model performs on the test set 📈. This is what you did in Notebook 3 when you tried different k, graphed them and found the value of k that resulted in the best model. You found the best k for k-NN, so that means you tuned k. For this project, you are strongly encouraged to try tuning more than one parameter for each model. You should make sure to pick a parameter that actually has an important effect on your model/data, and explain why you chose the parameters you chose in your text description.

### Where should I start?
Start with the example .ipynb file. Look at the different datasets and decide on the one you will focus on. Next, begin answering the questions that you can answer before you even start coding.

Use the template for building and testing a scikit-learn model. Start by doing the following:
- Change that example code to work with your new data
- Look for the appropriate documentation for the scikit-learn modules for the machine learning algorithms we have discussed in class: http://scikit-learn.org/stable/modules/classes.html .
- Try to produce several plots like the one you did in Notebook 3.

# Rubric and Grading
| **Description/Writing**  |**Points Awarded** (1 point each)  |**Notes** |
| ------------------------------- | ------------------- | --------- |
| 1: Name                         |        |    |
| 2: Data Prep                    |        |    | 
| 3: **Regression** Metrics       |        |    |
| 4: Initial Models               |        |    | 
| 5: Fine Tuning                  |        |    |
| 6: Analysis                     |        |    |
| 7: **Classification** Metrics   |        |    |
| 8: Initial Models               |        |    | 
| 9: Fine Tuning                  |        |    |
| 10: Analysis                     |        |    |
| 11: Bumps in the Road            |        |    | 
| 12: Conclusions                  |        |    |
| <b>Total                        |       /12 | </b>   |


| **Code**  | **Points Awarded**  (1 point each) | **Notes** |
| --------- | ------------------- | --------- |
| normalization of data           |        |    |
| **Regression** knn + graph             |        |    |
| **Regression** weighted knn + graph                   |        |    |
| **Regression** decision tree + graph                  |        |    |
| **Classification** knn  + graph        |        |    |
| **Classification** weighted knn  + graph                  |        |    |
| **Classification** decision tree + graph                  |        |    |
| confusion matrix                |        |    | 
| <b>Total      |       /8 | </b>   |

| **Written Portion**  | **Code Portion**   | **Total** |**Notes** |
| --------- | ------------------- | --------- |--------- |
|         /12  |                 /8    |        /20   |           |

