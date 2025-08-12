---
title: "Truy vấn dữ liệu"
weight: 3
---

## 2.3. Truy vấn Dữ liệu với Athena

Bây giờ bạn đã có bảng dữ liệu trong Athena, bạn có thể bắt đầu sử dụng SQL để phân tích. Đây là bước cuối cùng trong Phần 2, nơi chúng ta xác minh dữ liệu đã sẵn sàng và hiểu rõ hơn về nội dung của nó.

### Mục tiêu
* Chạy các câu lệnh SQL để truy vấn và phân tích dữ liệu.
* Hiểu cách Athena hoạt động với dữ liệu trên S3.

### Hướng dẫn

#### Bước 1: Mở trình soạn thảo truy vấn
1.  Trong giao diện Athena, bạn sẽ thấy một trình soạn thảo (query editor) để viết các câu lệnh SQL.


#### Bước 2: Chạy các câu lệnh SQL

1.  **Truy vấn dữ liệu cơ bản**: Chạy câu lệnh sau để xem tất cả các cột của 10 dòng đầu tiên của bảng:
    ```sql
    SELECT * FROM "quicksight_workshop_db"."sales_data_csv" LIMIT 10;
    ```
    * **Lưu ý**: Thay `quicksight_workshop_db` và `sales_data_csv` bằng tên database và bảng của bạn.

2.  **Truy vấn phân tích**: Thử chạy một truy vấn phức tạp hơn để tính tổng doanh số bán hàng theo từng khu vực:
    ```sql
    SELECT
        region,
        SUM(sales) AS total_sales
    FROM "quicksight_workshop_db"."sales_data_csv"
    GROUP BY
        region
    ORDER BY
        total_sales DESC;
    ```
    Kết quả của truy vấn này sẽ cho bạn biết khu vực nào có doanh số cao nhất.

3.  **Truy vấn nâng cao**: Sử dụng mệnh đề `WHERE` để lọc dữ liệu theo một điều kiện cụ thể. Ví dụ, truy vấn doanh số bán hàng của riêng `North America` trong năm 2024:
    ```sql
    SELECT
        product_name,
        sales,
        sales_date
    FROM "quicksight_workshop_db"."sales_data_csv"
    WHERE
        region = 'North America' AND YEAR(sales_date) = 2024
    ORDER BY
        sales_date ASC;
    ```
    
    * Lưu ý: Athena hỗ trợ các hàm SQL phổ biến như `YEAR()` để trích xuất năm từ một cột kiểu `date`.

Bạn đã thành thạo việc sử dụng Athena để truy vấn dữ liệu. Kết quả từ các truy vấn này có thể được sử dụng làm nguồn dữ liệu cho QuickSight ở phần tiếp theo.