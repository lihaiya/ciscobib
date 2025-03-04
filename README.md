BIB,CiscoBIB,Cisco call manager,cucm, call manager,cisco,collaboration,CiscoBIB Uses Built-In-Bridge (BIB) of Cisco IP phone！思科录音系统！思科电话系统录音！思科CUCM录音！思科BIB录音！

Telephone terminal streaming recording, such as BIB recording supported by Cisco IP phone system:

Since most Cisco IP phones support BIB function, the so-called BIB function is that when Cisco IP phones are on a call, they send their incoming and outgoing traffic to the voice gateway, and then pass it to the PSTN external landline (internal and external call recording) or landline user (internal call recording), while copying their incoming and outgoing traffic to the recording server, thereby realizing call recording.

At this time, the recording software is located in the server that is interconnected with the IP phone network and the CUCM network, and can receive the traffic sent by the IP phone for recording.

## 📫 How to reach us:
Skype：https://join.skype.com/invite/rVbQH1igkQwV

Skype UserID：live:.cid.fedb411de91d9b

Email:leehear@gmail.com

WeChat:David_Li_Haiya

## Blow is the phone model supported Device Matrix
Unified CM Silent Monitoring/Recording Supported Device Matrix:
https://developer.cisco.com/site/uc-manager-sip/documents/supported/

## Configuration steps and screenshots
一，Phone界面配置，在Phone的配置界面，在“Built In Bridge”选择“On”；
二，DN界面配置，在号码界面配置中：
1，在Recording Option，选择“Automatic Call Recording Enabled”；
2，在“Recording Profile”选择，“Recording_Profile”; 
3，在“Recording Media Source”下拉框，选择“Phone Preferred”即可！

![image](https://github.com/user-attachments/assets/d93e9fdd-527a-44e3-b5dd-bc7cddfbe546)
![image](https://github.com/user-attachments/assets/9aba110a-3743-40d9-b61a-eca92c11813a)
![image](https://github.com/user-attachments/assets/4a1cdf08-71ee-43fa-b3dc-aa629d6dab2c)
![image](https://github.com/user-attachments/assets/95482dea-225a-41e7-acc5-c1a3c2846562)
![image](https://github.com/user-attachments/assets/4e95b410-e489-4279-b6ce-78a5f9917526)
![image](https://github.com/user-attachments/assets/f37895ba-443c-4096-b2c2-b2956c1ba53e)

# 😄价值观：我们坚信，软件只有被用起来，才能给用户带去价值，才能让自身产生迭代！！！
