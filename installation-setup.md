>first you have to create a virtual environment for BOT-NAME by using conda
in this environment we use python version 3.8 because rasa doesn't support python new version
```
conda create --name BOT-NAME python==3.8
```
>now you have to activate this environment by using this command
```
conda activate BOT-NAME
```
>now you have to download the update version of pip
```
python -m pip uninstall pip
python -m ensurepip
python -m pip install -U pip
```
>we have also another way to upgrade pip by using this command
```
python -m pip install --upgrade pip
```
>before downloading rasa using pip you need to install some prerequisite of rasa
```
conda install ujson
```
```
conda install tensorflow
```
>now we finally install rasa by using this command
```
pip install rasa
```
>now we check is rasa is succesfully installed

>to know rasa version
```
rasa --version
```
>to know all command for rasa
```
rasa -h
```
>first you need to run command rasa init this command is for creating new rasa projects
```
rasa init
```

>after running this command these files are created
.
├── actions
│   ├── __init__.py
│   └── actions.py
├── config.yml
├── credentials.yml
├── data
│   ├── nlu.yml
│   └── stories.yml
├── domain.yml
├── endpoints.yml
├── models
│   └── <timestamp>.tar.gz
└── tests
   └── test_stories.yml


>now we train rasa model by using this command
```
rasa train
```
>when you run this command rasa train your model will train and new file created /model folder and the default name of the foler is <timestamp>.tar.gz but if you want change the name of your model you can run this command
```
rasa train --fixed-model-name "MODEL_NAME"
```
>if we want to use our bot simply use this command
```
rasa shell
```

>if you want to create new training data by chatting to your assitant
```
rasa interactive
```
>if you want to start a server with your trained model
```
rasa run
```
>command to generate visual representaton of your stories this command will show you graph of your stores
```
rasa visualize
```
>if you want to delete conda environment
```
conda env remove -n jupiterbot
```
