# Mini_Yelp
##  How is the application built
Node.JS  
server side: express  
client side: next.js, react

Install npm packages in both client/serverside
```
npm install
```
set up ```.env``` file to store mySQL password



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
### authentication  
 ![66d729e7f19a6afbca7ce6e2bb71d93](https://github.com/LifeIsHardBruh/Mini-Yelp_review_management_system/assets/43108245/deaaa1e9-f7d1-4245-aa41-eec3a739ff03)
 ![ea2654e2088b698b5bbd0eb69b79a78](https://github.com/LifeIsHardBruh/Mini-Yelp_review_management_system/assets/43108245/84808838-a100-4aa3-a1be-264df0ed4d1b)


### search business by name, category, city, state or combinations / Star Distribution for business
![9b86bb0bb2e93194973e9359baf80bc](https://github.com/LifeIsHardBruh/Mini-Yelp_review_management_system/assets/43108245/29e66f24-e98a-4759-825d-9c98dda9d16c)
![333877786f3e3b4f936a321ff99245f](https://github.com/LifeIsHardBruh/Mini-Yelp_review_management_system/assets/43108245/d6da064a-102a-48d8-8a96-fd1781ff1564)
![2a53e2d26fb7c8adf4f1142b86c4be1](https://github.com/LifeIsHardBruh/Mini-Yelp_review_management_system/assets/43108245/dc717a3e-de49-4af3-bb93-a9c4a5c605e1)
![d0624846ec4cb87235d1dacb8f663bd](https://github.com/LifeIsHardBruh/Mini-Yelp_review_management_system/assets/43108245/5a854791-57a1-4e56-858d-34cc6a44ee9c)

### write, update, delete review / thumbs up for others' comment  
![f1bea5521b22a3fa5f045fcfd95ea7e](https://github.com/LifeIsHardBruh/Mini-Yelp_review_management_system/assets/43108245/1336c742-f80c-4c22-a5cf-ff3342d4366b)

### User profile / Follow User  
![b1d0ff5eda82b8cd471773287a12663](https://github.com/LifeIsHardBruh/Mini-Yelp_review_management_system/assets/43108245/d8e354bf-bdd5-4c72-9c73-163719efb98f)
![4ba9685eafcb5f7bde3e0080e1b0c6f](https://github.com/LifeIsHardBruh/Mini-Yelp_review_management_system/assets/43108245/31e18fbf-f923-4482-b03f-b52810f91f02)















