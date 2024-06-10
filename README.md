# NetworkAnalysis-webshell
The SOC received an alert in their SIEM for ‘Local to Local Port Scanning’ where an internal private IP began scanning another internal system.

 1. What is the IP responsible for conducting the port scan activity?
 * Open pcap file in wireshark
 * go to statistics > conversation then choose tcp, we can see the attacker ip address in adress A column

   ![image](https://github.com/George-1100/NetworkAnalysis-webshell/assets/76154087/0be022ca-b9ce-4c96-8d5c-0e6ea75fbd84)

   ANS: 10.251.96.4

   2. What is the port range scanned by the suspicious host?
      * check port b colum first to last port number for port Range

    ![image](https://github.com/George-1100/NetworkAnalysis-webshell/assets/76154087/7afc2552-c797-4ce7-8628-06fa0b3c8f93)

      ANS: 1-1024

 3.  What is the type of port scan conducted?
   Go to display filter search for ip.addr == 10.251.96.4
   ![image](https://github.com/George-1100/NetworkAnalysis-webshell/assets/76154087/75830d93-fb84-4f2b-a33b-85ec20a5ce99)


     ANS : TCP SYN

4. Two more tools were used to perform reconnaissance against open ports, what were they?
   
   ![image](https://github.com/George-1100/NetworkAnalysis-webshell/assets/76154087/b2a29953-af4d-411e-bb1d-89730fbe66a9)

   ![image](https://github.com/George-1100/NetworkAnalysis-webshell/assets/76154087/833e77ff-f7e1-4b32-8cce-06eb6844ba9e)

      ANS: gobuster 3.0.1, sqlmap 1.4.7

   5. What is the name of the php file through which the attacker uploaded a web shell? 

      ![image](https://github.com/George-1100/NetworkAnalysis-webshell/assets/76154087/699b587d-91ec-4838-8a1e-37f1b804abe9)

      ANS: editprofile.php

   6. What is the name of the web shell that the attacker uploaded?

      ![image](https://github.com/George-1100/NetworkAnalysis-webshell/assets/76154087/c05f9a9b-d5c9-43ae-8c34-1ea924aae0b5)

      ANS : dbfunctions.php

   7. What is the parameter used in the web shell for executing commands?

     ![image](https://github.com/George-1100/NetworkAnalysis-webshell/assets/76154087/15fbbaf3-6382-4e5e-b2a1-f23d9073daaf)

      ANS : cmd

   8. What is the first command executed by the attacker?

      ![image](https://github.com/George-1100/NetworkAnalysis-webshell/assets/76154087/c4a889f9-a241-4545-9dea-fe22a3358b22)

   ANS: id

9. What is the type of shell connection the attacker obtains through command execution?

   ![image](https://github.com/George-1100/NetworkAnalysis-webshell/assets/76154087/71c415b6-08e7-492a-bcd8-a4707c65edd3)
 
 ANS : reverse

 10. What is the port he uses for the shell connection?

     ![image](https://github.com/George-1100/NetworkAnalysis-webshell/assets/76154087/a5be78cf-cbcb-4580-a56f-a967ef806078)

Ans : 4422





  

        
      
