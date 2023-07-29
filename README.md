# Hotel_Review_Management_System
## Database Drive Application
Node.JS  
server side: express  
client side: next.js  

Install npm packages in both client/serverside
```
npm install
```
set up ```.env``` file to store mySQL password

## Load sample datasets from localhost:3306
```
cd server-side
node initialize-database.js
```
which runs all sql script in 
[intialize-test.sql](SQL-query/sample-datasets/initialize-test.sql)

## Load production datasets
unzip the [production_dataset.tar.gz](productionDataset/production_dataset.tar.gz)
With the cleaned csv file, we can import the data in to our mysql database. We applied function “LOAD DATA INFILE ‘path’ INTO TABLE table_name” so that we can import one csv file for a table within a short period of time. In folder “productionDataset”, we created three files and implement them one by one.   
InitializedProductionTable.sql: create table and schema for the database.  
ImportProductionDataBase.sql: load the data in csv file to the table in database.  
FinalizedDBWithTrigger.sql: Set up triggers so that further insertion and update can be automated.  




## START front end on localhost:8000
```
cd client-side
npm run dev
```
```
/login
/signup
/logout
/business/:bid
/review/:rid
/main
```

## server-side: REST API on localhost:3000
```
cd server-side
nodemon(or node) index.js
```

POST ```/api/auth/signup```  **not create session cookie yet**  
POST ```/api/auth/login```   **create session cookie**  
DELETE ```/api/auth/logout``` **destroy session cookie**   

GET ```/api/business/search```  
GET ```/api/business/:bid```  
POST ```/api/business/:bid```  
POST ```/api/business/search```  


GET ```/api/review/:rid```  
PUT ```/api/review/:rid```  
DELETE ```/api/review/:rid```  
POST ```/api/review/:rid/cool```  


## feature it currently support
- authentication  


- search business by name, category, city, state or combinations  


  
- write, update, delete review  


- thumbs up for others comment  


- Star Distribution  


- Follow User  















