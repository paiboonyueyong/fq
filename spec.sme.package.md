# SME Package

## collection name = "biz_package_fixip"
```json
{
	"package_code" : "4",
	"package_desc" : "30Mbps / 10 Mbps",
	"price" : 4249,
	"fixline_free_desc" : "1,000 บาท/เดือน"
}
```

## getSMEPackageList

* URL 
http://{server}/getSMEPackageList

* Request

* Response (if success)
```json
{
    "RESULT_DATA": [
        {
            "package_code": "1",
            "package_desc": "30Mbps / 10 Mbps",
            "price": 1349,
            "fixline_free_desc": "300 บาท/เดือน"
        },
        {
            "package_code": "2",
            "package_desc": "50Mbps / 20 Mbps",
            "price": 1549,
            "fixline_free_desc": "500 บาท/เดือน"
        },
        {
            "package_code": "3",
            "package_desc": "30Mbps / 10 Mbps",
            "price": 2349,
            "fixline_free_desc": "700 บาท/เดือน"
        },
        {
            "package_code": "4",
            "package_desc": "30Mbps / 10 Mbps",
            "price": 4249,
            "fixline_free_desc": "1,000 บาท/เดือน"
        }
    ],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull",
    "RESULT_TOTAL": 4
}
```