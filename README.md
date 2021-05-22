# Simple-Chatbot
using deeplearning keras and python GUI TKINTER

let us see the file structure and the type of files we will be creating:


    Intents.json – The data file which has predefined patterns and responses.
    trainchatbot.py – In this Python file, we wrote a script to build the model and train our chatbot.
    Words.pkl – This is a pickle file in which we store the words Python object that contains a list of our vocabulary.
    Classes.pkl – The classes pickle file contains the list of categories.
    Chatbot_model.h5 – This is the trained model that contains information about the model and has weights of the neurons.
    ChatBOT.py – This is the Python script in which we implemented GUI for our chatbot. Users can easily interact with the bot.
    
Here are the 5 steps to create a chatbot in Python from scratch:

    Import and load the data file
    Preprocess data
    Create training and testing data
    Build the model
    Predict the response
    
1. Import and load the data file:
                          First, make a file name as train_chatbot.py. We import the necessary packages for our chatbot and initialize the variables we will use in our Python project. The data file is in JSON format so we used the json package to parse the JSON file into Python.
2. Preprocess data:
                  When working with text data, we need to perform various preprocessing on the data before we make a machine learning or a deep learning model. Based on the requirements we need to apply various operations to preprocess the data. Tokenizing is the most basic and first thing you can do on text data. Tokenizing is the process of breaking the whole text into small parts like words. Here we iterate through the patterns and tokenize the sentence using nltk.word_tokenize() function and append each word in the words list. We also create a list of classes for our tags. Now we will lemmatize each word and remove duplicate words from the list. Lemmatizing is the process of converting a word into its lemma form and then creating a pickle file to store the Python objects which we will use while predicting.
3. Create training and testing data
                  Now, we will create the training data in which we will provide the input and the output. Our input will be the pattern and output will be the class our input pattern belongs to. But the computer doesn’t understand text so we will convert text into numbers.
 4. Build the model
                  We have our training data ready, now we will build a deep neural network that has 3 layers. We use the Keras sequential API for this. After training the model for 200 epochs, we achieved 100% accuracy on our model. Let us save the model as ‘chatbot_model.h5’.
 5. Predict the response (Graphical User Interface)
                   To predict the sentences and get a response from the user to let us create a new file ‘chatapp.py’. We will load the trained model and then use a graphical user interface that will predict the response from the bot. The model will only tell us the class it belongs to, so we will implement some functions which will identify the class and then retrieve us a random response from the list of responses. Now we will develop a graphical user interface. Let’s use Tkinter library which is shipped with tons of useful libraries for GUI. We will take the input message from the user and then use the helper functions we have created to get the response from the bot and display it on the GUI. Here is the full source code for the GUI.
 6. Run the chatbot
          To run the chatbot, we have two main files; trainchatbot.py and chatbot.py. If we don’t see any error during training, we have successfully created the model. Then to run the app, we run the second file.python chatbot.py. The program will open up a GUI window within a few seconds. With the GUI you can easily chat with the bot.
          
Output of the chatbot is shown in the chatbot.jpeg file in the above.

![image](https://user-images.githubusercontent.com/69139140/119218565-95a4d800-bafe-11eb-8042-0deca3e53a7b.png)

                 

                   


 
