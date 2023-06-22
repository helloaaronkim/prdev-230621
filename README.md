# prdev-230621


## Information
* API instance id (prod)
  * 18776017
* Org
  * orgid : 5aa6791f-a5c8-4f60-9cac-dd3e396b4bcf
  * org client_id : 43ef998d2d81478ca02b4ad8b9e5f5a3
  * org client_secret : 5B8b70710c15417E8B0936d9B091C734
* ConnectedApps
  * Exchange Viewer
    * client_id : f3e000b78d2b4bf290e60220c18c7ae4
    * client_secret : d77474DFc6A245edA9A910EA4F7D2857
  * Exchange Contributor
    * client_id : b8b02f3795ba4203bcca3ab2a290e6b3
    * client_secret : 70Be7672158847B88e8AdAa4104791FA
  * CloudHub Deployment
    * client_id : a422a6bb3c80476f8695af382b26a816
    * client_secret : 9eC853aC286541b9Ae83E2b8Dd0B207D

## Request list
```
curl -ik -X PUT -H "Content-Type: application/json" -d "{\"lastName\":\"Smith\",\"numBags\":2}" https://localhost:8081/api/v1/tickets/123/checkin

curl -ik -X PUT -H "Content-Type: application/json" -d "{\"lastName\":\"Smith\",\"numBags\":2}" https://check-in-papi-kybfte.5sc6y6-4.usa-e2.cloudhub.io/api/v1/tickets/123/checkin

```

## TBU

```
-M-Danypoint.platform.client_id=43ef998d2d81478ca02b4ad8b9e5f5a3
-M-Danypoint.platform.client_secret=5B8b70710c15417E8B0936d9B091C734

mvn -DmuleDeploy deploy -Dap.client_id=43ef998d2d81478ca02b4ad8b9e5f5a3 -Dap.client_secret=5B8b70710c15417E8B0936d9B091C734 -Dap.ca.client_id=a422a6bb3c80476f8695af382b26a816 -Dap.ca.client_secret=9eC853aC286541b9Ae83E2b8Dd0B207D -Dencrypt.key=secure12345 -Ddeployment.env=dev

mvn -DmuleDeploy deploy -Dap.client_id=43ef998d2d81478ca02b4ad8b9e5f5a3 -Dap.client_secret=5B8b70710c15417E8B0936d9B091C734 -Dap.ca.client_id=a422a6bb3c80476f8695af382b26a816 -Dap.ca.client_secret=9eC853aC286541b9Ae83E2b8Dd0B207D -Dencrypt.key=secure12345 -Ddeployment.env=test

mvn -DmuleDeploy deploy -Dap.client_id=43ef998d2d81478ca02b4ad8b9e5f5a3 -Dap.client_secret=5B8b70710c15417E8B0936d9B091C734 -Dap.ca.client_id=a422a6bb3c80476f8695af382b26a816 -Dap.ca.client_secret=9eC853aC286541b9Ae83E2b8Dd0B207D -Dencrypt.key=secure12345 -Ddeployment.env=prod -Ddeployment.suffix=

```


export M2_HOME="~/Desktop/apache-maven-3.6.3"
PATH="${M2_HOME}/bin:${PATH}"
export PATH

## Host
```
https://check-in-papi-kybfte.5sc6y6-4.usa-e2.cloudhub.io
```