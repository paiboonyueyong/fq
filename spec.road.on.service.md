# road On-Service

## collection name = "road_on_service"
```json
{
    "sub_district" : "คลองเตยเหนือ",
    "district" : "วัฒนา",
    "province" : "กรุงเทพมหานคร",
	"service_result" : "กรุณาตรวจสอบ"
}
```

## getRoadOnServiceList

* URL 
http://{server}/getRoadOnServiceList

* Request
```json
{
    "sub_district" : "คลองเตยเหนือ",
    "district" : "วัฒนา",
    "province" : "กรุงเทพมหานคร"
}
```

* Response (if success)
```json
{
    "RESULT_DATA": [
        {
            "road": "สุขุมวิท",
            "sub_district": "คลองเตยเหนือ",
            "district": "วัฒนา",
            "province": "กรุงเทพมหานคร"
        }
    ],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull",
    "RESULT_TOTAL": 1
}
```