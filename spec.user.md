# User Management

## Request Header (alway pass : token) 
    You have to get "token" from login method 

# newUser

## url

http://{processServer}/newUser

## request body

```json

{
    "EMP_ID" : "01049769",
    "USER_NAME" : "Paiboon",
    "USER_SURNAME" : "Yuenyong",
    "MOBILE" : "0864126585",
    "EMAIL" : "paiboon_yue@truecorp.co.th",
    "DEPARTMENT": "Enterprise Service Development / GIS and Service Inventoy System",
    "CHIEF_EMP_ID": "01011770",
    "USER_ROLE":  "Approver", //Sale, Approver, Pricer, PDF,
    "IT_ADMIN": "Y"
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

## response (if duplicate user)

```json
{
    "RESULT_DATA": [],
    "RESULT_STATUS": "U01",
    "RESULT_MESSAGE": "Duplicate User"
}

```

# updateUser

## url
    http://{processServer}/updateUser/{empId}

## request body

```json
{
    "USER_NAME" : "Paiboon",
    "USER_SURNAME" : "Yuenyong",
    "MOBILE" : "0864126585",
    "EMAIL" : "paiboon.yue@gmail.com",
    "DEPARTMENT" : "Geographic Information System",
    "CHIEF_EMP_ID" : "01011770",
    "USER_ROLE" : "Approver",
    "IT_ADMIN" : "Y"
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

## response (if duplicate user)

```json
{
    "RESULT_DATA": [],
    "RESULT_STATUS": "U01",
    "RESULT_MESSAGE": "Duplicate User"
}

```

# deleteUser
    Use to delete user

## url
    http://{processServer}/deleteUser/{empId}

## request body (No)

## response (if success)

```json
{
    "RESULT_DATA": [],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull"
}
```

# getUserInfo
    Use to get user information

## url
    http://{processServer}/getUserInfo/{empId}

## request body (No)

## response (if success)

```json
{
    "RESULT_DATA": [
        {
            "EMP_ID": "01049769",
            "USER_NAME": "Paiboon",
            "USER_SURNAME": "Yuenyong",
            "MOBILE": "0864126585",
            "EMAIL": "paiboon.yue@gmail.com",
            "DEPARTMENT": "Geographic Information System",
            "USER_ROLE": "Approver",
            "IT_ADMIN": "Y"
        }
    ],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull"
}

```
## response (if no data found)

```json
{
    "RESULT_DATA": [],
    "RESULT_STATUS": "404",
    "RESULT_MESSAGE": "No data found"
}

```

# getUserList

## url
    http://{processServer}/getUserList/{pageNo}/{pageSize}

## request body (body empty = getAll)

```json
{
	"filter":"010",
	"orderField":"EMP_ID",
	"orderType":"-1" //1=asc, -1=desc
}

```

## response (if success)

```json
{
    "RESULT_DATA": [
        {
            "EMP_ID": "01030272",
            "USER_NAME": "Sunantha",
            "USER_SURNAME": "Aiamsamarng",
            "MOBILE": "0891565461",
            "EMAIL": "Sunantha_Aia@truecorp.co.th",
            "DEPARTMENT": "Enterprise Service Development / GIS and Service Inventoy System",
            "USER_ROLE": "Sale",
            "IT_ADMIN": "Y"
        },
        {
            "EMP_ID": "01007138",
            "USER_NAME": "Nareerat",
            "USER_SURNAME": "Preechakorn",
            "MOBILE": "0802999522",
            "EMAIL": "Nareerat_Pre@truecorp.co.th",
            "DEPARTMENT": "Enterprise Service Development / GIS and Service Inventoy System",
            "USER_ROLE": "Sale",
            "IT_ADMIN": "Y"
        }
    ],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull",
    "RESULT_TOTAL": 2
}

```

# getSaleList

## url
    http://{processServer}/getSaleList

## request body (body empty = getAll)

```json
{
	"filter":"a"
}

```

## response (if success)

```json
{
    "RESULT_DATA": [
        {
            "EMP_ID": "01007138",
            "USER_NAME": "Nareerat",
            "USER_SURNAME": "Preechakorn"
        },
        {
            "EMP_ID": "01030272",
            "USER_NAME": "Sunantha",
            "USER_SURNAME": "Aiamsamarng"
        }
    ],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull"
}

```

