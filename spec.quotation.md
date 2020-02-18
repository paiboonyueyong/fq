# Quotation Management

## Request Header (alway pass : token) 
    You have to get "token" from login method 
       
# saveQuotation

## url

    http://{processServer}/saveQuotation/

## request body

```json

{
	"CUSTOMER_NAME": "บริษัท แมคโคร์222",
	"PLAN_ID": "PR002",
	"PROJECT": "Y",
	"SME": "N",
	"MEDIA_PLAN": {
	    "SERVICE_TYPE": "Internet",
	    "CONNECTION": "VPN"
	}
}
    
```
## response (if success)

```json

{
    "RESULT_DATA": [],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull"
}

```

## response (if duplicate quotation no)

```json

{
    "RESULT_DATA": [],
    "RESULT_STATUS": "Q01",
    "RESULT_MESSAGE": "Duplicate Quotation No."
}

```

# deleteQuotation
    Use to delete quotation

## url
    http://{processServer}/deleteQuotation/{quotationNo}

## request body (No)

## response (if success)

```json
{
    "RESULT_DATA": [],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull"
}
```

# getQuotationInfo
    Use to get information of quotation

## url
    http://{processServer}/getQuotationInfo/{quotationNo}

## request body (No)

## response (if success)

```json

{
    "RESULT_DATA": [
        {
            "QUOTATION_NO": "Q0701201900002",
            "CUSTOMER_NAME": "บริษัท แมคโคร์",
            "REQUESTED_DATE": "2019-01-15T10:48:12.191Z",
            "PRINTED_DATE": "2019-01-15T10:48:12.191Z",
            "EXPIRED_DATE": "2019-01-15T10:48:12.191Z",
            "PLAN_ID": "PR002",
            "EQUIP_TOTAL": 500,
            "ADD_SERVICE_TOTAL": 1000,
            "VAS_TOTAL": 3790,
            "VAS_DISCOUNT": 500,
            "TOTAL_PRICE": 47900,
            "TOTAL_TARGET_PRICE": 40000,
            "TOTAL_DISCOUNT_PRICE": 7900,
            "NET_PRICE": 40000,
            "STATUS": "Approved",
            "PROJECT": "Y",
            "SME": "N",
            "SME_PACKAGE": {
                "PACKAGE_CODE": "30Mbps / 10 Mbps (ฟรีค่าโทร 300 บาท/เดือน)"
            },
            "MEDIA_PLAN": {
                "SERVICE_TYPE": "Internet",
                "CONNECTION": "VPN"
            },
            "SALE_EMP_ID": "01007138",
            "CREATED_BY": "01007138",
            "CREATED_DATE": "11/01/2019, 10:30:11",
            "LAST_UPDATED_BY": "01049769",
            "LAST_UPDATED_DATE": "2019-01-16T09:13:19.573Z",
            "APPROVE_ID": "01007156",
            "APPROVE_DATE": "26/01/2019, 16:30:11",
            "REJECT_REASON": "ลูกค้าติด blacklist",
            "PRICE_EVAL_RESULT": "ประเมินราคาแล้วไม่สามารถคิดราคาได้ต่ำกว่า xxx บาท",
            "LOCATION": [
                {
                    "LOCATION_ID": "R000001",
                    "FC_CODE": "B3",
                    "PRICER_PRICE": 8400,
                    "LATITUDE": 13.715946,
                    "LONGITUDE": 100.576043,
                    "START_DEST": "ต้นทาง",
                    "BUILDING_NAME": "อาคารทดสอบ 2",
                    "ADDRESS": "123 ถ.ทดสอบ คลองเตย คลองตัน กทม 10310",
                    "KM": 400,
                    "PROJECT": "Y",
                    "EXISTING_CPE": "N",
                    "INSTALLATION_DAYS": 15,
                    "INTER_SPEED_MBPS": 10,
                    "INTER_SPEED_PRICE": 3790,
                    "DOMESTIC_SPEED_MBPS": 15,
                    "DOMESTIC_SPEED_PRICE": 4790,
                    "TOTAL_PRICE": 9600,
                    "TARGET_PRICE": 8600,
                    "DISCOUNT_PRICE": 1000,
                    "NET_PRICE": 8600,
                    "CREATED_BY": "01007138",
                    "CREATED_DATE": "2019-01-15T10:48:12.191Z",
                    "LAST_UPDATED_BY": "01007156",
                    "LAST_UPDATED_DATE": "2019-01-15T10:48:12.191Z",
                    "APPROVE_ID": "01007156",
                    "APPROVE_ID_BY": "Wutthin",
                    "APPROVE_DATE": "2019-01-15T10:48:12.191Z",
                    "NETWORK_STS": "Y",
                    "PDF_CONFIRM": {
                        "PDF_CONFIRMED_DATE": "2019-01-15T10:48:12.191Z",
                        "NETWORK_STS": "G",
                        "SERVICE": "GPON",
                        "EQUIPMENT": "BKK000XXX",
                        "DW_LENGTH": 25,
                        "LENGTH_TOTAL": 1500,
                        "PDF_MESSAGE": "ถ้าเลือก GPON หรือ L2Switch ดึง default ข้อความมาจาก qt_media_service.pdf_message",
                        "REJECT_REASON": "qt_reject_reason (role=pdf) if select other fill by self",
                        "ADDITIONAL_INFO": "กรอกหรือไม่กรอกก็ได้"
                    },
                    "PRICE_SUMMARY": [
                        {
                            "LOCATION_ID": "R0000001",
                            "CODE": "M0001",
                            "SERVICE_GROUP": "Link speed",
                            "SERVICE_DESC": "Link speed Desc",
                            "SPEED": 15,
                            "TOTAL_PRICE": 1000,
                            "DISCOUNT_PRICE": 500,
                            "DISCOUNT_PERCENTAGE": 50
                        },
                        {
                            "LOCATION_ID": "R0000001",
                            "CODE": "R0001",
                            "SERVICE_GROUP": "Router",
                            "SERVICE_DESC": "Cisco 1803 RF",
                            "SPEED": 15,
                            "TOTAL_PRICE": 1000,
                            "DISCOUNT_PRICE": 500,
                            "DISCOUNT_PERCENTAGE": 50
                        },
                        {
                            "LOCATION_ID": "R0000001",
                            "SERVICE_GROUP": "Charge",
                            "TOTAL_PRICE": 1000,
                            "DISCOUNT_PRICE": 500,
                            "DISCOUNT_PERCENTAGE": 50
                        }
                    ]
                },
                {
                    "LOCATION_ID": "R000002",
                    "FC_CODE": "B3",
                    "LATITUDE": 14.715946,
                    "LONGITUDE": 100.576043,
                    "START_DEST": "ปลายทาง",
                    "BUILDING_NAME": "อาคารทดสอบ 1",
                    "ADDRESS": "123 ถ.ทดสอบ คลองเตย คลองตัน กทม 10310",
                    "KM": 400,
                    "PROJECT": "Y",
                    "EXISTING_CPE": "N",
                    "INSTALLATION_DAYS": 15,
                    "INTER_SPEED_MBPS": 10,
                    "INTER_SPEED_PRICE": 3790,
                    "DOMESTIC_SPEED_MBPS": 15,
                    "DOMESTIC_SPEED_PRICE": 4790,
                    "TOTAL_PRICE": 9600,
                    "TARGET_PRICE": 8600,
                    "DISCOUNT_PRICE": 1000,
                    "NET_PRICE": 8600,
                    "CREATED_BY": "01007138",
                    "CREATED_DATE": "2019-01-15T10:48:12.191Z",
                    "LAST_UPDATED_BY": "2019-01-15T10:48:12.191Z",
                    "LAST_UPDATED_DATE": "2019-01-15T10:48:12.191Z",
                    "APPROVE_ID": "01007156",
                    "APPROVE_DATE": "2019-01-15T10:48:12.191Z",
                    "NETWORK_STS": "G",
                    "PRICE_SUMMARY": [
                        {
                            "LOCATION_ID": "R000002",
                            "CODE": "M0001",
                            "SERVICE_GROUP": "Link speed",
                            "SERVICE_DESC": "Link speed Desc",
                            "SPEED": 15,
                            "TOTAL_PRICE": 1000,
                            "DISCOUNT_PRICE": 500,
                            "DISCOUNT_PERCENTAGE": 50
                        },
                        {
                            "LOCATION_ID": "R000002",
                            "CODE": "R0001",
                            "SERVICE_GROUP": "Router",
                            "SERVICE_DESC": "Cisco 1803 RF",
                            "SPEED": 15,
                            "TOTAL_PRICE": 1000,
                            "DISCOUNT_PRICE": 500,
                            "DISCOUNT_PERCENTAGE": 50
                        },
                        {
                            "LOCATION_ID": "R000002",
                            "SERVICE_GROUP": "Charge",
                            "TOTAL_PRICE": 1000,
                            "DISCOUNT_PRICE": 500,
                            "DISCOUNT_PERCENTAGE": 50
                        }
                    ]
                }
            ],
            "INTERNET_VAS": [
                {
                    "CODE": "DVS1",
                    "SERVICE_DESC": "CPU 1 RAM(GB) 2 HDD(GB) 100, No OS",
                    "UNIT": 1,
                    "TOTAL_PRICE": 1890,
                    "PRINT_FLAG": "Y"
                },
                {
                    "CODE": "DVS2",
                    "SERVICE_DESC": "CPU 1 RAM(GB) 2 HDD(GB) 100, No OS",
                    "UNIT": 1,
                    "TOTAL_PRICE": 1890,
                    "PRINT_FLAG": "Y"
                }
            ],
            "EQUIPMENT_NETWORK": [
                {
                    "CODE": "EQ0001",
                    "SERVICE_DESC": "NT123",
                    "UNIT": 1,
                    "TOTAL_PRICE": 4890,
                    "PRINT_FLAG": "Y"
                }
            ],
            "ADDITIONAL_SERVICE": [
                {
                    "CODE": "AD0001",
                    "SERVICE_DESC": "IphoneX",
                    "UNIT": 1,
                    "TOTAL_PRICE": 4890,
                    "PRINT_FLAG": "Y"
                }
            ]
        }
    ],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull"
}

```

