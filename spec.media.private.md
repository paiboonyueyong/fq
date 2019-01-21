# road On-Service

## collection name = "media_private_copper"
## collection name = "media_private"
```json
{
    "speed_mbps": 1,
    "p_suggest_price": 3400,
    "p_ae": 3100,
    "p_ad": 2800,
    "p_dd": 2600,
    "p_director": 2500
}
```

## getMediaPrivateList

* URL 
http://{server}/getMediaPrivateList



* Request
```json
{
    "media_copper" : "copper"
}
```

* Response (if success)
```json

{
    "RESULT_DATA": [
        {
            "speed_mbps": 1,
            "p_suggest_price": 3400,
            "p_ae": 3100,
            "p_ad": 2800,
            "p_dd": 2600,
            "p_director": 2500
        },
        {
            "speed_mbps": 2,
            "p_suggest_price": 3800,
            "p_ae": 3300,
            "p_ad": 2900,
            "p_dd": 2700,
            "p_director": 2500
        },
        {
            "speed_mbps": 3,
            "p_suggest_price": 4100,
            "p_ae": 3500,
            "p_ad": 3000,
            "p_dd": 2800,
            "p_director": 2500
        }
    ],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull",
    "RESULT_TOTAL": 3
}
```