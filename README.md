# FLASK_RESTFUL_API_LIN_REG

Here contains code for a Restful API built using the Flask_Restful extension to Flask. 

The following classes can be found in the resources folder:
- add_data.py - this allows you to add data to the database
- create_tables.py - this will create a database to store the training data and username & passwords if one does not exist already
- db.py - this initiates the Flask_SLQAlchemy connection
- predict.py - this will allow you to send JSON data and retrieve a prediction from the lin reg model
- security.py - this will authenticate the user to provide a JSON web token (JWT)
- train.py - this will train the model or retrain the model with new data
- user.py - this will find, get and delete users from the database

Prediction: use the following format for the JSON data
{"input_data":[{"fields":["age","sex","cp","trestbps","chol","fbs","restecg","thalach","exang","oldpeak","slope","ca","thal"],
                                  "values":[[1,1,1,1,0,5,1231,1,1,1,1,1,1]]}]}
