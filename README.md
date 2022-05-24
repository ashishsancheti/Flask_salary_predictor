# Flask_salary_predictor
This is a demo project to elaborate how Machine Learn Models are deployed on production using Flask API. It predicts the salary of the employee based on the experience, test_score, interview_score.

# Prerequisites
You must have Scikit Learn, Pandas (for Machine Leraning Model) and Flask (for API) installed.

# Project Structure
This project has four major parts :
  1. model.py - This contains code fot our Machine Learning model to predict employee salaries absed on trainign data in 'hiring.csv' file.
  2. main.py - This contains Flask APIs that receives employee details through GUI or API calls, computes the precited value based on our model and returns it.
  3. text.py - This uses requests module to call APIs already defined in app.py and dispalys the returned value.
  4. templates - This folder contains the HTML template to allow user to enter employee detail and displays the predicted employee salary.


# Running the project
  1. Run "python model.py" in terminal --> This would create a serialized version of our model into a file model.pkl
  2. Run "python main.py (in seperate terminal) to start Flask API. By default, flask will run on port 5000.
  3. Navigate to URL http://localhost:5000
