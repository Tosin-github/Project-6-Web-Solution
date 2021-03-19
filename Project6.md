
## Web Solution With WordPress


Disk: This is basically creating one or more region storage so that each region can operate separately.
Partition: This is typically created so that a user can have a different operating system on the same hard disk
Volume: The three ways dimension space. 
Storage infrastructure: This indicates the process from the data storage tier to the application phase  and proceeds to the presentation tier
In this project, I have more understanding of different disk management in Linx and working with several storage package management, especially in Redhat. 

Working in a Redhat environment compare to ubuntu I learnt so much, the package management is different.

<img width="579" alt="1" src="https://user-images.githubusercontent.com/79447751/111813750-82dd0f80-88d1-11eb-825e-7e7e50e87fcf.PNG">

<img width="486" alt="2" src="https://user-images.githubusercontent.com/79447751/111814168-11519100-88d2-11eb-9aed-1d1ac405b5c0.PNG">

<img width="483" alt="3" src="https://user-images.githubusercontent.com/79447751/111815179-46aaae80-88d3-11eb-8336-a9748b71408e.PNG">

Partition table scan:
  MBR: not present
  BSD: not present
  APM: not present
  GPT: not present

Creating new GPT entries.

Command (? for help): Type (n) Is to show me a number.
Partition number (1-128, default 1): 1
First sector (34-20971486, default = 2048) or {+-}size{KMGTP}:
Last sector (2048-20971486, default = 20971486) or {+-}size{KMGTP}:
The current type is 'Linux filesystem'
Hex code or GUID (L to show codes, Enter = 8300): Type (8e00)
Changed type of partition to 'Linux LVM'

Command (? for help): Type (p)It gave me access to check my work
Disk /dev/xvdf: 20971520 sectors, 10.0 GiB
Sector size (logical/physical): 512/512 bytes
Disk identifier (GUID): C31CE27D-0BBE-4ADB-9B02-4BC61BB7B26A
Partition table holds up to 128 entries
Main partition table begins at sector 2 and ends at sector 33
First usable sector is 34, last usable sector is 20971486
Partitions will be aligned on 2048-sector boundaries
Total free space is 2014 sectors (1007.0 KiB)

Number  Start (sector)    End (sector)  Size       Code  Name
   1            2048        20971486   10.0 GiB    8E00  Linux LVM

Command (? for help): Type (w) This indicates access to write
Final checks complete. About to write GPT data. THIS WILL OVERWRITE EXISTING
PARTITIONS!!

Do you want to proceed? (Y/N):  Type (yes)
OK; writing new GUID partition table (GPT) to /dev/xvdf.
The operation has completed successfully.
[ec2-user@ip-172-31-31-56 ~]$
[ec2-user@ip-172-31-31-56 ~]$
[ec2-user@ip-172-31-31-56 ~]$ sudo gdisk /dev/xvdg
GPT fdisk (gdisk) version 1.0.3

