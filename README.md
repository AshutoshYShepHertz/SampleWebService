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
    
    
    NOTE: Hitting the APIS with Timer is not affecting it much 
          Database is behaving properly and is able to handle the load.No Delay coming from db side.
          
    
    Detailed Analysis:
        Transactions:                     806 hits
        Availability:                 100.00 %
        Elapsed time:                   5.29 secs
        Data transferred:               0.04 MB
        Response time:                  0.89 secs
        Transaction rate:             152.36 trans/sec
        Throughput:                     0.01 MB/sec
        Concurrency:                   19.72
        Successful transactions:         807
        Failed transactions:               0
        Longest transaction:            0.65
        Shortest transaction:           0.00

    
  GET Load Test:

  Simulated with 100 Threads/Second:
    
    Response time : < 1 Second
    
    On Increasing more users : response time becomes >1 sec and Server avaiability is less than 100%
    
    Graph is attached: GET REQUEST_Load Response.
    
    Detailed Analysis:
      Transactions:                    2537 hits
      Availability:                 100.00 %
      Elapsed time:                   5.07 secs
      Data transferred:               0.12 MB
      Response time:                  0.72 secs
      Transaction rate:             500.39 trans/sec
      Throughput:                     0.02 MB/sec
      Concurrency:                  161.80
      Successful transactions:        2540
      Failed transactions:               0
      Longest transaction:            1.73
      Shortest transaction:           0.00
    
