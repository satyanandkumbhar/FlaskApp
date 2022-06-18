# Basic flask app
Uses Flask & Sqlite

#### Creating virtual env - mac OS
```
python3 -m venv env
```

#### Activating virtual env - mac OS
```
source env/bin/activate
```


#### De-activating virtual env - mac OS
```
deactivate
```

#### installing all dependencies/libraries from requirements.txt
```
pip3 install -r requirements.txt
```

#### How to run
Multiple options to run this app
* You can run this app as standalone application with python3 app.py
  * python3 app.py
* Run in docker container - use following steps
  * docker build -t flaskapp .
  * docker run flaskapp
* Deploy using pipeline
  * Use the provided Jenkins file to create a pipeline
  * The jenkins will do all the steps
  * Application will be accessible at port 5000
