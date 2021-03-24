# NEIGHBOURHOOD

Neighbourhood is a simple API allowing consumers to:
* Store information about the household members, houses and addresses; 
* Provide the lookup of the house, owners and address;  
* Find people in the neighbourhood according the age groups or household sizes;

The application uses REST architecture. It uses common [HTTP response](https://cybersguards.com/http-response-codes/) codes. Accepts [form encoded](https://dev.to/sidthesloth92/understanding-html-form-encoding-url-encoded-and-multipart-forms-3lpa)  data and returns JSON format data. 


## API BLUEPRINT

+ [Raw API Blueprint](https://github.com/gretaivan/neighbourhood-api/blob/main/apiary.apib)
+ [Mock Server](https://app.apiary.io/neighbourhoodapi/editor)

## USAGE 

## Home Route [/]

### Connection Successful [GET]

+ Response 200 (text/plain)

        You successfully connected to the Neighbourhood API
    
## House Collection [/houses]

### List All Houses [GET]

+ Response 200 (application/json)
            
            [
                 {
                    "id:" 2,
                    "address": "London",
                    "owner": "Harry Potter"
                }
            ]
    

### Create a new House [POST]

+ Request (application/json)

        {
            "address": "London",
            "owner": "Harry Potter"
        }

+ Response 201 (application/json)

    + Headers

            Location: /houses/2

    + Body
            
            {
                "id:" 2,
                "address": "London",
                "owner": "Harry Potter"
            }

    + Schema
    

            {
                "$schema": "http://json-schema.org/draft-04/schema#",
                "type": "object",
                "properties": {
                    "address": "string",
                    "owner": "string"
                }
            }
            
## HTTP REQUEST TYPES
```GET``` - to get the data resources
```POST``` - to create a new data resource

## HTTP RESPONSE CODES IN API

```200``` ```OK```
```201``` ```Created```

## INSTALLATION AND USAGE for developers
 
### Instalation 
* Fork and clone the repo  
* cd into the cloned repo 
* in terminal ```npm install```