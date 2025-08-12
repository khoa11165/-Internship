---
title: "Tạo Dashboard"
weight: 1
---

## 3.1. Tạo Dashboard QuickSight

Sau khi đã có bảng dữ liệu trong Athena, chúng ta sẽ sử dụng nó làm nguồn dữ liệu cho QuickSight.

### Mục tiêu

* Kết nối QuickSight với Athena thông qua một **Data Source**.
* Tạo một **Dataset** mới từ bảng Athena để sử dụng trong các phân tích.
* Tạo một phân tích (**Analysis**) và xuất bản thành một **Dashboard** hoàn chỉnh.

### Hướng dẫn chi tiết

#### Bước 1: Đăng nhập và Truy cập QuickSight

1.  Đăng nhập vào **AWS Management Console** và tìm kiếm **`QuickSight`**.
2.  Nếu bạn chưa có tài khoản QuickSight, bạn sẽ cần đăng ký. Hãy chọn phiên bản **Standard** hoặc **Enterprise** và hoàn tất quá trình đăng ký ban đầu.

#### Bước 2: Tạo Data Source và Dataset

1.  Trong giao diện QuickSight, nhấn vào **"Datasets"** ở menu bên trái.
2.  Nhấn **"New dataset"**.
3.  Trong danh sách các nguồn dữ liệu, chọn **"Athena"**.


4.  **Data source name**: Đặt tên cho nguồn dữ liệu, ví dụ: `Athena_quicksight_workshop`.
5.  Nhấn **"Validate connection"** và sau đó **"Create data source"**.

6.  **Chọn bảng dữ liệu**:
    * Trong danh sách các database, chọn database của bạn đã tạo trong Glue (ví dụ: `quicksight_workshop_db`).
    * Chọn bảng dữ liệu đã được Glue tạo (ví dụ: `sales_data_csv`).
    * Nhấn **"Select"**.

7.  **Cấu hình Dataset**:
    * QuickSight sẽ hỏi bạn muốn sử dụng **SPICE** (in-memory) hay truy vấn trực tiếp (**Direct query**).
    * Chọn **"Direct query"** để truy vấn dữ liệu trực tiếp từ Athena. Điều này giúp đảm bảo dữ liệu trên dashboard luôn cập nhật.
    * Nhấn **"Visualize"**.


#### Bước 3: Tạo và Xuất bản Dashboard

1.  QuickSight sẽ mở một trang phân tích (**Analysis**). Đây là nơi bạn sẽ xây dựng các biểu đồ.
2.  Tại đây, bạn có thể kéo và thả các trường dữ liệu (`fields`) vào các vùng để tạo các biểu đồ. Ví dụ:
    * Kéo **`sales_date`** vào trục X.
    * Kéo **`sales`** vào trục Y.
    * Kéo **`region`** vào mục **"Group/Color"** để nhóm dữ liệu theo khu vực.
3.  Sau khi đã có các biểu đồ ưng ý, nhấn **"Share"** ở góc trên bên phải và chọn **"Publish dashboard"**.
4.  **Dashboard name**: Đặt tên, ví dụ: `Sales_Analytics_Dashboard`.
5.  Nhấn **"Publish dashboard"**.