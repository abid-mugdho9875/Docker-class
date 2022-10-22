nslookup
We try to connect with the google.com ip addresss. 
1. - dig google.com

-![image](https://user-images.githubusercontent.com/75389185/197331003-f1121174-d10a-4790-835d-a20f60c2edc8.png)

Here, it gives result which denotes the mapping ip address of googl.com

- ![image](https://user-images.githubusercontent.com/75389185/197331071-854593f1-e950-44e5-8be1-c165cb214847.png)
Here, we see that dns query is udp type request.




2. telnet --> this command used to conect TCP connection with ip address.
It has two part ip address and port number.
![image](https://user-images.githubusercontent.com/75389185/197331243-d703f691-c77a-45f7-ad01-6b3670e45561.png)

- If we see the result we find that after established connection, connection not break as TCP connection oriented protocol.

- Interesting fact that Telnet has internal mechanism to dns query. 

![image](https://user-images.githubusercontent.com/75389185/197331396-2318cadb-cdce-4a0f-8f31-fc5a49802a44.png)

Here, at first DNS query happend. Then TCP conection established. But why connection is closed after some period??
- Here timeout happend. Suppose, google has million and million client. As TCP is connection oriented protocol. It might be overloaded for the server to maintain the connection.So after certain time it is closed their connection.

- Timeout should be slected carefully. Otherwise connection might be failed!!!!
- Redirection done throug browser.

What happens if we use 
`telnet facebook.com 443`

ping ---> ICMP protocol.Packet transfer time find.

One microservices try to connect with another microservice but can not connect , timeout is happend. How can we debug?
- We use telnet to connect ip with fixed port. If we can't connect, we understand that there is problem in network. Otherwise, network is ok. 
Types of timeout- 
1. connection is not established. (network issue)
2. Connection established but it brekas after some time.


 If we build dockerfile it becames docker image. 
 If we push dockerimage to dockerhub. It stills docker image.
 If we run dockerfile it becames container.

