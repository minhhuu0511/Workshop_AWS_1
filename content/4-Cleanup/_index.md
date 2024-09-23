+++
title = "Dọn dẹp tài nguyên  "
date = 2021
weight = 6
chapter = false
pre = "<b>4. </b>"
+++
# Dọn dẹp các tài nguyên đã sử dụng
Chúng ta sẽ tiến hành các bước sau để xóa các tài nguyên chúng ta đã tạo trong bài thực hành này.


![SG](/images/4.clean/066-Clean.png)
+ RDS: Chọn database  **employeems ** ->  **Action** ->  **delete **.
![SG](/images/4.clean/067-Clean.png)
+ Bỏ tích ở **Create final snapshot** và **retain automated backups**. Tích vào ô **I acknowledge that upon instance deletion, automated backups …..**.
+ Nhập **delete me** vào ô xác nhận và nhấn **Delete**.

![SG](/images/4.clean/068-Clean.png)
+ Dbsubnet group: chọn db-subnet group và chọn **Delete**.
![SG](/images/4.clean/069-Clean.png)
+ Chọn **Delete**.
![SG](/images/4.clean/070-Clean.png)
+ EC2: Chọn **Web Server** ->  **Instance state** ->  **Terminate (delete) instance**.
![SG](/images/4.clean/071-Clean.png)
+ Chọn **Terminate (delete)**.
![SG](/images/4.clean/072-Clean.png)
+ VPC: Chọn **VPC Main** -> **Action** -> **Delete VPC**.