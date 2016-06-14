# SampleWebService
=================================================================================================

This web Service Support 2 Method Types : GET and POST.

POST for LOGIN or for Signing IN.

The webservice is connected with MySQL DB. where the username and password are saved.


POST API : http://jmeertes.cloudapp.net:8080/LoginWebService/REST/WebService/login?username=ashu&password=ashu

GET API : http://jmeertes.cloudapp.net:8080/LoginWebService/REST/WebService/logout

========================================================================================================


POST Load Test:

  Simulated with 100 Threads/Second:
    
    Response time : < 1 Second
    
    On Increasing more users : response time becomes >1 sec and Server avaiability is less than 100%
    
    Graph is attached: POST REQUEST_Load Response.
    
    
