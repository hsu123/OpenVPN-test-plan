 ##### 1. Private Tunnel    
| ID    | Priority | Severity | Steps                                                        | Expected Results                                             |
| ----- | -------- | -------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 1.1   | High     | Critical | 1. open app <br />2. press private tunnel button <br />3. key in email <br />4. key in password  <br />5. press login button | 1. show three buttons <br />2. show login form <br />5. login successfully, and show email in left sidebar |
| 1.1.a | High     | Critical | 1. press VPN Gateway button<br />2. select a region(US only) from dropdown list<br />3. open a website which is US -only | 1. show dropdown lists<br /><br />2. show connected in app<br />3. connect the website successfully |
| 1.1.b | High     | High     | 1. press on switch in the private tunnel view<br /><br />2. press Yes<br />3. open a website which is US -only | 1. show a dialog "Do you wish to disconnect from Seattle WA?"<br />2. show disconnected status<br />3. fail to connect the website successfully |
| 1.1.c | Medium   | Medium   | 1. press VPN Gateway button<br />                            | 1. show dropdown lists<br /><br />                           |
| 1.1.d | Medium   | Medium   | 1. open setting view<br />2. change the VPN Protocol to "xxxx"<br />( should test all protocals provided, but how to measure it)<br />3. press disconnect<br />4. press connect | 1. show setting panel<br /><br />4. connect successfully<br /><br /> |
| 1.1.e | Low      | Low      | 1. open setting view<br />2. change the Connection timeout to "xxxx"<br />( should test all )<br />3. press disconnect<br />4. press connect |                                                              |
| 1.1.f | Low      | Low      | 1. open log file view                                        | 1. show all logs                                             |
| 1.1.g | High     | High     | 1. press logout button                                       | 1. logout successfully, back to main view                    |
| 1.2   | Low      | Low      | 1. press register link                                       | 1. open default browser to login web page("")                |
| 1.3   | Low      | Low      | 1. press forget password link                                | 1. open default browser to forget password web page("")      |



###### 2. Access Server

| ID    | Priority | Severity | Steps                                                        | Expected Results                |
| ----- | -------- | -------- | ------------------------------------------------------------ | ------------------------------- |
| 2.1   | High     | Critical | 1. open app <br />2. press Access Server button <br />3. key in host (reference to ...) <br />4. key in password  <br />5. press add server button | 5. successfully add and connect |
| 2.1.1 | High     | High     | 1. press connect to server                                   | 1. successfully connect         |
| 2.1.2 | High     | High     | 1. press disconnect to server                                | 1. successfully disconnect      |
| 2.2   |          |          |                                                              |                                 |





###### 2. OVPN Profile

| ID   | Priority | Severity | Steps                                                        | Expected Results |
| ---- | -------- | -------- | ------------------------------------------------------------ | ---------------- |
| 3.1  | Medium   | Medium   | 1. open app <br />2. press OVPN Profile button <br />3. select file location<br />4. press import button |                  |