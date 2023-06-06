# Email/SMS Spam or Not Spam Classifier 📧📵
## Email/SMS Spam or Not Spam Classifier
This project aims to classify whether an email or SMS is spam or not spam using machine learning techniques. The dataset used for this project is the Kaggle SMS Spam Collection Dataset, which contains a collection of SMS messages labeled as spam or not spam.

## Dataset 📊

The dataset used for this project has the following dimensions: (5572, 5). It consists of SMS messages along with their corresponding labels. The preprocessing steps performed on the dataset are as follows:

Lowercasing: All text in the SMS messages is converted to lowercase to ensure consistency.

Tokenization: The SMS messages are split into individual words or tokens, which helps in further analysis.

Removing Special Characters: Special characters, such as punctuation marks and symbols, are removed from the text as they do not contribute to the classification process.

Removing Stop Words and Punctuation: Common words like "a," "the," and punctuation marks that do not carry much meaning are removed from the text to focus on more important words.

Stemming: Words are reduced to their base or root form, such as converting "running" to "run," to reduce the dimensionality of the dataset and improve classification performance.

## Vectorization Techniques 🎛️

Two vectorization techniques were used for this project:

Bag of Words: This technique represents the SMS messages as a collection or bag of words, where each word is assigned a unique index. The presence or absence of these words is used as features for training the classifier.

TF/IDF (Term Frequency-Inverse Document Frequency): This technique evaluates the importance of each word in a document by considering its frequency in the document and the inverse frequency across all documents. It helps in giving higher weightage to words that are more relevant to the classification task.

## Classification Model 🤖
For this project, the Multinomial Naive Bayes classifier from the scikit-learn library was used. The classifier achieved an accuracy of 0.9709864603481625 on the test data. The confusion matrix for the classification results is as follows:

lua
Copy code
[[896   0]
 [ 30 108]]
The classifier correctly classified 896 non-spam messages and 108 spam messages, with no false negatives (non-spam messages classified as spam). The overall precision of the classifier is 1.0.

## Visualization 📊🌟
To gain a better understanding of the text data, a word cloud was generated. A word cloud is a visual representation of word frequency, where the size of each word represents its frequency in the text. This visualization technique can provide insights into the most frequent words in spam and non-spam messages.

## Web Application 🌐
The project includes a web application built using Streamlit, a Python library for building interactive web applications. The web application provides a user interface to input new email or SMS messages and get a prediction on whether they are spam or not spam based on the trained classifier.

## Installation and Usage

If there is no requirements.txt file in your project, you can mention the required dependencies in your README file along with the installation instructions. Here's an updated section for installation and usage:

## Installation and Usage ⚙️🖥️

To run the project locally, follow these steps:

* Clone the repository from GitHub.
* Install the required dependencies using the following commands:
![image](https://github.com/YaqoobD/Email-SMS-Spam-Classifier-End-to-End-Project-Heroku-Deployment/assets/52135942/dfbca8e4-cfd2-4c7e-9781-b5b55d39118f)

* Run the Streamlit application using the command streamlit run app.py.
* Access the web application in your browser at the provided local URL.
You can then interact with the web application by entering new email or SMS messages and getting the classification results.

Make sure you have Python and pip installed on your system before running the installation commands.

Feel free to modify the dependencies based on your specific requirements and package versions.

## Future Improvements 🔮
Here are some potential areas for future improvements:

Experiment with other machine learning algorithms, such as Support Vector Machines or Random Forests, to compare their performance with the Naive Bayes classifier.

Explore additional preprocessing techniques, such as lemmatization

## App Demo 🖥️
![image](https://github.com/YaqoobD/Email-SMS-Spam-Classifier-End-to-End-Project-Heroku-Deployment/assets/52135942/e92b2f4a-c78c-405b-8176-3ff3db87b460)

![image](https://github.com/YaqoobD/Email-SMS-Spam-Classifier-End-to-End-Project-Heroku-Deployment/assets/52135942/4e12eed4-935b-48bf-93e1-6dff8f926eb7)

![image](https://github.com/YaqoobD/Email-SMS-Spam-Classifier-End-to-End-Project-Heroku-Deployment/assets/52135942/b9ad09cd-650b-48d1-824e-c735fde7168d)
