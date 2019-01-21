# VAS Management

## vas collection

```json

{
    "package_code": "WH05",
    "package_desc": "Web Host 500 MB",
    "gm_price": 100, /* price = gm_price + gm_price*(0.5) => (margin = 50%) */
    "period": "M", /* M = "Month", O = "One time charge" */
    "group": "Web Host",
    "sub_group": "",
    "type": "Main" /* Main, Optional (before buy optional type must be buy main type first) */
}

```

## vas group

```json

["Web Host", "Database Host", "Mail Hosting", "Mail Relay Cleanner",
 "Mail Backup", "Traffic exchange", "Virtual Server", "Ddos"]

```

# getVasGroupList

## url
    http://{server}/getVasGroupList

## response (if success)

```json
{
    "RESULT_DATA": [
        {
            "group": "Web Host"
        },
        {
            "group": "Database Host"
        }
    ],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull"
}

```

# getVasList

## url
    http://{server}/getVasList

## response (if success)

```json
{
    "RESULT_DATA": [
        {
            "package_code": "DVS1",
            "package_desc": "CPU 1 RAM(GB) 2 HDD(GB) 100, No OS",
            "price": 100, 
            "period": "M",
            "group": "Virtual Server",
            "sub_group": "self managed",
            "type": "Main"
        },
        {
            "package_code": "RM2",
            "package_desc": "RAM 2 GB (Hardware)",
            "price": 1440, 
            "period": "M",
            "group": "Virtual Server",
            "sub_group": "self managed",
            "type": "Optional"
        }
    ],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull"
}
```