# getQuotationList

## url
    http://{processServer}/getQuotationList/{pageNo}/{pageSize}

## request body (body empty = getAll)

```json

{
	"filter":"",
	"customerName":"แมค",
	"orderField": "MEDIA_PLAN.CONNECTION",
	"orderType": 1 // 1=asc, -1=desc
}

```

## response (if success)

```json
{
    "RESULT_DATA": [
        {
            "QUOTATION_NO": "Q0701201900001",
            "CUSTOMER_NAME": "บริษัท แมคโคร์",
            "REQUESTED_DATE": "2019-01-15T10:46:49.137Z",
            "STATUS": "Approved",
            "MEDIA_PLAN": {
                "SERVICE_TYPE": "Internet",
                "CONNECTION": "VPN"
            },
            "APPROVE_ID": "01007156"
        },
        {
            "QUOTATION_NO": "Q0701201900002",
            "CUSTOMER_NAME": "บริษัท แมคโคร์",
            "REQUESTED_DATE": "2019-01-15T10:48:12.191Z",
            "STATUS": "Approved",
            "MEDIA_PLAN": {
                "SERVICE_TYPE": "Internet",
                "CONNECTION": "VPN"
            },
            "APPROVE_ID": "01007156"
        },
        {
            "CUSTOMER_NAME": "บริษัท แมคโคร์",
            "REQUESTED_DATE": "2019-01-15T10:48:12.191Z",
            "STATUS": "Approved",
            "MEDIA_PLAN": {
                "SERVICE_TYPE": "Internet",
                "CONNECTION": "VPN"
            },
            "QUOTATION_NO": "Q1601201900001"
        },
        {
            "CUSTOMER_NAME": "บริษัท แมคโคร์222",
            "REQUESTED_DATE": "2019-01-15T10:48:12.191Z",
            "STATUS": "Approved",
            "MEDIA_PLAN": {
                "SERVICE_TYPE": "Internet",
                "CONNECTION": "VPN"
            },
            "QUOTATION_NO": "Q1601201900002"
        },
        {
            "CUSTOMER_NAME": "บริษัท แมคโคร์222",
            "REQUESTED_DATE": "2019-01-15T10:48:12.191Z",
            "STATUS": "Approved",
            "MEDIA_PLAN": {
                "SERVICE_TYPE": "Internet",
                "CONNECTION": "VPN"
            },
            "QUOTATION_NO": "Q1601201900003"
        }
    ],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull",
    "RESULT_TOTAL": 5
}

```


