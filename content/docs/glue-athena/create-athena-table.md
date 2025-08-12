---
title: "Tạo bảng Athena"
weight: 2
---

## 2.2. Truy vấn dữ liệu với Amazon Athena

Sau khi Glue Crawler đã "xử lý" và tạo metadata trong Data Catalog, **Amazon Athena** có thể sử dụng nó để **truy vấn dữ liệu** trực tiếp trên S3. Bước này giúp chúng ta xác minh dữ liệu đã sẵn sàng để sử dụng và chuẩn bị nó cho QuickSight.

### Mục tiêu
* Cấu hình nơi lưu kết quả truy vấn trong S3.
* Xác nhận bảng dữ liệu đã được tạo trong Athena.
* Hiểu mối quan hệ giữa Glue Data Catalog và Athena.

### Mối quan hệ Glue Data Catalog và Athena

Glue Data Catalog đóng vai trò như một kho chứa metadata trung tâm. Khi Athena truy vấn dữ liệu, nó sẽ không quét toàn bộ các file trong S3 mà sẽ tra cứu metadata trong Glue Data Catalog để biết cấu trúc dữ liệu (tên cột, kiểu dữ liệu, định dạng file...). Điều này giúp truy vấn nhanh hơn và hiệu quả hơn về mặt chi phí.

### Hướng dẫn

#### Bước 1: Truy cập và Cấu hình Athena

1.  Đăng nhập vào **AWS Console** và tìm kiếm **`Athena`**.
2.  Khi truy cập Athena lần đầu, bạn có thể được yêu cầu cấu hình một S3 bucket để lưu kết quả truy vấn. Điều này rất quan trọng vì Athena cần một nơi để lưu trữ kết quả của các câu lệnh truy vấn.
3.  Nhấn **"Edit settings"** ở góc trên bên phải.
4.  **Query result location**: Nhấn **"Browse S3"** và chọn S3 Bucket mà bạn đã tạo, sau đó tạo một thư mục con, ví dụ: `s3://quicksight-workshop-ten-cua-ban/athena-results/`.
5.  Nhấn **"Save"**.


#### Bước 2: Kiểm tra bảng dữ liệu

1.  Trong giao diện Athena, ở mục **"Database"** bên trái, chọn database mà bạn đã tạo trong Glue (ví dụ: `quicksight_workshop_db`).
2.  Trong mục **"Tables"**, bạn sẽ thấy một bảng mới, được tạo bởi Glue Crawler, ví dụ: `sales_data_csv`.


Bây giờ bạn đã có một bảng dữ liệu trong Athena, sẵn sàng cho việc truy vấn và là nguồn dữ liệu trực tiếp cho QuickSight.