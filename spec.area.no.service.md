# Area No-Service

## collection name = "area_no_service"
```json
{
	"area_name_th" : "ปัญจธานี",
	"area_name_en" : "Panjathani Tower",
	"sub_district" : "ช่องนนทรี",
	"district" : "ยานนาวา",
	"province" : "กรุงเทพมหานคร",
	"service_result" : "ไม่สามารถให้บริการได้"
}
```

## getAreaNoServiceList

* URL 
http://{server}/getAreaNoServiceList

* Request
```json
{
    "sub_district" : "ห้วยขวาง",
    "district" : "ห้วยขวาง",
    "province" : "กรุงเทพมหานคร"
}
```

* Response (if success)
```json
{
    "RESULT_DATA": [
        {
            "_id": "5bce12e1fecc161c28f9b386",
            "area_name_th": "เดอะ แกรนด์ พระราม 9",
            "area_name_en": "The Grand Rama 9 ",
            "sub_district": "ห้วยขวาง",
            "district": "ห้วยขวาง",
            "province": "กรุงเทพมหานคร",
            "service_result": "ไม่สามารถให้บริการได้",
            "area_name": "เดอะ แกรนด์ พระราม 9 กรุงเทพมหานคร,ห้วยขวาง,ห้วยขวาง"
        },
        {
            "_id": "5bce12e1fecc161c28f9b388",
            "area_name_th": "ที.ซี.กรีน",
            "area_name_en": "TC Green",
            "sub_district": "ห้วยขวาง",
            "district": "ห้วยขวาง",
            "province": "กรุงเทพมหานคร",
            "service_result": "ไม่สามารถให้บริการได้",
            "area_name": "ที.ซี.กรีน กรุงเทพมหานคร,ห้วยขวาง,ห้วยขวาง"
        },
        {
            "_id": "5bce12e1fecc161c28f9b38a",
            "area_name_th": "LPN พระราม 9",
            "area_name_en": "",
            "sub_district": "ห้วยขวาง",
            "district": "ห้วยขวาง",
            "province": "กรุงเทพมหานคร",
            "service_result": "ไม่สามารถให้บริการได้",
            "area_name": "LPN พระราม 9 กรุงเทพมหานคร,ห้วยขวาง,ห้วยขวาง"
        }
    ],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull",
    "RESULT_TOTAL": 3
}
```