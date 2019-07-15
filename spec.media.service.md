
# Media Service

## Request Header (alway pass : token) 
    You have to get "token" from login method 

# getMediaService

## URL 

http://{server}/getMediaService

## no request body

## response (if success)

```json

{
    "RESULT_DATA": [
        {
            "MEDIA": "Copper",
            "SERVICE": "Doccis",
            "PDF_MESSAGE": ""
        },
        {
            "MEDIA": "Copper",
            "SERVICE": "VDSL",
            "PDF_MESSAGE": "ข้อความ xxxxxxx"
        },
        {
            "MEDIA": "Fiber",
            "SERVICE": "GPON",
            "PDF_MESSAGE": ""
        },
        {
            "MEDIA": "Fiber",
            "SERVICE": "L2 Switch",
            "PDF_MESSAGE": "ข้อความ yyyyyyyy"
        }
    ],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull"
}

```