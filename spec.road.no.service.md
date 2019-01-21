# road No-Service

## collection name = "road_no_service"
```json
{
    "sub_district": "สีลม",
    "district": "บางรัก",
    "province": "กรุงเทพมหานคร",
	"service_result" : "กรุณาตรวจสอบ"
}
```

## getRoadNoServiceList

* URL 
http://{server}/getRoadNoServiceList

* Request
```json
{
    "sub_district": "สีลม",
    "district": "บางรัก",
    "province": "กรุงเทพมหานคร"
}
```

* Response (if success)
```json
{
    "RESULT_DATA": [
        {
            "road": "สีลม",
            "sub_district": "สีลม",
            "district": "บางรัก",
            "province": "กรุงเทพมหานคร"
        },
        {
            "road": "สาทรเหนือ",
            "sub_district": "สีลม",
            "district": "บางรัก",
            "province": "กรุงเทพมหานคร"
        }
    ],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull",
    "RESULT_TOTAL": 2
}
```