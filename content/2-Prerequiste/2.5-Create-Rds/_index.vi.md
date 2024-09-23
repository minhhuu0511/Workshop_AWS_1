---
title : "Tạo RDS "
date :  "`r Sys.Date()`" 
weight : 5
chapter : false
pre : " <b> 2.5 </b> "
---


#### Tạo VPC **Lab VPC**
 Truy cập giao diện quản trị dịch vụ VPC:
 ![EC2](/images/2.prerequisite/022-CreateRDS.png)
 ![EC2](/images/2.prerequisite/023-CreateRDS.png)
  + Click **Database**.
  + Click **Create Database**.




![EC2](/images/2.prerequisite/024-CreateRDS.png)
+ Click **Standard create**.
![EC2](/images/2.prerequisite/025-CreateRDS.png)
+ Engine type: Click **MySQL**.
![EC2](/images/2.prerequisite/026-CreateRDS.png)

![EC2](/images/2.prerequisite/027-CreateRDS.png)
![EC2](/images/2.prerequisite/028-CreateRDS.png)
+ Template: Free tier
+ DB cluster identifier: Nhập employeeMS
![EC2](/images/2.prerequisite/077-CreateRDS.png)
+ Chọn: **Multi-AZ DB Cluster**.  
![EC2](/images/2.prerequisite/029-CreateRDS.png)
+ Master username: Nhập **Admin**.
+ Credentials management: Chọn **Self managed**
+ Bỏ chọn **Auto generate password**
+ Nhập mật khẩu mong muốn.
![EC2](/images/2.prerequisite/030-CreateRDS.png)
![EC2](/images/2.prerequisite/031-CreateRDS.png)
+ Các nội dung trên giữ nguyên như mặc định.
![EC2](/images/2.prerequisite/032-CreateRDS.png)
+ Chọn **Connect to an EC2 compute resource**.
+ EC2 instance: Chọn **Web Server**. 
![EC2](/images/2.prerequisite/033-CreateRDS.png)
+ DB subnet group: **Choose existing**.
+ Existing DB subnet groups: **db-subnet group**.
![EC2](/images/2.prerequisite/034-CreateRDS.png)
+ VPC security group (firewall): **Choose existing**.
+ Additional VPC security group: **RDS-SG**.
![EC2](/images/2.prerequisite/035-CreateRDS.png)
+ Database authentication options: **Password authentication**.
+ Monitoring: có thể sử dụng hoặc không.
![EC2](/images/2.prerequisite/036-CreateRDS.png)
+ Additional configuration: Initial database name **employeeMS**.
+ **Enable automated backups**.
![EC2](/images/2.prerequisite/037-CreateRDS.png)
+ **Create Database**.

