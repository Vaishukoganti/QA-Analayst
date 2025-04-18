##API Validation using Postman and Chrome Dev tools

#Validation for Phone Number page on login page

Request url: https://api.linqapp.com/api/v3/phone_numbers

GET call

Status Code: 200k

Psotman Response:
{
    "data": {
        "phone_numbers": []
    }
}
 
Steps:
 1. Navigate the url
 2. open the Dev tools
 3. Go to Network Console tab
 4. Copy the Request Url
 5. Look for Request method
 6. Copy the Content-Type which is a key-value pair
 7. Copy the api-token 
 8. Open postman
 9. Create a New collection
 10. Select the request method
 11. paste the request url
 12. Select the header
 13. Add key as content type and values as application/json
 14. Add key as X-Linq-API-Token and values as "0b9dac67-c52d-49f9-a44c-29fed2e7011f" 
 15. Hit on Send
 16. Look for the API message 




##Validation for saving contact inside profile

 #Request url: https://api.linqapp.com/api/v2/form_fields

 Post Call

 Status code: 200k

 Request Body: 
  {
  "formable_id": 2488986,
  "formable_type": "Contact",
  "input_type": "phone_number",
  "label": "Mobile",
  "value": "4709395339"
}


Response body:

{
    "data": {
        "form_field": {
            "id": 522014,
            "formable_id": 2488986,
            "formable_type": "Contact",
            "input_type": "phone_number",
            "label": "Mobile",
            "placeholder": null,
            "value": "4709395339",
            "is_required": false,
            "updated_at": "2025-04-18T16:51:12.160-05:00"
        }
    }
}

 Steps:
 1. Navigate the url
 2. open the Dev tools
 3. Go to Network Console tab
 4. Copy the Request Url
 5. Look for Request method
 6. Copy the Content-Type which is a key-value pair
 7. Copy the api-token 
 8. Open postman
 9. Create a New collection
 10. Select the request method
 11. paste the request url
 12. Select the header
 13. Add key as content type and values as application/json
 14. Add key as X-Linq-API-Token and values as "0b9dac67-c52d-49f9-a44c-29fed2e7011f" 
 15. Add the Request body
 15. Hit on Send
 16. Look for the API message 



Findings:

x-linq-api-token: "0b9dac67-c52d-49f9-a44c-29fed2e7011f"

Usually most of them use Authorization: Bearer, but this say's No OAuth2 or cookie-based login, this is a token-auth API, likely for mobile/web hybrid apps.