# getReportList

## url
    http://{processServer}/getReportList/{pageNo}/{pageSize}

## request body (body empty = getAll)

```json

{
	"startDate": "05/02/2020",
	"endDate": "05/02/2020",
	"orderField": "MEDIA_PLAN.CONNECTION",
	"orderType": 1  // 1=asc, -1=desc
}

```

## response (if success)

```json
{
    "RESULT_DATA": [
        {
            "QUOTATION_NO": "FC2020020500348",
            "CREATED_DATE": "05/02/2020",
            "SERVICE_TYPE": "Private",
            "CONNECTION": "VPN",
            "SALE_EMP_NAME": "จงจิตร เครือศรี",
            "DEPARTMENT": "GIS and Service Inventoy System",
            "LOCATION": [
                {
                    "BUILDING_NAME": " อาคาร KSP",
                    "HOUSE_NO": "296",
                    "SUB_DISTRICT": "ห้วยขวาง",
                    "DISTRICT": "ห้วยขวาง",
                    "PROVINCE": "กรุงเทพมหานคร",
                    "DOMESTIC_SPEED_MBPS": "100",
                    "INTER_SPEED_MBPS": null,
                    "MEDIA": "Fiber",
                    "PDF_LCN": {
                        "EQUIPMENT": "",
                        "DW": "",
                        "DISTANCE": ""
                    },
                    "DISTANCE": "0.43"
                }
            ]
        }
    ],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull",
    "RESULT_TOTAL": 1
}

```