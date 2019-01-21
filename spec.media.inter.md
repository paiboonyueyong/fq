# road On-Service

## collection name = "media_inter"
```json
{
    "speed_mbps": 1,
    "p_suggest_price": 1600,
    "p_ae": 1485,
    "p_ad": 1238,
    "p_dd": 1114,
    "p_director": 990,
    "i_suggest_price": 5100,
    "i_ae": 4276,
    "i_ad": 3698,
    "i_dd": 3409,
    "i_director": 3120
}
```

## getMediaInterList

* URL 
http://{server}/getMediaInterList

* Request

* Response (if success)
```json
{
    "RESULT_DATA": [
        {
            "speed_mbps": 1,
            "p_suggest_price": 1600,
            "p_ae": 1485,
            "p_ad": 1238,
            "p_dd": 1114,
            "p_director": 990,
            "i_suggest_price": 5100,
            "i_ae": 4276,
            "i_ad": 3698,
            "i_dd": 3409,
            "i_director": 3120
        },
        {
            "speed_mbps": 2,
            "p_suggest_price": 3300,
            "p_ae": 3043,
            "p_ad": 2417,
            "p_dd": 2103,
            "p_director": 1790,
            "i_suggest_price": 5400,
            "i_ae": 4552,
            "i_ad": 3896,
            "i_dd": 3568,
            "i_director": 3240
        },
        {
            "speed_mbps": 3,
            "p_suggest_price": 3900,
            "p_ae": 3621,
            "p_ad": 2876,
            "p_dd": 2503,
            "p_director": 2130,
            "i_suggest_price": 5700,
            "i_ae": 4805,
            "i_ad": 4078,
            "i_dd": 3714,
            "i_director": 3350
        },
        {
            "speed_mbps": 4,
            "p_suggest_price": 4600,
            "p_ae": 4284,
            "p_ad": 3402,
            "p_dd": 2961,
            "p_director": 2520,
            "i_suggest_price": 7200,
            "i_ae": 6081,
            "i_ad": 4776,
            "i_dd": 4123,
            "i_director": 3470
        }
    ],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull",
    "RESULT_TOTAL": 4
}
```