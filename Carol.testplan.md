### Test Plan

----

#### Target application

[OpenVPN Connect – Fast & Safe SSL VPN Client](https://play.google.com/store/apps/details?id=net.openvpn.openvpn&hl=zh_TW)

#### Objectives

Test the basic function. After pass all test cases, the basic function in this APP could be deliverable.

#### History

| Version | Date       | Author      | Description of Change |
| ------- | ---------- | ----------- | --------------------- |
| 1       | 2018/06/10 | Chia-Yu Hsu | Draft                 |
|         |            |             |                       |



#### Scope

Unit Test

####  



#### Environment

----

##### Device

Andrioid 4.3 Nexus 7 (at least)

##### Roles

* The user with free trail version
* The user with premium version

##### Other requirements 

* Accounts for OpenVPN

* VPN server

  

#### Test Features

----



1. Private Tunnel

​	(1.1) Log in 

​		(1.1.a) Connect 

​		(1.1.b) Disconnect 

​		(1.1.c) Choose VPN Gateway

​		(1.1.d) Setting-VPN-protocal

​		(1.1.e) Setting-VPN-timeout 

​		(1.1.f) Log file 

​		(1.1.g) Log out 

​	(1.2) Register 

​	(1.3) Forget password 

2. Access Server 

​	(2.1) Add server 

​		(2.1.a) Connect 

​		(2.1.b) Disconnect

​	(2.2) Deploy Access Server

3. OVPN Profile 

​	(3.1) Import files



#### Test cases

---



 ##### 1. Private Tunnel    

| ID    | Priority | Severity | Steps                                                        | Expected Results                                             |
| ----- | -------- | -------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 1.1   | High     | Critical | 1. open app <br />2. press private tunnel button <br />3. key in email <br />4. key in password  <br />5. press login button | 1. show three buttons <br />2. show login form <br />5. login successfully, and show email in left sidebar |
| 1.1.a | High     | Critical | 1. press VPN Gateway button<br />2. select a region(US only) from dropdown list<br />3. open a website which is US -only | 1. show dropdown lists<br /><br />2. show connected in app<br />3. connect the website successfully |
| 1.1.b | High     | High     | 1. press on switch in the private tunnel view<br /><br />2. press Yes<br />3. open a website which is US -only | 1. show a dialog "Do you wish to disconnect from Seattle WA?"<br />2. show disconnected status<br />3. fail to connect the website successfully |
| 1.1.c | Medium   | Medium   | 1. press VPN Gateway button<br />                            | 1. show dropdown lists<br /><br />                           |
| 1.1.d | Medium   | Medium   | 1. open setting view<br />2. change the VPN Protocol to "xxxx"<br />( should test all protocals provided, but how to measure it)<br />3. press disconnect<br />4. press connect | 1. show setting panel<br /><br />4. connect successfully<br /><br /> |
| 1.1.e | Low      | Low      | 1. open setting view<br />2. change the Connection timeout to "xxxx"<br />( should test all )<br />3. press disconnect<br />4. press connect | 3. disconnect <br />4. reconnect                             |
| 1.1.f | Low      | Low      | 1. open log file view                                        | 1. show all logs                                             |
| 1.1.g | High     | High     | 1. press logout button                                       | 1. logout successfully, back to main view                    |
| 1.2   | Low      | Low      | 1. press register link                                       | 1. open default browser to login web page("")                |
| 1.3   | Low      | Low      | 1. press forget password link                                | 1. open default browser to forget password web page("")      |



###### 2. Access Server

| ID    | Priority | Severity | Steps                                                        | Expected Results                        |
| ----- | -------- | -------- | ------------------------------------------------------------ | --------------------------------------- |
| 2.1   | High     | Critical | 1. open app <br />2. press Access Server button <br />3. key in host (reference to ...) <br />4. key in password  <br />5. press add server button | 5. successfully add and connect         |
| 2.1.1 | High     | High     | 1. press connect to server                                   | 1. successfully connect                 |
| 2.1.2 | High     | High     | 1. press disconnect to server                                | 1. successfully disconnect              |
| 2.2   | Low      | Low      | 1. press deploy server  link                                 | 1. open default browser to web page("") |





###### 2. OVPN Profile

| ID   | Priority | Severity | Steps                                                        | Expected Results                                             |
| ---- | -------- | -------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 3.1  | Medium   | Medium   | 1. open app <br />2. press OVPN Profile button <br />3. select file location<br />4. press import button | 2. Open files directories view<br />4. Load server setting and connect |



