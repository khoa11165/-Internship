---
title: "Tạo Glue Crawler"
weight: 1
---

## 2.1. Tạo AWS Glue Crawler (Xử lý dữ liệu)

Trong luồng dữ liệu của chúng ta, bước đầu tiên sau khi dữ liệu được tải lên S3 là xử lý nó. Tuy nhiên, thay vì phải viết code phức tạp, chúng ta sẽ sử dụng **AWS Glue Crawler** để tự động "xử lý" bằng cách khám phá và tạo ra metadata (schema) cho dữ liệu. Metadata này sau đó sẽ được lưu trong **AWS Glue Data Catalog**.

### Mục tiêu
* **Tải dữ liệu mẫu lên S3 Bucket.**
* Tạo một Glue Crawler để quét file dữ liệu mẫu đó.
* Tạo một IAM Role để cấp quyền cho Glue truy cập vào S3.
* Tạo ra một bảng metadata trong Data Catalog.

### Bước 1: Chuẩn bị và tải dữ liệu mẫu lên S3

Trước khi tạo crawler, bạn cần tải một file dữ liệu mẫu lên S3 Bucket mà bạn đã tạo ở phần trước.
1.  **Tạo file CSV**: Mở một trình chỉnh sửa văn bản và tạo một file mới tên là **`sales_data.csv`** với nội dung sau:
    ```csv
    order_id,product_name,sales,region,sales_date,customer_id
    1,Laptop,1200,North America,2024-01-15,CUST001
    2,Mouse,25,Europe,2024-01-16,CUST002
    3,Keyboard,75,North America,2024-01-17,CUST001
    4,Monitor,300,Asia,2024-01-18,CUST003
    5,Headphones,50,Europe,2024-01-19,CUST002
    6,Laptop,1500,North America,2024-02-20,CUST004
    7,Mouse,30,Asia,2024-02-21,CUST005
    8,Keyboard,80,Europe,2024-02-22,CUST006
    9,Monitor,350,North America,2024-02-23,CUST004
    10,Headphones,60,Asia,2024-02-24,CUST007
    ```
2.  **Tải lên S3 Bucket**: Bạn có thể tải file lên qua AWS Console hoặc sử dụng AWS CLI.
    * **Qua Console**: Mở S3 Console, chọn bucket của bạn và nhấn **"Upload"** để tải file `sales_data.csv` lên.
    * **Qua AWS CLI**: Mở terminal và chạy lệnh sau (thay đổi tên bucket của bạn):
        ```bash
        aws s3 cp sales_data.csv s3://quicksight-workshop-ten-cua-ban/
        ```
    ![Giao diện tải file lên S3 Bucket của AWS](/images/upload-s3.png)

### Bước 2: Truy cập AWS Glue và Tạo Crawler

1.  Đăng nhập vào **AWS Management Console** và tìm kiếm **`Glue`**.
2.  Trong menu bên trái, dưới mục **"Data Catalog"**, chọn **"Crawlers"**. Nhấn **"Create crawler"** để bắt đầu.


### Bước 3: Cấu hình Crawler

1.  **Name**: Đặt tên cho crawler của bạn, ví dụ: `quicksight-workshop-crawler`.
2.  **Data source**: Nhấn **"Add a data source"**.
    * **Choose a data source**: Chọn **"S3"**.
    * **Crawl data in**: Chọn **"In the current account"**.
    * **S3 path**: Nhấn **"Browse S3"** và chọn S3 Bucket mà bạn đã tải file `sales_data.csv` lên.
    * Nhấn **"Add"**.


### Bước 4: Tạo IAM Role và Chạy Crawler

1.  **IAM role**: Chọn **"Create new IAM role"**. Đặt tên, ví dụ: `AWSGlueServiceRole-quicksight-workshop`. Vai trò này sẽ cấp quyền cho Glue để đọc dữ liệu từ S3.
2.  **Target database**: Nhấn **"Add a database"** và tạo một database mới, ví dụ: `quicksight_workshop_db`.
3.  **Frequency**: Để mặc định là **"On demand"** (chỉ chạy khi bạn yêu cầu).
4.  Nhấn **"Next"** và **"Finish"** để hoàn tất việc tạo crawler.
5.  Trong danh sách các crawler, chọn crawler bạn vừa tạo và nhấn **"Run"**. Quá trình này có thể mất vài phút.


Sau khi chạy xong, Glue sẽ hoàn thành việc "xử lý" dữ liệu của bạn và tạo một bảng metadata trong Data Catalog.