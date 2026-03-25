# CiscoBIB
BIB,CiscoBIB,Cisco call manager,cucm, call manager,cisco,collaboration,CiscoBIB Uses Built-In-Bridge (BIB) of Cisco IP phone.

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

Cisco BiB(Built in Bridge) Recording Configuration:

Device > Device Settings > SIP Profile > Add New
 - Name = SIP Profile for BIB Recording
 Section : SIP OPTIONS Ping
 - Enable OPTIONS Ping to monitor destination status for Trunks with Service Type "None (Default)" = Checked
 - Ping Interval for In-service and Partially In-service Trunks (seconds) = 60
Save


Device > Trunk > Add New > Trunk Type = SIP Trunk > Next
 - Device Name = SIP-Trunk-To-Recording-Server
 - Device Pool
 - PSTN Access = Unchecked
 - SIP Trunk Security Profile
 - SIP Profile = SIP Profile for BIB Recording
Save


Call Routing > Route/Hunt > Route Group > Add New
 - Route Group Name = RG_Recording
 - Select "SIP-Trunk-To-Recording-Server", then click "Add to Route Group" button
Save

Call Routing > Route/Hunt > Route List > Add New
 - Name = RL_Recording
 - CUCM Group
Save
Click "Add Route Group" button
 - Route Group = "RG_Recording"
Save

Call Routing > Route/Hunt > Route Pattern > Add New
 - Route Pattern
 - Route Partition
 - Gateway/Route List = RL_Recording
 - Call Classification = OnNet
 - Provide Outside Dial Tone = unchecked
Save

Device > Device Settings > Recording Profile > Add New
 - Name
 - Recording Calling Search Space
 - Recording Destination Address
Save

Phone
 - Built In Bridge = On
DN
 - Recording Option = Automatic Call Recording Enabled
 - Recording Profile = Recording_Profile


# 😄我们坚信：软件只有被用起来，才能给用户带去价值，才能让自身产生迭代！
