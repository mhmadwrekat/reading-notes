# Machine Learning Intro


There’s a big challenge in data science called “Tactical Hell.” This is actually a term from startups, and it’s when you have too many tactics to choose from :

Should you develop your product more? Invest in marketing? Hire an accountant? Etc.

In many ways, training a ML model is like growing a startup. You also have too many tactics to choose from :

Should you clean your data more? Engineer features? Test new algorithms? Etc.

There’s a lot of trial and error, so how do you avoid chasing dead ends? The answer is “Exploratory Analysis.” (Which is just fancy-talk for “getting to know” your data.)

Doing this upfront helps you save time and avoid wild goose chases… As a data scientist, you are a commander with limited resources (i.e. time). Exploratory analysis is like sending scouts to learn where to deploy your forces!

---
***Model*** a set of patterns learned from data .

***Algorithm*** a specific ML process used to train a model .

***Training data*** the dataset from which the algorithm learns the model . 

***Test data*** a new dataset for reliably evaluating model performance .

***Features*** Variables (columns) in the dataset used to train the model .

***Target variable*** A specific variable you're trying to predict .

***Observations*** Data points (rows) in the dataset .


![Machine Learning](https://www.iberdrola.com/wcorp/gc/prod/en_US/comunicacion/machine_learning_mult_1_res/machine_learning_746x419.jpg)


---
***Supervised Learning***

1. In practice, it's often used as an advanced form of predictive modeling .
2. Each observation must be labeled with a "correct answer."
3. Only then can you build a predictive model because you must tell the algorithm what's "correct" while training it (hence, "supervising" it) .
4. Regression is the task for modeling continuous target variables .
5. Classification is the task for modeling categorical (a.k.a. "class") target variables .

---
Unsupervised Learning :

1. In practice, it's often used either as a form of automated data analysis or automated signal extraction .
2. Unlabeled data has no predetermined "correct answer."
3. You'll allow the algorithm to directly learn patterns from the data (without "supervision") .
4. Clustering is the most common unsupervised learning task, and it's for finding groups within your data .

---
***Key takeaway : The most effective algorithms typically offer a combination of regularization, automatic feature selection, ability to express nonlinear relationships, and/or ensembling. Those algorithms include***

- Lasso regression .
- Ridge regression .
- Elastic-Net .
- Random forest .
- Boosted tree .


> What is Feature Engineering ? Feature engineering is about creating new input features from your existing ones.


> Infuse Domain Knowledge You can often engineer informative features by tapping into your expertise about the domain.


***The 2 most commonly recommended ways of dealing with missing data actually suck***

1. Dropping observations that have missing values .
2. Imputing the missing values based on other observations

***Missing categorical data***

*The best way to handle missing data for categorical features is to simply label them as ’Missing’!*

1. You’re essentially adding a new class for the feature .
2. This tells the algorithm that the value was missing .
3. This also gets around the technical requirement for no missing values .

***Missing numeric data***

*For missing numeric data, you should flag and fill the values .*

1. Flag the observation with an indicator variable of missingness .
2. Then, fill the original missing value with 0 just to meet the technical requirement of no missing values .


![Machine Learning](https://www.simplilearn.com/ice9/free_resources_article_thumb/Deep-Learning-vs-Machine-Learning.jpg)


---
#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>