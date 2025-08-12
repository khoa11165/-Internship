---
title: "Dọn dẹp Tài nguyên"
weight: 1
---

## 4.1. Dọn dẹp Tài nguyên

Hãy làm theo các bước dưới đây để xóa tất cả các tài nguyên bạn đã tạo trong suốt workshop.

### Bước 1: Dọn dẹp các tài nguyên trong QuickSight

1.  **Đăng nhập vào QuickSight**: Truy cập [AWS QuickSight Console](https://quicksight.aws.amazon.com/).
2.  **Xóa Dashboard**:
    * Trong menu bên trái, chọn **"Dashboards"**.
    * Chọn dashboard bạn đã tạo, nhấn vào biểu tượng **ba dấu chấm (...)** -> **"Delete"**.
3.  **Xóa Dataset**:
    * Trong menu bên trái, chọn **"Datasets"**.
    * Chọn dataset đã tạo, nhấn vào biểu tượng **ba dấu chấm (...)** -> **"Delete"**.


### Bước 2: Dọn dẹp các tài nguyên trong AWS Glue

1.  **Đăng nhập vào AWS Console**: Tìm kiếm **"Glue"**.
2.  **Xóa Crawler**:
    * Chọn **"Crawlers"** trong menu **"Data Catalog"**.
    * Chọn crawler bạn đã tạo, nhấn **"Actions"** -> **"Delete crawler"**.
3.  **Xóa Database**:
    * Chọn **"Databases"**.
    * Chọn database bạn đã tạo (ví dụ: `quicksight_workshop_db`), nhấn **"Actions"** -> **"Delete database"**.

### Bước 3: Dọn dẹp S3 Bucket (Quan trọng!)

Đây là bước quan trọng nhất để tránh chi phí lưu trữ. Bạn có thể chọn một trong hai cách dưới đây.

#### Cách 1: Sử dụng AWS CLI để xóa nhanh nhất (khuyến khích)

* Mở Terminal hoặc Command Prompt.
* Chạy lệnh sau để xóa toàn bộ các file trong bucket:
    ```bash
    aws s3 rm s3://quicksight-workshop-ten-cua-ban --recursive
    ```
* Tiếp theo, chạy lệnh này để xóa chính bucket đó:
    ```bash
    aws s3 rb s3://quicksight-workshop-ten-cua-ban
    ```
* **Lưu ý**: Thay `quicksight-workshop-ten-cua-ban` bằng tên bucket của bạn.

#### Cách 2: Xóa S3 Bucket thủ công qua Console

1.  **Đăng nhập vào AWS Console**: Tìm kiếm **"S3"**.
2.  **Xóa các đối tượng trong Bucket**:
    * Chọn S3 Bucket của bạn.
    * Nhấn vào tab **"Objects"**.
    * Chọn tất cả các file trong bucket, nhấn **"Delete"**.
    * Bạn sẽ cần nhập `permanently delete` để xác nhận việc xóa.
3.  **Xóa Bucket**:
    * Sau khi bucket trống, quay lại trang S3.
    * Chọn bucket của bạn, nhấn **"Actions"** -> **"Delete"**.
    * Bạn sẽ cần nhập lại tên bucket để xác nhận.


Sau khi bạn đã hoàn thành các bước trên, tất cả các tài nguyên liên quan đến workshop này sẽ được xóa hoàn toàn.