---
title: "Tùy chỉnh Visuals"
weight: 2
---

## 3.2. Tùy chỉnh và Làm đẹp Dashboard

QuickSight cung cấp một bộ công cụ mạnh mẽ để bạn có thể tùy chỉnh các biểu đồ (visuals) và layout của dashboard, giúp nó trở nên trực quan và dễ hiểu hơn.

### Mục tiêu

* Lựa chọn loại biểu đồ phù hợp cho từng loại dữ liệu.
* Tùy chỉnh màu sắc, nhãn, tiêu đề và thêm bộ lọc.
* Sắp xếp các visuals trên dashboard một cách hợp lý.

### Hướng dẫn chi tiết

#### Bước 1: Mở lại Phân tích (Analysis)

1.  Quay lại trang **"Analysis"** trong QuickSight.
2.  Mở phân tích mà bạn đã tạo ở bước trước (ví dụ: `Sales_Analytics_Analysis`).

#### Bước 2: Tùy chỉnh Biểu đồ (Visuals)

1.  **Chọn loại biểu đồ**:
    * Nhấn vào biểu đồ bạn muốn thay đổi.
    * Ở góc trên bên trái, bạn có thể thay đổi loại biểu đồ (ví dụ: từ biểu đồ cột sang biểu đồ tròn, biểu đồ đường,...)
    * **Mẹo**: Biểu đồ đường thích hợp cho dữ liệu theo thời gian. Biểu đồ cột/tròn thích hợp cho dữ liệu so sánh.

2.  **Tùy chỉnh các trường dữ liệu**:
    * **Ví dụ biểu đồ cột**:
        * **Kéo `region` vào mục "X axis"**.
        * **Kéo `sales` vào mục "Y axis"** và đảm bảo nó được tổng hợp (`Sum`).
    
    

3.  **Tùy chỉnh định dạng**:
    * Nhấn vào biểu đồ, sau đó chọn biểu tượng **"Format visual"** (thường là một bánh răng hoặc một bút lông).
    * Trong mục này, bạn có thể:
        * **Title**: Đặt tiêu đề cho biểu đồ, ví dụ: "Tổng Doanh Số theo Khu vực".
        * **Colors**: Thay đổi màu sắc của các thanh hoặc lát cắt.
        * **Labels**: Hiển thị nhãn dữ liệu trên biểu đồ.
        * **Axes**: Tùy chỉnh tên và định dạng của các trục X, Y.

#### Bước 3: Thêm Bộ lọc (Filters)

1.  Ở menu bên trái, chọn **"Filters"**.
2.  Nhấn **"Create filter"** và chọn một trường dữ liệu (ví dụ: `sales_date`).
3.  Bạn có thể tạo bộ lọc theo ngày, tháng, năm, v.v. để người dùng có thể tương tác với dashboard.
4.  **Ví dụ**: Thêm bộ lọc cho `sales_date` và chọn loại `Date Range`. Người dùng sau đó có thể chọn một khoảng thời gian để xem dữ liệu.


#### Bước 4: Cập nhật Dashboard

1.  Sau khi đã tùy chỉnh xong, nhấn **"Share"** ở góc trên bên phải.
2.  Chọn **"Publish dashboard"** và chọn dashboard của bạn để cập nhật với các thay đổi mới nhất.