# Chatbot Deployment with Flask and JavaScript
tutorial with Flask and JavaScript.

This gives 2 deployment options:
- Deploy within Flask app with jinja2 template
- Serve only the Flask prediction API. The used html and javascript files can be included in any Frontend application (with only a slight modification) and can run completely separate from the Flask App then.

## Initial Setup:
This repo currently contains the starter files.

Clone repo and create a virtual environment
```
$ git clone https://github.com/prabal-17/chat_bot.git
$ cd chat_bot
$ python3 -m venv venv
$ . venv/bin/activate or .\venv\Scripts\activate
```
Install dependencies
```
$  pip install Flask torch torchvision nltk
```
Install nltk package
```
$ (venv) python
>>> import nltk
>>>nltk.download('punkt')
>>>nltk.download('punkt_tab')
>>>nltk.download('averaged_perceptron_tagger')  # Just in case POS tagging is needed
>>>exit() #to get back
```
Modify `intents.json` with different intents and responses for your Chatbot

Run
```
$ (venv) python train.py
```
This will dump data.pth file. And then run
the following command to test it in the console.
```
$ (venv) python chat.py
```
To quit type below command then enter
```
$ quit
```
To run type
```
$ python app.py
```
