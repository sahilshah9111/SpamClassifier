# SpamClassifier
### Setup Instructions:
1. First, I have created a separate python virtual environment for this assignment.
2. Next, after activating the virtual environment, I have installed necessary packages needed for this project.
3. Using pip.freeze, I created requirements.txt which contains installed package list in virtual environment with its versions.
4. Now, open jupyter notebook and choose apprpriate venv in which you want to work.

### Execution Instructions:
1. Split the datasets into a training set and a test set.
2. Write a data preparation pipeline to convert each email into a feature vector. The preparation pipeline should transform an email into a (sparse) vector that indicates the presence or absence of each possible word. For example, if all emails only ever contain four words, “Hello,” “how,” “are,” “you,” then the email “Hello you Hello Hello you” would be converted into a vector [1, 0, 0, 1] (meaning [“Hello” is present, “how” is absent, “are” is absent, “you” is present]), or [3, 0, 0, 2] if you prefer to count the number of occurrences of each word.
3. Add hyperparameters to the pipeline to control whether or not to strip off email headers, convert each email to lowercase, remove punctuation, replace all URLs with “URL,” replace all numbers with “NUMBER,” or even perform stemming (i.e., trim off word endings; there are Python libraries available to do this).
4. Finally, try out several classifiers and build a great spam classifier, with both high recall and high precision.
