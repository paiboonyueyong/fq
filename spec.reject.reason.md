# Reject Reason

## Request Header (alway pass : token) 
    You have to get "token" from login method 

# getRejectReason

## URL 

http://{server}/getRejectReason

## request body

```json
{
    "role":"Approver"
}

```
## response (if success)

```json

{
    "RESULT_DATA": [
        {
            "REJECT_REASON": "ราคาที่ต่อรองไม่สามารถรับได้",
            "ROLE": "Approver"
        },
        {
            "REJECT_REASON": "รายได้ที่ได้รับไม่คุ้มในระยะยาว",
            "ROLE": "Approver"
        },
        {
            "REJECT_REASON": "ลูกค้าติด Black List",
            "ROLE": "Approver"
        }
    ],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull"
}

```