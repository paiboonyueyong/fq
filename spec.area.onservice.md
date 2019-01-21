# Area On-Service

## collection name = "area_on_service"
```json
{
	"service" : "VDSL",
	"area_name_th" : "ฮิวโก้",
	"area_name_en" : "",
	"sub_district" : "ลาดกระบัง",
	"district" : "ลาดกระบัง",
	"province" : "กรุงเทพมหานคร",
	"charge" : 0,
	"installation_days" : 3
}
```

## getAreaOnServiceList

* URL 
http://{server}/getAreaOnServiceList

* Request

* Response (if success)
```json
{
    "RESULT_DATA": [
        {
            "services": [
                {
                    "service": "L2 Switch",
                    "charge": 2861.11,
                    "installation_days": 12
                },
                {
                    "service": "VDSL",
                    "charge": 0,
                    "installation_days": 3
                }
            ],
            "area_name": "208 วายเลส โรด กรุงเทพมหานคร,ปทุมวัน,ลุมพินี",
            "area_name_th": "208 วายเลส โรด",
            "area_name_en": "",
            "sub_district": "ลุมพินี",
            "district": "ปทุมวัน",
            "province": "กรุงเทพมหานคร"
        },
        {
            "services": [
                {
                    "service": "GPON",
                    "charge": 138.89,
                    "installation_days": 12
                },
                {
                    "service": "VDSL",
                    "charge": 0,
                    "installation_days": 3
                }
            ],
            "area_name": "253 อโศก กรุงเทพมหานคร,วัฒนา,คลองเตยเหนือ",
            "area_name_th": "253 อโศก",
            "area_name_en": "",
            "sub_district": "คลองเตยเหนือ",
            "district": "วัฒนา",
            "province": "กรุงเทพมหานคร"
        }
    ],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull",
    "RESULT_TOTAL": 2
}
```