```json
{
    "RESULT_DATA": [
        {
            "main" : {
                "TI Manage" :[
                    {
                        "package_code" : "VST1",
                        "package_desc" : "CPU 1 RAM(GB) 2 HDD(GB) 100, No OS , Add On  Firewall + IPS , Backup Snapshot  Full (2 Week)",
                        "period" : "M",
                        "sub_group" : "TI managed",
                        "gm_price" : 5200,
                    },
                    {
                        "package_code" : "VST2",
                        "package_desc" : "CPU 1 RAM(GB) 4 HDD(GB) 200, No OS , Add On  Firewall + IPS , Backup Snapshot  Full (2 Week)",
                        "period" : "M",
                        "sub_group" : "TI managed",
                        "gm_price" : 8000,
                    },
                    {
                        "package_code" : "VST3",
                        "package_desc" : "CPU 2 RAM(GB) 4 HDD(GB) 200, No OS , Add On  Firewall + IPS , Backup Snapshot  Full (2 Week)",
                        "period" : "M",
                        "sub_group" : "TI managed",
                        "gm_price" : 9600                    
                    },
                    {
                        "package_code" : "VST4",
                        "package_desc" : "CPU 2 RAM(GB) 8 HDD(GB) 200, No OS , Add On  Firewall + IPS , Backup Snapshot  Full (2 Week)",
                        "period" : "M",
                        "sub_group" : "TI managed",
                        "gm_price" : 16000
                    },
                    {
                        "package_code" : "VST5",
                        "package_desc" : "CPU 4 RAM(GB) 8 HDD(GB) 500, No OS , Add On  Firewall + IPS , Backup Snapshot  Full (2 Week)",
                        "period" : "M",
                        "sub_group" : "TI managed",
                        "gm_price" : 18700,
                    }
                ],
                "self managed" :[
                    {
                        "package_code" : "DVS5",
                        "package_desc" : "CPU 4 RAM(GB) 8 HDD(GB) 500, No OS",
                        "period" : "M",
                        "sub_group" : "self managed",
                        "gm_price" : 9900
                    },
                    {
                        "package_code" : "DVS1",
                        "package_desc" : "CPU 1 RAM(GB) 2 HDD(GB) 100, No OS",
                        "period" : "M",
                        "sub_group" : "self managed",
                        "gm_price" : 3790
                    },
                    {
                        "package_code" : "DVS2",
                        "package_desc" : "CPU 1 RAM(GB) 4 HDD(GB) 200, No OS",
                        "period" : "M",
                        "sub_group" : "self managed",
                        "gm_price" : 4900
                    },
                    {
                        "package_code" : "DVS3",
                        "package_desc" : "CPU 2 RAM(GB) 4 HDD(GB) 200, No OS",
                        "period" : "M",
                        "sub_group" : "self managed",
                        "gm_price" : 5800
                    },
                    {
                        "package_code" : "DVS4",
                        "package_desc" : "CPU 2 RAM(GB) 8 HDD(GB) 200, No OS",
                        "period" : "M",
                        "sub_group" : "self managed",
                        "gm_price" : 7600
                    }
                ]
            },
            "options": [
                {
                    "package_code" : "HD5",
                    "package_desc" : "Disk space 500GB  (Hardware)",
                    "period" : "M",
                    "sub_group" : "Optional",
                    "gm_price" : 2000
                },
                {
                    "package_code" : "RM2",
                    "package_desc" : "RAM 2 GB   (Hardware)",
                    "period" : "M",
                    "sub_group" : "Optional",
                    "gm_price" : 960
                },
                {
                    "package_code" : "CP1",
                    "package_desc" : "CPU 1 Vcore    (Hardware)",
                    "period" : "M",
                    "sub_group" : "Optional",
                    "gm_price" : 800
                },
                {
                    "package_code" : "LR6",
                    "package_desc" : "Redhat Linux 6",
                    "period" : "M",
                    "sub_group" : "Optional",
                    "gm_price" : 0
                },
                {
                    "package_code" : "WW8",
                    "package_desc" : "MS Windows Sever 2008 Web Edition",
                    "period" : "M",
                    "sub_group" : "Optional",
                    "gm_price" : 480
                },
                {
                    "package_code" : "WS8",
                    "package_desc" : "MS Windows Server 2008 Standard Edition",
                    "period" : "M",
                    "sub_group" : "Optional",
                    "gm_price" : 800
                },
                {
                    "package_code" : "WE8",
                    "package_desc" : "MS Windows Server 2008 Enterprise Edition",
                    "period" : "M",
                    "sub_group" : "Optional",
                    "gm_price" : 2000
                },
                {
                    "package_code" : "SW8",
                    "package_desc" : "MS SQL Server 2008 R2 Web Edition",
                    "period" : "M",
                    "sub_group" : "Optional",
                    "gm_price" : 800
                },
                {
                    "package_code" : "SS8",
                    "package_desc" : "MS SQL Server 2008 R2 Standard Edition",
                    "period" : "M",
                    "sub_group" : "Optional",
                    "gm_price" : 10000
                },
                {
                    "package_code" : "TFW",
                    "package_desc" : "TrendMicro Firewall + IPS",
                    "period" : "M",
                    "sub_group" : "Optional",
                    "gm_price" : 1600
                },
                {
                    "package_code" : "TAV",
                    "package_desc" : "TrendMicro AntiVirus",
                    "period" : "M",
                    "sub_group" : "Optional",
                    "gm_price" : 480
                },
                {
                    "package_code" : "TFP",
                    "package_desc" : "TrendMicro Firewall + IPS + File Integrity + Log Inspection + Antivirus",
                    "period" : "M",
                    "sub_group" : "Optional",
                    "gm_price" : 3200
                },
                {
                    "package_code" : "TUG",
                    "package_desc" : "TrendMicro Upgrade (from TFW to TFP) for Virtual Server Only",
                    "period" : "M",
                    "sub_group" : "Optional",
                    "gm_price" : 1600
                },
                {
                    "package_code" : "TAV",
                    "package_desc" : "TrendMicro AntiVirus (Bundle with MS Windows; First time Only)",
                    "period" : "M",
                    "sub_group" : "Optional",
                    "gm_price" : 360
                }
            ]
        }
    ],
    "RESULT_STATUS": "000",
    "RESULT_MESSAGE": "Successfull"
}
```



