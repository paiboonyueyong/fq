# WorkFlow Management

## Request Header (alway pass : token) 
    You have to get "token" from login method 
       
# setQuotationExpire

## url

    http://{processServer}/setQuotationExpire/{quotationNo}

## request body

```json

{
	"expireDate": "22/01/2019" // format --> DD/MM/YYYY  
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

# pdfConfirmLocation

## url

    http://{processServer}/pdfConfirmLocation/{quotationNo}/{locationId}

## request body

```json

{
    "NETWORK_STS" : "G",
    "SERVICE" : "GPON",
    "EQUIPMENT" : "BKK000XXX",
    "DW_LENGTH" : 25.0,
    "LENGTH_TOTAL" : 1500.0,
    "PDF_MESSAGE" : "ถ้าเลือก GPON หรือ L2Switch ให้ดึง default ข้อความมาจาก QT_MEDIA_SERVICE.PDF_MESSAGE",
    "REJECT_REASON" : "เลือก drowdown ดึงข้อมูลจาก QT_REJECT_REASON (ROLE=PDF) แต่ถ้าเลือกอื่นๆ ให้ระบุข้อมูลเอง",
    "ADDITIONAL_INFO" : "กรอกหรือไม่กรอกก็ได้" 
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

# setPriceEvaluate

## url

    http://{processServer}/setPriceEvaluate/{quotationNo}/{locationId}

## request body

```json

{
	"priceEvalResult": "ราคาไม่สามารถลดได้ต่ำกว่า 20,000 บาท"
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

# approveQuotation

## url

    http://{processServer}/approveQuotation/{quotationNo}

## request body (No)

## response (if success)

```json

{
    "RESULT_DATA": [],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull"
}

```

# rejectQuotation

## url

    http://{processServer}/rejectQuotation/{quotationNo}

## request body

```json

{
	"rejectReason": "บริษัทไม่อยากขาย"
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

# delegateQuotation

## url

    http://{processServer}/delegateQuotation/{quotationNo}/{toSaleEmpId}

## request body (No)

## response (if success)

```json

{
    "RESULT_DATA": [],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull"
}

```