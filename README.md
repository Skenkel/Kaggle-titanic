# Kaggle-titanic
My solutions for Kaggle's  titanic competition

Skenkel-Titanic-EDA is some exploratory data analysis of who lived and who died in the training set. It defines many of the other notebooks. In short, Women and Children survived, and every indicator of social status (ticket price, title, etc) all indicate survivability. 

Pipelines-mvp is a minimum viable product of using the scikit-learn pipelines feature. The important thing to  remember when using pipelines is that each step of each pipeline is instantiated on the train test split seperately. This is very risky when dummying categorical data, as it is extremely likely than one category value will not be present in either the training or test data. If that occurs, the pipeline will break. The way to avoid this issue is ensure the pandas column is a 'category' with all values assigned to it. 

Stacking Shows how to stack several different models ( I use a SVM, Decission Tree Clasifier, Logistic Regression and K-neighbors classifier) to merge their predictions. 

Titanic-Tensorflow shows how to use a tflearn classifier. 

