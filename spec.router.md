# road On-Service

## collection name = "router"
```json
{
    "router_model": "Cisco 2821RF",
    "rental_price": 450,
    "max_speed": 50
}
```

## getRouterList

* URL 
http://{server}/getRouterList



* Request
```json
{
    "max_speed" : "50"
}
```

* Response (if success)
```json

{
   "RESULT_DATA": [
        {
            "router_model": "Cisco 2821RF",
            "rental_price": 450,
            "max_speed": 50
        },
        {
            "router_model": "Cisco 819 4G",
            "rental_price": 760,
            "max_speed": 50
        },
        {
            "router_model": "JUNIPER,SRX300",
            "rental_price": 750,
            "max_speed": 200
        }
    ],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull",
    "RESULT_TOTAL": 3
}
```