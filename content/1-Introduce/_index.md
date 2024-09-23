---
title : "Giới thiệu"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 1. </b> "
---
**Amazon Elastic Compute Cloud (EC2)** là một dịch vụ đám mây của AWS (Amazon Web Services) cung cấp các máy chủ ảo để chạy các ứng dụng. EC2 cho phép người dùng tạo và quản lý các **phiên bản máy chủ ảo (instance)** với nhiều hệ điều hành khác nhau như Linux và Windows. Dịch vụ này linh hoạt, giúp người dùng dễ dàng mở rộng hoặc thu gọn tài nguyên tính toán theo nhu cầu của ứng dụng.

Với việc sử dụng EC2, bạn sẽ có được những ưu điểm sau:

- **Tính linh hoạt**: Người dùng có thể chọn cấu hình phần cứng, hệ điều hành và mạng của máy chủ theo yêu cầu.
- **Tự động mở rộng**: Dịch vụ hỗ trợ tự động mở rộng (Auto Scaling) dựa trên lưu lượng truy cập hoặc tải của ứng dụng.
- **Bảo mật**: EC2 tích hợp với các dịch vụ bảo mật khác của AWS như IAM (Identity and Access Management), cho phép kiểm soát chi tiết quyền truy cập vào các phiên bản.
- **Tính khả dụng cao**: AWS cung cấp các tùy chọn để triển khai trên nhiều vùng (regions) và khu vực sẵn sàng (availability zones), đảm bảo hệ thống luôn hoạt động liên tục.
- **Thanh toán theo sử dụng**: Người dùng chỉ phải trả phí dựa trên tài nguyên mà họ sử dụng, giúp tối ưu hóa chi phí.


**Amazon RDS (Relational Database Service)** là một dịch vụ quản lý cơ sở dữ liệu (CSDL) trên đám mây do AWS cung cấp. RDS giúp dễ dàng thiết lập, vận hành, và mở rộng cơ sở dữ liệu quan hệ một cách tự động, giúp người dùng tập trung vào phát triển ứng dụng mà không phải lo về quản lý hạ tầng. Dịch vụ này hỗ trợ nhiều hệ quản trị cơ sở dữ liệu khác nhau.

Với việc sử dụng **RDS**, bạn sẽ có được những ưu điểm sau:

- **Quản lý tự động**: RDS tự động quản lý các tác vụ như sao lưu, vá lỗi, cập nhật phần mềm và sao chép dữ liệu. Điều này giúp giảm công việc quản lý thủ công cho người dùng.
- **Tính mở rộng**: Người dùng có thể dễ dàng mở rộng hoặc thu hẹp tài nguyên cơ sở dữ liệu theo nhu cầu, từ việc điều chỉnh kích thước ổ đĩa đến tăng giảm số lượng phiên bản (instance) cơ sở dữ liệu.
- **Sao lưu và khôi phục**: RDS hỗ trợ tính năng tự động sao lưu hàng ngày và tạo các điểm khôi phục (snapshot) để đảm bảo dữ liệu luôn được an toàn và có thể phục hồi khi cần thiết.
- **Bảo mật tích hợp**: RDS hỗ trợ mã hóa dữ liệu cả khi lưu trữ và truyền tải, đồng thời tích hợp với các dịch vụ bảo mật của AWS như IAM và VPC để kiểm soát truy cập và bảo vệ dữ liệu.
- **Hiệu suất cao**: Amazon RDS được tối ưu hóa để cung cấp hiệu suất ổn định với độ trễ thấp. Amazon Aurora, một cơ sở dữ liệu tương thích với MySQL và PostgreSQL, cung cấp hiệu năng cao hơn nhiều so với cơ sở dữ liệu MySQL thông thường.
- **Hỗ trợ tính khả dụng cao**: Với RDS Multi-AZ (Multi-Availability Zone), dữ liệu được sao chép tự động giữa các khu vực sẵn sàng khác nhau, đảm bảo rằng cơ sở dữ liệu luôn sẵn sàng trong trường hợp có sự cố.

+ Ở bài thực hành này chúng ta sẽ chạy 1 ứng dụng CRUD đơn giản lên máy ảo EC2 và RDS để làm quen với 2 dịch vụ này.
