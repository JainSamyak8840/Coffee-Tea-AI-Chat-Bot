# Implementation of a Coffee&Tea Shop Chatbot in PyTorch.  
Chatbot implementation with PyTorch. 
- The implementation is done with a Feed Forward Neural net with 2 hidden layers.


## Installation

### Create an environment

```console
mkdir myproject
$ cd myproject
$ python3 -m venv venv
```


### Install PyTorch and dependencies

 ```console
pip install nltk
 ```

If you get an error during the first run, you also need to install `nltk.tokenize.punkt`:
Run this once in your terminal:
 ```console
$ python
>>> import nltk
>>> nltk.download('punkt')
```

## Usage
Run
```console
python train.py
```
This will dump `data.pth` file. And then run
```console
python chat.py
```
## Customize
Have a look at [intents.json](intents.json). Just define a new `tag`, possible `patterns`, and possible `responses` for the chat bot. 
```console
{
  "intents": [
    {
      "tag": "greeting",
      "patterns": [
        "Hi",
        "Hey",
        "How are you",
        "Is anyone there?",
        "Hello",
        "Good day"
      ],
      "responses": [
        "Hey :-)",
        "Hello, thanks for visiting",
        "Hi there, what can I do for you?",
        "Hi there, how can I help?"
      ]
    },
    ...
  ]
}
```
