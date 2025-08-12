---
title: "Phần 2: Glue + Athena"
weight: 20
---

## Phần 2: AWS Glue và Amazon Athena 🚀

Chào mừng bạn đến với phần thứ hai của workshop! Đây là giai đoạn cốt lõi của giải pháp phân tích dữ liệu, nơi chúng ta sẽ biến dữ liệu thô đã được **thu thập trên Amazon S3** thành một nguồn dữ liệu có cấu trúc, sẵn sàng cho việc phân tích và trực quan hóa.

Trong mô hình kiến trúc của chúng ta, **Amazon S3** là nơi lưu trữ dữ liệu thô, **AWS Glue** đóng vai trò là "bộ não" xử lý dữ liệu để tạo ra metadata, còn **Amazon Athena** là "công cụ" giúp chúng ta truy vấn và khám phá dữ liệu đó một cách dễ dàng bằng các câu lệnh **SQL** chuẩn.

Điểm mạnh của giải pháp này là mô hình **Serverless**, giúp bạn:
* **Tiết kiệm chi phí**: Bạn chỉ phải trả tiền cho dung lượng lưu trữ trên S3 và lượng dữ liệu mà bạn truy vấn bằng Athena.
* **Dễ dàng mở rộng**: Hệ thống có thể xử lý lượng dữ liệu từ vài GB đến hàng PB mà không cần bạn phải quản lý server.
* **Tích hợp liền mạch**: Các dịch vụ AWS được thiết kế để hoạt động cùng nhau một cách hiệu quả, giúp pipeline dữ liệu của bạn chạy trơn tru.

Kết thúc phần này, bạn sẽ nắm được cách:
1.  **Sử dụng AWS Glue Crawler**: Để tự động khám phá và tạo ra metadata (schema) cho dữ liệu.
2.  **Tích hợp với Amazon Athena**: Để truy vấn dữ liệu trực tiếp trên S3 mà không cần phải di chuyển hoặc tải dữ liệu lên.

Hãy bắt đầu khám phá cách xây dựng pipeline dữ liệu này!