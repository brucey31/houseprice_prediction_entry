# House Price Prediction Kaggle Competition Entry

This is a quick weekend try of the house price prediction competition on kaggle

  - See https://www.kaggle.com/harlfoxem/housesalesprediction for project
  - See https://www.kaggle.com/harlfoxem/housesalesprediction/data for the data file

### Installation

I have used a whole load of libraries to get this repo going, plus the SQL Alchemy ORM to create a DB table to query and a google maps api heatmap animation

#### To install and prepare environment run
```bash
mkdir house_price_prediction
git clone {get git address from above}
virtualenv house_price_prediction

cd house_price_prediction
source bin/activate
pip install -r requirements.txt
```

### Credentials
In the first cell, after the imports you will see some creds that need filling.

1. db_name - _The db name of a postgres db that you have read write access to_
2. db_host  _The host of the postgres db_
3. db_username  _The username with read write access to the db_
4. db_password  _The password for the above user_
5. gmaps.configure(api_key="") _This is a google maps API key (See https://developers.google.com/maps/documentation/javascript/get-api-key)_



### Run it

``` sh 
jupyter nbextension enable --py gmaps
jupyter notebook
```

and you are good to go!!
