first you have to create a virtual environment for jupiterbot by using conda
in this environment we use python version 3.8 because rasa doesn't support python new version
```
conda create --name jupiterbot python==3.8
```
now you have to activate this environment by using this command
```
conda activate jupitebot
```
now you have to download the update version of pip
```
python -m pip uninstall pip
python -m ensurepip
python -m pip install -U pip
```
we have also another way to upgrade pip by using this command
```
python -m pip install --upgrade pip
```

now we finally install rasa by using this command
```
pip install rasa
```
now we check is rasa is succesfully installed

to know rasa version
```
rasa --version
```
to know all command for rasa
```
rasa -h
```
now we train rasa model by using this command
```
rasa train
```
if we want to use our bot simply use this command
```
rasa shell
```
and the alternate method for train and use bot
```
rasa init
```
