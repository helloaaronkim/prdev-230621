# prdev-230621


## Information
* API instance id (prod)
  * 18776017
* Org
  * orgid : 5aa6791f-a5c8-4f60-9cac-dd3e396b4bcf
  * org client_id : 43ef998d2d81478ca02b4ad8b9e5f5a3
  * org client_secret : 5B8b70710c15417E8B0936d9B091C734

## Request list
```
curl -ik -X PUT -H "Content-Type: application/json" -d "{\"lastName\":\"Smith\",\"numBags\":2}" https://localhost:8081/api/v1/tickets/123/checkin
```

## TBU

```
-M-Danypoint.platform.client_id=43ef998d2d81478ca02b4ad8b9e5f5a3
-M-Danypoint.platform.client_secret=5B8b70710c15417E8B0936d9B091C734
```


export M2_HOME="~/Desktop/apache-maven-3.6.3"
PATH="${M2_HOME}/bin:${PATH}"
export PATH