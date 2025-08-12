---
title: "Giới thiệu Workshop"
weight: 2
---

## Giới thiệu Workshop

### Tóm tắt Dự án

Dự án này nhằm xây dựng một hệ thống phân tích dữ liệu hiện đại, trực quan và dễ tích hợp trên nền tảng AWS để giải quyết bài toán phân tích và trực quan hóa dữ liệu bán hàng, hành vi khách hàng. Giải pháp này sử dụng Amazon QuickSight làm công cụ chính để xây dựng dashboard, với dữ liệu được thu thập từ Amazon S3, xử lý bằng AWS Glue và truy vấn bằng Athena. Dashboard sau đó sẽ được nhúng vào hệ thống CRM nội bộ qua iframe, có hỗ trợ phân quyền người dùng (Row-Level Security).

### Lợi Ích Chính của Giải Pháp

* **Tăng Hiệu Quả**: Giảm thời gian tạo báo cáo từ **2-3 ngày** xuống dưới **15 phút**.
* **Tối Ưu Chi Phí**: Tiết kiệm tới **40% chi phí** so với các hệ thống BI truyền thống.
* **Chất Lượng Dữ Liệu**: Giảm tỷ lệ lỗi dữ liệu từ ~10% xuống dưới **2%**.
* **ROI**: Ước tính đạt **62% sau 3 tháng**.

### Kiến Trúc Giải Pháp

Kiến trúc hệ thống được thiết kế theo mô hình **serverless** và **modular**, nhằm đảm bảo tính hiệu quả về chi phí và khả năng mở rộng. 

**Các thành phần chính của kiến trúc:**
* **External Sources & Internal Uploads**: Dữ liệu từ các nguồn bên ngoài (CRM, Ads) và file nội bộ (Excel, CSV).
* **Amazon S3**: Lưu trữ dữ liệu thô với chi phí thấp.
* **AWS Glue Crawler + Data Catalog**: Tự động phát hiện schema dữ liệu và xây dựng metadata catalog.
* **Amazon Athena**: Truy vấn dữ liệu trực tiếp trên S3 bằng SQL.
* **Amazon QuickSight**: Trực quan hóa dữ liệu và cung cấp dashboard tương tác.
* **Embedded Iframe**: Dashboard được nhúng vào hệ thống nội bộ.