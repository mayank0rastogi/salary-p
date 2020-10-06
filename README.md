## ML-Model-Heroku-Deployment
This is a My First project to elaborate how Machine Learn Models are deployed on production using Flask API on the Local Computer as Well as Heroku

### Prerequisites
You must have Scikit Learn, Pandas (for Machine Leraning Model) and Flask (for API) installed.

### Project Structure
This project has four major parts :
1. untitled.ipny - This contains code fot our Machine Learning model to predict employee salaries absed on trainign data in 'hiring.csv' file.
2. app.py - This contains Flask APIs that receives employee details through GUI or API calls, computes the precited value based on our model and returns it.
4. templates(index.html)/Static(css) - This folder contains the HTML template to allow user to enter employee detail and displays the predicted employee salary and some simple styling using Style.css.


### Running the project
1.Create the machine learning model by running below File in google collab -
```
 untitled3.ipynb
```
This would create a serialized version of our model into a file model.pkl

2. Run app.py using below command to start Flask API
```
python app.py
```
By default, flask will run on port 5000 

3. Navigate to localhost URL http://127.0.0.1:5000/

You Can Also Deploy the Model on Heroku
```
https://salary-p.herokuapp.com/predict
```

You should be able to view the homepage as below :
![alt text]()

Enter valid numerical values in all 3 input boxes and hit Predict.

If everything goes well, you should  be able to see the predcited salary vaule on the HTML page!
![alt text](http://www.thepythonblog.com/wp-content/uploads/2019/02/Result.png)

