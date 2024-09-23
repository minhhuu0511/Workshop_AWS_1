---
title : "Tạo các kết nối"
date :  "`r Sys.Date()`" 
weight : 4
chapter : false
pre : " <b> 3. </b> "
---

#### Kết nối với EC2 sử dụng MobaXterm 
![SG](/images/3.Connect/039-AccessEC2.png)
+Truy cập và xem Public IP của EC2 vừa tạo:
![SG](/images/3.Connect/040-AccessEC2.png)
+Tạo 1 Session mới
![SG](/images/3.Connect/041-AccessEC2.png)
+ Nhập **Public IP** của EC2 vào **Remote Host**.
+ Specify username: **ec2-user**.
+ Tích vào ô **User private key**. Tìm đường dẫn đến file **key** đã tải xuống.
+ Nhấn **ok**.

![SG](/images/3.Connect/042-AccessEC2.png)
+ Đã kết nối thành công.
![SG](/images/3.Connect/043-InstallEC2.png)
+ Tiến hành cài đặt java cho EC2
+ **sudo yum install java-17-amazon-corretto-headless**.
![SG](/images/3.Connect/044-InstallEC2.png)
+ Nhập **y**.
![SG](/images/3.Connect/045-InstallEC2.png)
+ Kiểm tra phiên bản java
+ **Java -version**

![SG](/images/3.Connect/046-InstallEC2.png)
+ cat /etc/*release.
+ Lệnh để xác định máy ảo linux thuộc phiên bản nào.
![SG](/images/3.Connect/078-Connect.png)

+ ở phiên bản này sử dụng các câu lệnh sau:
+ Trước tiên, cập nhật danh sách các gói để đảm bảo bạn có phiên bản mới nhất:
+ **sudo yum update -y**.
![SG](/images/3.Connect/047-InstallEC2.png)
+ sudo yum install git -y
![SG](/images/3.Connect/048-InstallEC2.png)
+ Kiểm tra cài đặt git
+ **git --version**

![SG](/images/3.Connect/049-InstallEC2.png)
+ Clone project
+ git clone **https://github.com/minhhuu0511/spring-ec2.git**

![SG](/images/3.Connect/050-InstallEC2.png)
+ Cài Maven
+ **sudo yum install maven -y**

![SG](/images/3.Connect/051-InstallEC2.png)
+ Sau đó, kiểm tra Maven:
+ **mvn -version**

![SG](/images/3.Connect/052-InstallEC2.png)
+ Tìm kiếm vị trí project
![SG](/images/3.Connect/053-InstallEC2.png)
+ Đi đến nơi chứa project bằng câu lệnh
+ **cd /home/ec2-user/spring-ec2**

![SG](/images/3.Connect/054-InstallEC2.png)
+ lỗi do phiên bản maven không đáp ứng yêu cầu.
+ Tải phiên bản mới hơn.
![SG](/images/3.Connect/055-InstallEC2.png)
+ **wget https://downloads.apache.org/maven/maven-3/3.9.9/binaries/apache-maven-3.9.9-bin.tar.gz**
![SG](/images/3.Connect/056-InstallEC2.png)
+ Giải nén tệp tải về và di chuyển thư mục đến vị trí phù hợp:
+ tar -xzf apache-maven-3.9.9-bin.tar.gz
+ sudo mv apache-maven-3.9.9 /usr/local/maven
![SG](/images/3.Connect/057-InstallEC2.png)
+ Thêm Maven vào biến môi trường PATH để dễ dàng truy cập:
+ echo 'export M2_HOME=/usr/local/maven' >> ~/.bash_profile
+ echo 'export PATH=$M2_HOME/bin:$PATH' >> ~/.bash_profile
+ source ~/.bash_profile

![SG](/images/3.Connect/058-InstallEC2.png)
+ Mvn clean install để tạo file jar

![SG](/images/3.Connect/059-InstallEC2.png)
+ File jar tạo thành công trong thư mục.
+ Di chuyển đến thư mục chứa file jar
+ cd /home/ec2-user/spring-ec2/target/

![SG](/images/3.Connect/060-InstallEC2.png)

+ Chạy file jar
+ Java -jar employeemanagmentbackend-0.0.1-SNAPSHOT.jar
![SG](/images/3.Connect/061-TestAPI.png)
![SG](/images/3.Connect/062-TestAPI.png)
![SG](/images/3.Connect/063-TestAPI.png)
![SG](/images/3.Connect/064-TestAPI.png)
![SG](/images/3.Connect/065-TestAPI.png)
+ Dùng postman để test các API, **Public IP:8080/employee**