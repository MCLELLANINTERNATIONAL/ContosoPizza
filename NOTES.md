# ContosoPizza Assignment Notes

## Additional Pizza Records Added

Additional pizza records were added to the Pizza list in `PizzaService.cs`:

- Id: 3  
  Name: Hawaii  
  IsGlutenFree: false  

- Id: 4  
  Name: Chicken Supreme  
  IsGlutenFree: false  

# API Testing Evidence

## GET Request

Endpoint:

### text
GET /Pizza

Returned Status:

### text
200 OK

Example Response:

### json
[
  {
    "id": 1,
    "name": "Classic Italian",
    "isGlutenFree": false
  },
  {
    "id": 2,
    "name": "Veggie",
    "isGlutenFree": true
  },
  {
    "id": 3,
    "name": "Hawaii",
    "isGlutenFree": false
  },
  {
    "id": 4,
    "name": "Chicken Supreme",
    "isGlutenFree": false
  }
]

## POST Request

Endpoint:

### text
POST /Pizza

Returned Status:

### text
201 Created

Example Request:

### json
{
  "name": "BBQ Chicken",
  "isGlutenFree": false
}

## PUT Request

Endpoint:

### text
PUT /Pizza/3

Returned Status:

### text
204 No Content

Example Request:

### json
{
  "id": 3,
  "name": "Hawaiian",
  "isGlutenFree": false
}

## DELETE Request

Endpoint:

### text
DELETE /Pizza/3


Returned Status:

### text
204 No Content

# Summary

ContosoPizza Web API successfully supports the following CRUD operations:

- GET
- POST
- PUT
- DELETE

All operations were tested successfully using ASP.NET Core Web API endpoints.