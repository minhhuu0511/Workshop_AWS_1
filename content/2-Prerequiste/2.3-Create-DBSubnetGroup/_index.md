---
title : "Tạo DBSubnet Group "
date :  "`r Sys.Date()`" 
weight : 3 
chapter : false
pre : " <b> 2.3 </b> "
---


#### Tạo DBSubnet Group **DB-Subnet Group**
Truy cập giao diện quản trị dịch vụ RDS:
![VPC](/images/2.prerequisite/022-CreateRDS.png)

![VPC](/images/2.prerequisite/075-CreateDBSubnetGroup.png)

  + Click **Subnet group**.
  + Click **Create DB Subnet Group**.

![VPC](/images/2.prerequisite/019-CreateDBSubnetGroup.png)
+ Name: nhập **DB-Subnet Group**.
+ Decription nhập **Database**.
+ VPC: Chọn **VPC Main**.
![VPC](/images/2.prerequisite/021-CreateDBSubnetGroup.png)
+ AZ: chọn **us-east-1a**, **us-east-1b**.
+ Subnet chọn 2 Private Subnet.
+ Chọn **Create**.



