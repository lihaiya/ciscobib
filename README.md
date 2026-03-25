# CiscoBIB
BIB,CiscoBIB,Cisco call manager,cucm, call manager,cisco,collaboration,CiscoBIB Uses Built-In-Bridge (BIB) of Cisco IP phone，思科录音系统，思科电话系统录音，思科CUCM录音，思科BIB录音!!!

Telephone terminal streaming recording, such as BIB recording supported by Cisco IP phone system:

Since most Cisco IP phones support BIB function, the so-called BIB function is that when Cisco IP phones are on a call, they send their incoming and outgoing traffic to the voice gateway, and then pass it to the PSTN external landline (internal and external call recording) or landline user (internal call recording), while copying their incoming and outgoing traffic to the recording server, thereby realizing call recording.

At this time, the recording software is located in the server that is interconnected with the IP phone network and the CUCM network, and can receive the traffic sent by the IP phone for recording.

## - 📫 How to reach us 📫:
- Email:leehear@gmail.com

## Blow is the phone model supported Device Matrix
Unified CM Silent Monitoring/Recording Supported Device Matrix:
https://developer.cisco.com/site/uc-manager-sip/documents/supported/

## Screenshots
<img width="1431" height="564" alt="image" src="https://github.com/user-attachments/assets/f6779e93-0c8f-47b3-8693-2679eb5750b2" />
<img width="1426" height="517" alt="image" src="https://github.com/user-attachments/assets/a2705a6f-1ce8-4fe9-a700-7cc30e953ae8" />
<img width="1432" height="631" alt="image" src="https://github.com/user-attachments/assets/5a74516c-3843-44d2-9ac1-192497538e45" />
<img width="1426" height="568" alt="image" src="https://github.com/user-attachments/assets/0045ef12-8dd1-41e0-be61-1c6f118bdc3f" />
<img width="1413" height="577" alt="image" src="https://github.com/user-attachments/assets/f1f5e273-94ca-4cbc-b7f2-8a8e2e282e25" />
<img width="1423" height="354" alt="image" src="https://github.com/user-attachments/assets/87dad2c1-35c3-4fcd-8b52-ef16f3332d08" />
<img width="1418" height="595" alt="image" src="https://github.com/user-attachments/assets/11785b2f-bfa5-45a2-8391-03cb87d1fb59" />
<img width="1410" height="370" alt="image" src="https://github.com/user-attachments/assets/2db81950-873d-49be-a575-9b04656ed4bb" />

## Configuration steps
一，Phone界面配置，在Phone的配置界面，在“Built In Bridge”选择“On”；
二，DN界面配置，在号码界面配置中：
1，在Recording Option，选择“Automatic Call Recording Enabled”；
2，在“Recording Profile”选择，“Recording_Profile”; 
3，在“Recording Media Source”下拉框，选择“Phone Preferred”即可！



# 😄我们坚信：软件只有被用起来，才能给用户带去价值，才能让自身产生迭代！