<img width="483" alt="3" src="https://user-images.githubusercontent.com/79447751/111833174-b9bf1f80-88e9-11eb-810b-9a6ae4818640.PNG">
<img width="451" alt="4" src="https://user-images.githubusercontent.com/79447751/111833196-c04d9700-88e9-11eb-9928-acb8831acbca.PNG">
<img width="491" alt="5" src="https://user-images.githubusercontent.com/79447751/111833208-c6dc0e80-88e9-11eb-9e21-ad40f3e4baa7.PNG">
<img width="451" alt="6" src="https://user-images.githubusercontent.com/79447751/111833380-00ad1500-88ea-11eb-9e62-345cf1459396.PNG">
<img width="473" alt="7" src="https://user-images.githubusercontent.com/79447751/111833413-0a367d00-88ea-11eb-828e-ae64415832c7.PNG">
<img width="441" alt="8" src="https://user-images.githubusercontent.com/79447751/111833429-0efb3100-88ea-11eb-8b65-1e6cd126283d.PNG">
<img width="468" alt="9" src="https://user-images.githubusercontent.com/79447751/111833569-44078380-88ea-11eb-9e5d-ed1abefe2b4b.PNG">
<img width="506" alt="10" src="https://user-images.githubusercontent.com/79447751/111833582-49fd6480-88ea-11eb-9923-e4e6c21a7926.PNG">
<img width="530" alt="11" src="https://user-images.githubusercontent.com/79447751/111833685-6d281400-88ea-11eb-9132-2e21e75c1135.PNG">
<img width="463" alt="12" src="https://user-images.githubusercontent.com/79447751/111833694-6f8a6e00-88ea-11eb-8084-d859a8d935fa.PNG">
<img width="493" alt="13" src="https://user-images.githubusercontent.com/79447751/111833699-71ecc800-88ea-11eb-8c90-0c06a817b302.PNG">
<img width="493" alt="13" src="https://user-images.githubusercontent.com/79447751/111833699-71ecc800-88ea-11eb-8c90-0c06a817b302.PNG">
<img width="493" alt="15" src="https://user-images.githubusercontent.com/79447751/111833717-774a1280-88ea-11eb-9f1e-61161ed4f9c4.PNG">
<img width="461" alt="16" src="https://user-images.githubusercontent.com/79447751/111833726-7add9980-88ea-11eb-80a2-335dc5ad6c5d.PNG">
<img width="472" alt="17" src="https://user-images.githubusercontent.com/79447751/111833739-7fa24d80-88ea-11eb-9522-274911a8cc02.PNG">
<img width="483" alt="19" src="https://user-images.githubusercontent.com/79447751/111833755-85982e80-88ea-11eb-87b1-da2ec7a547b8.PNG">
<img width="465" alt="20" src="https://user-images.githubusercontent.com/79447751/111833760-88931f00-88ea-11eb-87ab-d6434e4671a3.PNG">
<img width="489" alt="21" src="https://user-images.githubusercontent.com/79447751/111834317-546c2e00-88eb-11eb-983b-0b8572bcf43d.PNG">
<img width="494" alt="22" src="https://user-images.githubusercontent.com/79447751/111834323-5635f180-88eb-11eb-95e3-20a593e1db96.PNG">
<img width="484" alt="24" src="https://user-images.githubusercontent.com/79447751/111834328-5930e200-88eb-11eb-91cb-36acf1be1541.PNG">
<img width="521" alt="25" src="https://user-images.githubusercontent.com/79447751/111834335-5c2bd280-88eb-11eb-8416-74cae47dc5f4.PNG">
<img width="486" alt="26" src="https://user-images.githubusercontent.com/79447751/111834338-5df59600-88eb-11eb-93fa-6a59b00bd8ad.PNG">
<img width="500" alt="27" src="https://user-images.githubusercontent.com/79447751/111834342-6057f000-88eb-11eb-9e59-ded3638d3482.PNG">
<img width="516" alt="28" src="https://user-images.githubusercontent.com/79447751/111834352-6221b380-88eb-11eb-93b7-9c68ddea2edf.PNG">
<img width="507" alt="29" src="https://user-images.githubusercontent.com/79447751/111834355-64840d80-88eb-11eb-95f9-708e2c4b79db.PNG">
<img width="441" alt="30" src="https://user-images.githubusercontent.com/79447751/111834356-664dd100-88eb-11eb-9761-402c0aa6494d.PNG">
<img width="524" alt="31" src="https://user-images.githubusercontent.com/79447751/111834391-749bed00-88eb-11eb-8c59-4ee71c5b104c.PNG">
<img width="491" alt="32" src="https://user-images.githubusercontent.com/79447751/111834399-76fe4700-88eb-11eb-9bd5-46771e8ef543.PNG">
<img width="456" alt="33" src="https://user-images.githubusercontent.com/79447751/111834406-7960a100-88eb-11eb-90b6-1a6fe407a696.PNG">
<img width="424" alt="34" src="https://user-images.githubusercontent.com/79447751/111834410-7b2a6480-88eb-11eb-97a5-ba698f2c0763.PNG">
<img width="402" alt="35" src="https://user-images.githubusercontent.com/79447751/111834416-7cf42800-88eb-11eb-81b8-d87de981160b.PNG">
<img width="421" alt="36" src="https://user-images.githubusercontent.com/79447751/111834426-7ebdeb80-88eb-11eb-9ba8-b286c8d5d590.PNG">
<img width="513" alt="37" src="https://user-images.githubusercontent.com/79447751/111834429-81204580-88eb-11eb-97c1-aef0bc38c1f8.PNG">






