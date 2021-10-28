# Text_Classification_SVM
Text Classification using Support Vector Machine


We will be using the Amazon Review Data to our project.

## Importing libraries
 ![image](https://user-images.githubusercontent.com/72303641/139268049-fba6204d-42ae-4d4f-aeb8-9e9d03337788.png)

## Reading the Data
 ![image](https://user-images.githubusercontent.com/72303641/139268095-36097ce9-5cda-4aee-920d-7aaf5ea39ef0.png)

Redating the data can be done by pd.read_csv() method, and we are going to be using latin-1 encoder

## Data Pre-processing
### Tokenization
Tokenization is the processing of breaking the sentences paragraphs in the smaller words, symbols or even sentences these are called tokens. NLTK has many useful libraries to do it
Such as word_tokenize() or sent_tokenize().

### Word Stemming/lemmatization
This is process of converting the words into its base forms or root form. Lemmatization is similar to stemming but stemming convert the words into the base form irrespective of the context. But stemming is easily and less computationally expensive.

After that this sequence of the procedure are undertaken:
1.	Removing the blank rows in the data
2.	Change all the text to lower cases
3.	Word tokenization
4.	Removing the stop words
5.	Removing Non alpha text
6.	Word Lemmatization

## Test train split and Encoding the words into number
 ![image](https://user-images.githubusercontent.com/72303641/139268213-179e20a2-848f-4cdd-b206-fb40128879a4.png)

## Words Vectorization
 ![image](https://user-images.githubusercontent.com/72303641/139268266-dbd10bf9-5af2-4186-8668-fdc388f1e02b.png)

This is process of converting the words into the one dimensional vectors in a way that the model can understand it is done by Term Frequency-inverse document by the method called TfidfVectorizer() 
Term Frequency: This summarizes how often a given word appears within a document.
Inverse Document Frequency: This down scales words that appear a lot across documents.

### Training the data with the ML model
We are going to train out models with Support Vector Machine. 

![Screenshot (175)](https://user-images.githubusercontent.com/72303641/139268987-742d1e2c-3c9e-4732-bf94-e97c743fa9e8.png)


 ### Prediction and Accuracy are shows above.

