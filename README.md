# NEIGHBOURHOOD
## [API documentation](https://neighbourhoodapi.docs.apiary.io/)

Neighbourhood is a simple API allowing consumers to:
* Store information about the household members, houses and addresses; 
* Provide the lookup of the house, owners and address;  
* Find people in the neighbourhood according the age groups or household sizes;

The application uses REST architecture. It uses common [HTTP response](https://cybersguards.com/http-response-codes/) codes. Accepts [form encoded](https://dev.to/sidthesloth92/understanding-html-form-encoding-url-encoded-and-multipart-forms-3lpa)  data and returns JSON format data. 


## API BLUEPRINT

+ [Raw API Blueprint](https://github.com/gretaivan/neighbourhood-api/blob/main/apiary.apib)
+ [Mock Server](https://app.apiary.io/neighbourhoodapi/editor)

## USAGE - A QUICK SUMMARY

### HTTP REQUEST TYPES
+ ```GET``` - to get the data resources
+ ```POST``` - to create a new data resource

### HTTP RESPONSE CODES IN API

+ ```200``` ```OK```
+ ```201``` ```Created```

### Home Route: /

#### Connection Successful - request type GET 
+ Response 200 (application/json)
    
### House Collection route: /houses

#### List All Houses request type GET 

+ Response 200 (application/json)
            
#### Create a new House - request type POST 

+ Request (application/json)

+ Response 201 (application/json)
         

## INSTALLATION AND USAGE for developers
 
### Instalation 
* Fork and clone the repo  
* cd into the cloned repo 
* in terminal ```npm install```
