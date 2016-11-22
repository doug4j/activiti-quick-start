# activiti-quick-start

1. Download Tomcat
1. Download and Install Activiti
1. Verify Environment
```
curl --user kermit:kermit http://localhost:8080/activiti-rest/service/management/engine
```
1. Startup Activiti
1. Design Simple Process
1. Manually Execute
1. Automated Execute
```
curl --user kermit:kermit -H "Content-Type: application/json" -X POST \
-d '{ "processDefinitionKey":"Onboarding", "variables": [ \
{ "name":"fullName", "value": "John Doe" }, \
{ "name":"yearsOfExperience", "value": 2 }\
]}' http://localhost:8080/activiti-rest/service/runtime/process-instances
```
