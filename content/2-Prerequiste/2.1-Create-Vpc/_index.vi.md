---
title : "Tạo VPC "
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 2.1 </b> "
---


#### Tạo VPC **Lab VPC**

Truy cập giao diện quản trị dịch vụ VPC:
![VPC](/images/2.prerequisite/001-CreateVPC.png)
+ Tìm kiếm **VPC**
![VPC](/images/2.prerequisite/002-CreateVPC.png)
+ Click **Your VPC**.
+ Click **Create VPC**.
![VPC](/images/2.prerequisite/003-CreateVPC.png)
+ Click **VPC and more**.
+ Nhập **VPC Main** vào **Auto-generated**.
+ IPv4 CIDR block nhập **10.0.0.0/16**.
+ IPv6 CIDR block chọn **No IPv6 CIDR block**.
+ Tenancy chọn **Default**.

![VPC](/images/2.prerequisite/004-CreateVPC.png)
+ Number of Availability Zones Chọn **2**.
+ Number of Public và Number of Private chọn **2**.
![VPC](/images/2.prerequisite/005-CreateVPC.png)
+ NAT gateways Chọn **None**.
+ VPC endpoints chọn **S3 Gateway**.
+ Chọn 2 mục trong DNS options 


