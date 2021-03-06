## Send email to specified workers

**POST project/v2/job/pm/workers/email**

```javascript
request param : 
  String jobId,
  String email,
  List<JobAssignStatus> status,
  boolean isPublic,
  ZonedDateTime applyTimeStart,
  ZonedDateTime lastEmailTimeStart,
  ZonedDateTime applyTimeEnd,
  ZonedDateTime lastEmailTimeEnd,
 
 request body emailVO: 
 {
    Set<String> emailSet,
    String subject,
    String htmlContent,
    String textContent
 }

```

1. send to all of workers

    assign jobId and emailVO(don't assign emailSet)

2. send to workers in some condition

    assign jobId and (status or applyTime or lastEmailTime) and emailVO(don't assign emailSet)

3. send to specified workers
    
    assign jobId and emailVO(with emailSet)

## Search work force

**GET project/v2/job/pm/workers**

Request:
```javascript
request param : 
  String jobId,
  
  boolean isPublic,
  int pageSize,
  int pageIndex,
  
 
 request body condition: 
 {
    List<JobAssignStatus> statusList,
    ZonedDateTime applyTimeStart,
    ZonedDateTime lastEmailTimeStart,
    ZonedDateTime applyTimeEnd,
    ZonedDateTime lastEmailTimeEnd,
    String email
 }

```

Response: 
```javascript
    new field Instant lastEmailTime;
```

