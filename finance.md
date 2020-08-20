## 修改的api

**API: /payment/v2/project/get/finance	GET**

reuqest: no change

response:
``` json
{
  "data": {
    "rowProjects": [
      {
        "id": "string",
        "paymentJobDTOList": [
          {
            "currentTlEmail": "string",
            "currentTlId": "string",
            "id": "string",
            "jobActiveStatus": "string",
            "jobContactEmail": "string",
            "jobCreatedTime": "2020-08-20T03:24:51.617Z",
            "jobCreatorId": "string",
            "jobId": "string",
            "jobName": "string",
            "jobPaymentStatus": "NEW",
            "jobPaymentType": "BY_COUNT",
            "jobRowFlag": true,
            "jobStatus": "string",
            "jobTenantType": "string",
            "jobType": "string",
            "jobVersion": "string",
            "lastOperationTime": "2020-08-20T03:24:51.618Z",
            "paymentPeriodId": "string",
            "paymentPeriodOrder": 0,
            "paymentPeriodYear": 0,
            "projectId": "string",
            "projectName": "string",
            "submitterEmail": "string",
            "totalAmount": 0,
            "totalApprovedAmount": 0,
            "version": 0
          }
        ],
        "projectActiveStatus": "string",
        "projectCreatedTime": "2020-08-20T03:24:51.618Z",
        "projectId": "string",
        "projectName": "string",
        "projectOwnerId": "string",
        "projectWorkdayId": "string",
        "version": 0
      }
    ],
    "totalCount": 0,
    "weChatProjects": [
      {
        "id": "string",
        "paymentJobDTOList": [
          {
            "currentTlEmail": "string",
            "currentTlId": "string",
            "id": "string",
            "jobActiveStatus": "string",
            "jobContactEmail": "string",
            "jobCreatedTime": "2020-08-20T03:24:51.618Z",
            "jobCreatorId": "string",
            "jobId": "string",
            "jobName": "string",
            "jobPaymentStatus": "NEW",
            "jobPaymentType": "BY_COUNT",
            "jobRowFlag": true,
            "jobStatus": "string",
            "jobTenantType": "string",
            "jobType": "string",
            "jobVersion": "string",
            "lastOperationTime": "2020-08-20T03:24:51.618Z",
            "paymentPeriodId": "string",
            "paymentPeriodOrder": 0,
            "paymentPeriodYear": 0,
            "projectId": "string",
            "projectName": "string",
            "submitterEmail": "string",
            "totalAmount": 0,
            "totalApprovedAmount": 0,
            "version": 0
          }
        ],
        "projectActiveStatus": "string",
        "projectCreatedTime": "2020-08-20T03:24:51.618Z",
        "projectId": "string",
        "projectName": "string",
        "projectOwnerId": "string",
        "projectWorkdayId": "string",
        "version": 0
      }
    ]
  },
  "message": "string",
  "status": 0,
  "time": "2020-08-20T03:24:51.618Z",
  "traceId": "string"
}
```

**API: /payment/v2/project/get/finance/all	GET**

reuqest: no change

response:
``` json
{
  "data": {
    "rowProjects": [
      {
        "id": "string",
        "paymentJobDTOList": [
          {
            "currentTlEmail": "string",
            "currentTlId": "string",
            "id": "string",
            "jobActiveStatus": "string",
            "jobContactEmail": "string",
            "jobCreatedTime": "2020-08-20T03:24:51.617Z",
            "jobCreatorId": "string",
            "jobId": "string",
            "jobName": "string",
            "jobPaymentStatus": "NEW",
            "jobPaymentType": "BY_COUNT",
            "jobRowFlag": true,
            "jobStatus": "string",
            "jobTenantType": "string",
            "jobType": "string",
            "jobVersion": "string",
            "lastOperationTime": "2020-08-20T03:24:51.618Z",
            "paymentPeriodId": "string",
            "paymentPeriodOrder": 0,
            "paymentPeriodYear": 0,
            "projectId": "string",
            "projectName": "string",
            "submitterEmail": "string",
            "totalAmount": 0,
            "totalApprovedAmount": 0,
            "version": 0
          }
        ],
        "projectActiveStatus": "string",
        "projectCreatedTime": "2020-08-20T03:24:51.618Z",
        "projectId": "string",
        "projectName": "string",
        "projectOwnerId": "string",
        "projectWorkdayId": "string",
        "version": 0
      }
    ],
    "totalCount": 0,
    "weChatProjects": [
      {
        "id": "string",
        "paymentJobDTOList": [
          {
            "currentTlEmail": "string",
            "currentTlId": "string",
            "id": "string",
            "jobActiveStatus": "string",
            "jobContactEmail": "string",
            "jobCreatedTime": "2020-08-20T03:24:51.618Z",
            "jobCreatorId": "string",
            "jobId": "string",
            "jobName": "string",
            "jobPaymentStatus": "NEW",
            "jobPaymentType": "BY_COUNT",
            "jobRowFlag": true,
            "jobStatus": "string",
            "jobTenantType": "string",
            "jobType": "string",
            "jobVersion": "string",
            "lastOperationTime": "2020-08-20T03:24:51.618Z",
            "paymentPeriodId": "string",
            "paymentPeriodOrder": 0,
            "paymentPeriodYear": 0,
            "projectId": "string",
            "projectName": "string",
            "submitterEmail": "string",
            "totalAmount": 0,
            "totalApprovedAmount": 0,
            "version": 0
          }
        ],
        "projectActiveStatus": "string",
        "projectCreatedTime": "2020-08-20T03:24:51.618Z",
        "projectId": "string",
        "projectName": "string",
        "projectOwnerId": "string",
        "projectWorkdayId": "string",
        "version": 0
      }
    ]
  },
  "message": "string",
  "status": 0,
  "time": "2020-08-20T03:24:51.618Z",
  "traceId": "string"
}
```

## 新增的api
**API: /payment/v2/item/finance/approve/batch/check	POST**

request:

* isPublic

* requestVO:

``` json
{
  "isRoW": true,
  "jobIds": [
    "string"
  ],
  "memo": "string",
  "roW": true,
  "seqInYear": 0,
  "year": 0
}
```

response:


``` json
{
  "data": {
    "resultMap": {
      "jobId1": {
        "approvedAmount": 0,
        "approvedCount": 0,
        "rejectedAmount": 0,
        "rejectedCount": 0
      },
      "jobId3": {
        "approvedAmount": 0,
        "approvedCount": 0,
        "rejectedAmount": 0,
        "rejectedCount": 0
      },
      "jobId3": {
        "approvedAmount": 0,
        "approvedCount": 0,
        "rejectedAmount": 0,
        "rejectedCount": 0
      }
    },
    "totalApprovedAmount": 0,  //所有job的approvedAmount总和
    "totalApprovedCount": 0,   //所有job的approvedCount总和
    "totalRejectedAmount": 0,  //同上
    "totalRejectedCount": 0    //同上
  },
  "message": "string",
  "status": 0,
  "time": "2020-08-20T03:42:15.149Z",
  "traceId": "string"
}
```

**API: /payment/v2/item/finance/approve/batch/approve**

request:

* isPublic

* paymentItemApproveVO:

``` json
{
  "isRoW": true,
  "jobIds": [
    "string"
  ],
  "memo": "string",
  "roW": true,
  "seqInYear": 0,
  "year": 0
}
```

response:

``` json
{
  "message": "string",
  "status": 0,
  "time": "2020-08-20T03:45:53.060Z",
  "traceId": "string"
}
```
