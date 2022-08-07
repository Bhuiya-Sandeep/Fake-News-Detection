# Fake News Detection

In this modern world, data is very important and by the 2020 year, 1.7 megaBytes data generated per second. So there are many technologies that change the world by this large amount of data. Machine learning is one of them and we are using this technology to detect fake news.

## What is fake news?
Fake news's simple meaning is to incorporate information that leads people to the wrong path. Nowadays fake news spreading like water and people share this information without verifying it. This is often done to further or impose certain ideas and is often achieved with political agendas.

For media outlets, the ability to attract viewers to their websites is necessary to generate online advertising revenue. So it is necessary to detect fake news.

## WorkFlow
![This is an image](https://miro.medium.com/max/1250/0*9RuEY4YE1eEDHkE8.png)
The above diagram shows how this pipeline generated numerical features and feed it into a machine learning algorithm. In this project, we are using some machine learning and Natural language processing libraries like NLTK, re (Regular Expression), Scikit Learn.

## Natural Language Processing

Machine learning data only works with numerical features so we have to convert text data into numerical columns. So we have to preprocess the text and that is called natural language processing.

In-text preprocess we are cleaning our text by steaming, lemmatization, remove stopwords, remove special symbols and numbers, etc. After cleaning the data we have to feed this text data into a vectorizer which will convert this text data into numerical features.

## Cleaning Data

We can’t use text data directly because it has some unusable words and special symbols and many more things. If we used it directly without cleaning then it is very hard for the ML algorithm to detect patterns in that text and sometimes it will also generate an error. So that we have to always first clean text data. In this project, we are making one function ‘cleaning_data’ which cleans the data.
Lemmatization: Convert the word or token in its Base form.

Examples :

Stay, Stays, Staying, Stayed — -> Stay

House, Houses, Housing — -> House

Stop words: words that occur too frequently and not considered informative

Examples :

{‘the’, ‘a’, ‘an’, ‘and’, ‘but’, ‘for’, ‘on’, ‘in’, ‘at’ …}
## Split the Data

Splitting the data is the most essential step in machine learning. We train our model on the trainset and test our data on the testing set. We split our data in train and test using the train_test_split function from Scikit learn.

## Tfidf Vectorizer

Tfidf-Vectorizer : (Term Frequency * Inverse Document Frequency)

1.Term Frequency: The number of times a word appears in a document divided by the total number of words in the document. Every document has its own term frequency.
![This is an image](https://miro.medium.com/max/686/0*Ug3-CrBXudr0onQf.png)


2. Inverse Document Frequency: The log of the number of documents divided by the number of documents that contain the word w. Inverse data frequency determines the weight of rare words across all documents in the corpus.
![This is an image](https://miro.medium.com/max/780/0*gt6nkmwULeyeeKp5.png)


Finally Tfidf vectorizer
![This is an image](https://miro.medium.com/max/1010/0*pTu7ioPaPWkrl6L1.png)

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Fake News Detection.

```bash
pip install Fake News Detection
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
