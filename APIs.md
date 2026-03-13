## Update User Email

Updates the email address of the logged-in user.

### Headers

    Authorization: Bearer <token>
    Content-Type: application/json

**Endpoint:** `/api/user/email`  
**Method:**`PUT`  
### Request Body:

    {
       "email": "akku@email.com"
    }

### Success Response:
**Status code: `200 OK`**

      json
        {
           "message": "Email updated successfully"
        }

### Error Responses
**Status code: `400 Bad Request`**

      json
        {
           "error": "Invalid email format"
        }

**Status code: `401 Unauthorized`**

      json
        {
           "error": "Unauthorized access"
        }
         
**Status code: `404 Not Found`**

      json
        {
           "error": "User not found"
        }

### Validation Rules
• **email** (string) – Required  
• Must be a valid email address.

------------------------------------------------

## Get User Videos API

Retrieves videos associated with the logged-in user.

----------


### Headers

    Authorization: Bearer <token>
    Content-Type: application/json

----------

**Endpoint:** `/api/user/videos`  
**Method:** `GET`  

----------


### Query Parameters

• **limit** (number) – Optional  
Number of videos to return

----------


### Success Response:
**Status code: `200 OK`**

    {     "videos":  [ 
           {
             "id": "vid_001",
             "title": "Travel Vlog",
             "duration": "10:25"
           }   
        ]
    }

----------

### Error Responses
**Status code: `400 Bad Request`**

      json
        {
          "error": "No videos found"
        }

**Status code: `401 Unauthorized`**

      json
        {
          "error": "Unauthorized access"
        }

         
**Status code: `404 Not Found`**

      json
        {
          "error": "User not found"
        }

------------------------------------------------

## Get Video Details

Retrieves detailed information for a specific video.

----------

**Endpoint:** `/api/videos/{videoId}`  
**Method:** `GET`

----------

### Path Parameters

• **videoId** (string) – Required  
Unique identifier of the video

----------

### Headers

`Authorization: Bearer <token>
Content-Type: application/json` 

----------

### Example Request

`GET /api/videos/vid_001` 

----------

### Success Response

**Status Code:** `200 OK`

    {  
      "id":  "vid_001",  
      "title":  "Travel Vlog",  
      "duration":  "10:25",  
      "quality":  "HD"  
    }

----------

### Error Responses

----------

**Status Code:** `401 Unauthorized`

    `{  
       "error":  "Unauthorized access"  
     }` 

**Status Code:** `404 Not Found`

    `{  
       "error":  "Video not found"  
     }`

------------------------------------------------

## Search Videos

Retrieves videos matching the search criteria.

----------

**Endpoint:** `/api/videos/search`  
**Method:** `GET`

----------

### Query Parameters

• **query** (string) – Required  
Search keyword or phrase

• **limit** (number) – Optional  
Number of videos to return

• **sortBy** (string) – Optional  
Field used for sorting (e.g., duration, title)

• **order** (string) – Optional  
Sort order: asc | desc

----------

### Headers

`Authorization: Bearer <token>
Content-Type: application/json` 

----------

### Example Request

`GET /api/videos/search?query=old+songs&limit=10&sortBy=duration&order=desc` 

----------

### Success Response

**Status Code:** `200 OK`

    {  
        "totalCount": 120,  
        "page": 1,  
        "limit": 10,  
        "videos": [  
         {  
            "id": "vid_001",  
            "title": "Old Songs Collection",  
            "duration": "10:25",  
            "quality": "HD"  
          }  
       ]
    }

----------

### Error Responses

----------

**Status Code:** `400 Bad Request`

    {  
       "error":  "Invalid query parameter"  
    }

**Status Code:** `401 Unauthorized`

    {  
       "error":  "Unauthorized access"  
    }

**Status Code:** `404 Not Found`

    {  
       "error":  "No videos found"  
    }

------------------------------------------------

## Create Playlist

Creates a new playlist for the logged-in user.

----------

**Endpoint:** `/api/playlists`  
**Method:** `POST`

----------

### Headers

`Authorization: Bearer <token>
Content-Type: application/json` 

---------

### Request Body

    {  
       "name": "My Favorites",  
       "description": "Collection of favorite videos"  
    }

----------
### Request Body Parameters

|Field           |Type                          |Required                         |Description                            |
|----------------|-------------------------------|-----------------------------|---------------|
|Name |String            |Yes            |Name of the playlist|
|Description          |String |No   | Short description of the playlist|


----------


### Success Response

**Status Code:** `201 Created`

    {  
       "id": "pl_001",  
       "name": "My Favorites",  
       "description": "Collection of favorite videos"  
    }

--------------
### Response Fields
|Field|Type|Description|
|-------|-----------|----------------|
|id | string  |Unique identifier of the playlist|
|name | string  |Name of the playlist|
|description | string  |Playlist description|
----------

### Error Responses


**Status Code:** `400 Bad Request`

    {  
       "error": "Playlist name is required"  
    }

**Status Code:** `401 Unauthorized`

    {  
        "error":  "Unauthorized access"  
    } 
