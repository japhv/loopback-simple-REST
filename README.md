# Gems REST API implementation using loopback

Visit https://gems-app.herokuapp.com/explorer/ (click "List Operations") to checkout the API documentation and also to play around with the API.

## Introduction
This is a REST API for your shiny gems!

Below are the current contents of your crystal pouch:

Id | Name | Unit Price | Count
---|------|------------|-------
 1 | Ruby | 100 | 50
 2 | Diamond | 500 | 10
 3 | Emerald | 400 | 40
 4 | Saphire | 1000 | 30
 
 Now you can use the REST api to add/modify/delete the contents of your crystal pouch
 
 For example, to add __Pearls__ to your crystal pouch you can 
 ```
 curl -X POST --header "Content-Type: application/json" --header "Accept: application/json" -d "{
  \"name\": \"Pearl\",
  \"unitPrice\": 30,
  \"count\": 100
}" "https://gems-app.herokuapp.com/api/gems"
 ```
 
 ## Setup
 
 ### Prerequisites
* [Git](https://git-scm.com/downloads)
* [PostgreSQL](https://www.postgresql.org/download/)
* [Node 6.x](https://nodejs.org/en/download/)
* npm 3.x ( or yarn)

### Installation

```
git clone https://github.com/japhv/loopback-simple-REST.git
cd loopback-simple-REST
npm install
```

### Running the application
To run the application simply type
```
node .
```

If all the packages and modules installed successfully you'll get the following message
```
Web server listening at: http://0.0.0.0:3000
Browse your REST API at http://0.0.0.0:3000/explorer
```
