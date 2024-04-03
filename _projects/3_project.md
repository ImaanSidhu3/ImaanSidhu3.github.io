---
layout: page
title: Data Science & Deep Learning Final Project
description: My final project for Data Analysis for Engineers
img: assets/img/DS_8.jpg
importance: 3
category: Academic
---

New York City experienced almost 100,000 vehicular accidents in 2021 with approximately 60,000 accidents leading to injury and 245 fatal accidents. The focus of this project was to develop a model through which emergency services can be notified about which vehicle crashes require additional attention. 

The data was collected from New York City Police Department's online database for traffic accidents. For our analysis, we  focused on identifying three critical data elements within the dataset: the location of the accident (which was presented as latitude and longitude), the cause of the accident, and the type of vehicle involved in the accident. The data was limited to streets within Manhattan as accidents on highways and bridges introduced complicating factors. 

4 methods were utilized in the project: Linear and Logistic Regression, Decision Trees, Naives Bayes Classification, and a Neural Network


Linear and logistic regression was the first method used to predict the number of persons injured in an automotive accident. Encoded categorical data was not found to significantly improve the linear or logistic regressions. Because of the small range of persons injured,  regression had a limited ability to predict the outcome.
<div class="row justify-content-sm-center">
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/DS_1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/DS_7.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Regression
</div>
The results of both the linear and logistic regressions were found to be insignificant. The predicted value for the number of persons injured appears to be heavily biased due to the majority of actual number of persons injured being 0.



Next, sklearn was implemented to build a decision tree library.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/DS_9.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Predicted vs Actual Injuries through Decision Tree
</div>
This approach proved to be far more successful. Through this approach ~70% classification accuracy was achieved. The prominent thing to note is that the data set was heavily biased towards 0 or 1 injuries in an accident which in turn made the model misclassify most other bins


The third approach used was the Naive Bayes Classification, using the sklearn Naive Bayes library. This method is very similar to the decision tree structure but has the ability to probabilistically weigh output bins. We utilized a Gaussian, Multinomial, and Complement Naive Bayes. Through this technique, there was a slight improvement in classification accuracy, though statistically insignificant. The alpha value was 1.0 and we used a training split of 80/20. 
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/DS_2.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/DS_5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/DS_8.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Naive Bayes
</div>


Finally, Neural Networks were used. As in the previous methodologies, the categorical data was encoded to allow for usage in the neural network. A neural network with 3 hidden layers using the activation function ReLu and the loss function MSE was implemented.

<div class="caption">
    Neural Network
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/DS_3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Neural Network Table.
</div>

The neural network performed adequately. The accuracy of the model typically peaked within the range of 65-66%, with the best ever performance achieving nearly 70% with ReLu as the activation function and having run for 300 epochs. However, this performance was not replicable with different splits of the data. Several different activation functions and loss functions were tried, with little significant change in the results of the model. The performance of these models does not improve with epochs over 100 or a change of activation function to sigmoid or tanh. Regardless of activation function, the neural network always appeared to filter out outliers, and failed to predict more than 2 injuries on any occasion. This hinders the usefulness of the model, as in the stated application the detection of outliers is of great significance.



The best performing models were the Multinomial Bayesian Classifier and the Decision Tree. 

Throughout the course of the project, we faced some challenges and accepted some limitations within its scope. Firstly, the dataset obtained from the City of New York consisted of many inaccuracies, incomplete information or variability in inputs. This is due to the fact that it is retrieved directly from police reports, which does not have a consistent format. Furthermore, the categorical nature of the data made it difficult to introduce regression to our model. This was noted as a challenge within the scope of linear and logistic regression, as well as within the neural network analysis. Within the data, there was a lack of relational parameters between the variables and it was difficult to assess or establish any link between different independent variables. Finally, after the initial data filtering exercise, we noted that there is a strong bias within the data towards 1 and 0 in the injury reporting. This meant that when comparing predicted against actual data, any value of persons other than 1 or 0 is treated as an outlier.


Based on our findings, we were able to identify potential future extensions for the project.

* Additional independent variables can be added to the model to account for time and situational            factors that may affect the severity of vehicle accidents. These variables include the date, ambient      weather conditions and road closures. 
    
* The model can be expanded to include the prediction of accident-related deaths in addition to injuries.

* An interface system can be developed for dispatch operators to provide emergency responders with injury estimates. This will ensure that first responders will have the clearest possible picture in the case of an emergency scenario.

* The model can be tested for a larger dataset, including data from previous years and other cities.

