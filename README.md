-Connected all devices on gns3 GUI. 

<img width="675" height="439" alt="image" src="https://github.com/user-attachments/assets/c76ecbea-6853-479d-9b02-5bda7ec56e5a" />

Switch 1

PC1 - 192.168.2.1/27      
PC2 - 192.168.2.2/27

Switch 2

PC3 - 192.168.3.1/27      
PC4 - 192.168.3.2/27


-Configure VPC 1
<VPC 1/>

<img width="322" height="67" alt="VPC1" src="https://github.com/user-attachments/assets/56ee4d1e-1379-42e5-aec9-3020f9130307" />

VPC2

<img width="306" height="64" alt="VPC 2" src="https://github.com/user-attachments/assets/a6d9e08f-f201-4c12-a47e-d578732889ad" />

ping requests from the first switch pcs

<img width="431" height="109" alt="ping PC2 to PC1" src="https://github.com/user-attachments/assets/b4f3055f-6511-4f2b-9584-a0d6e28aefff" />

Configured IPs on PC 3 & 4 on switch 2

PC3> ip 192.168.3.1/27

Checking for duplicate address...

PC1 : 192.168.3.1 255.255.255.224

Successful ping from PC 3 to 4

<img width="441" height="168" alt="image" src="https://github.com/user-attachments/assets/685ce361-f10b-4a05-8065-0789f395088d" />

This explains the partial broken connection. Because of the redundancy aused by the three switches, created a Spanning Tree Protocol(STP)

<img width="675" height="439" alt="image" src="https://github.com/user-attachments/assets/87c7ee83-4fbd-432f-bc02-533559dfb81e" />

PC4> ip 192.168.3.2/27

Checking for duplicate address...

PC1 : 192.168.3.2 255.255.255.224

<img width="436" height="192" alt="image" src="https://github.com/user-attachments/assets/bb7458f7-c2b1-495c-9675-9ad84cb4ccfe" />

ping request from PC2 on switch 1 to PC 3 & 4 on switch 2

<img width="331" height="87" alt="image" src="https://github.com/user-attachments/assets/2dc29235-074a-4972-9d2d-d4f8bca40e58" />

It didn't work since they are not on the same network, for communication to happen between them we would need a router for routing the IP addresses and enable communication. 
ping requests from PC3 to PC1 & PC2

Save configurations on all devices 
PC1
<img width="381" height="63" alt="image" src="https://github.com/user-attachments/assets/6efea966-5f82-4e9f-afe5-fde085990fa3" />

PC2 
<img width="350" height="65" alt="image" src="https://github.com/user-attachments/assets/0cf5574b-5d37-43fa-bb00-b21d26af6803" />

PC3
<img width="436" height="192" alt="image" src="https://github.com/user-attachments/assets/bd16fcc6-166e-47ce-90e5-6371aabcb2dd" />

PC4
<img width="346" height="60" alt="image" src="https://github.com/user-attachments/assets/3709f0e0-e5ef-4fb3-a882-6f1c7981f696" />




