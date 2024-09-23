---
title : "Tạo các security group"
date :  "`r Sys.Date()`" 
weight : 2
chapter : false
pre : " <b> 2.2 </b> "
---

#### Tạo các security group



Truy cập giao diện quản trị dịch vụ VPC
![SG](/images/2.prerequisite/074-CreateSG.png)   
  + Click **Security Group**.  
  + Click **Create security group**.

![SG](/images/2.prerequisite/006-CreateSG.png)
+ Security group name: Nhập **Web Server-SG**
+ Description: Nhập **Allow SSH for servers in public subnet.**
+ VPC chọn **VPC Main**
![SG](/images/2.prerequisite/007-CreateSG.png)
+ **Inbound** Thêm các rule sau: SSH, HTTP, HTTPS, Custom TCP với Source **AnyWhere**
![SG](/images/2.prerequisite/008-CreateSG.png)
+ **Outbound** rule giữ nguyên
![SG](/images/2.prerequisite/009-CreateSG.png)
+ Tiếp tục tạo Sercurity Group cho RDS
+ Security group name: Nhập **RDS-SG**
+ Description: Nhập **Only access by EC2 Instances**
+ VPC: Chọn VPC Main
![SG](/images/2.prerequisite/010-CreateSG.png)
+ **Inbound** Thêm rule MySQL/Aurora. Source **AnyWhere**

![SG](/images/2.prerequisite/012-CreateSG.png)

+ **Outbound** rule giữ nguyên



