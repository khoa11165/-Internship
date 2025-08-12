---
title: "Nhúng Dashboard"
weight: 3
---

## 3.3. Nhúng Dashboard QuickSight (Embedded Analytics)

Một trong những tính năng mạnh mẽ và giá trị nhất của QuickSight là khả năng nhúng dashboard vào các ứng dụng web hoặc cổng thông tin nội bộ của bạn. Điều này biến dashboard thành một phần không thể thiếu của hệ thống, giúp người dùng dễ dàng truy cập thông tin mà không cần phải rời khỏi ứng dụng.

### Mục tiêu

* Tạo một link nhúng (embed) cho dashboard của bạn.
* Hiểu cách sử dụng iframe để hiển thị dashboard.
* Tìm hiểu về các tùy chỉnh nâng cao cho dashboard nhúng.

### Hướng dẫn chi tiết

#### Bước 1: Chuẩn bị để Nhúng Dashboard

Để nhúng dashboard, bạn cần đảm bảo rằng người dùng có quyền truy cập.
1.  **Truy cập Dashboard đã Publish**: Trong QuickSight, vào mục **"Dashboards"** và chọn dashboard mà bạn đã tạo.
2.  **Chia sẻ Dashboard**: Nhấn nút **"Share"** ở góc trên bên phải.
    * Chọn **"Share with users and groups"** để cấp quyền cho những người dùng cần thiết.
    * **Lưu ý**: Trong môi trường sản phẩm, bạn nên sử dụng **Row-Level Security (RLS)** để đảm bảo người dùng chỉ xem được dữ liệu mà họ có quyền.

#### Bước 2: Lấy mã nhúng (Embed Code)

1.  Sau khi chia sẻ, trong menu **"Share"**, bạn có thể tìm thấy tùy chọn để lấy mã nhúng.
2.  QuickSight sẽ cung cấp cho bạn một đoạn mã **`iframe`** để nhúng dashboard.
3.  Đoạn mã sẽ có dạng tương tự như sau:
    
    ```html
    <iframe width="1000" height="600"
        src="[https://ap-southeast-1.quicksight.aws.amazon.com/sn/dashboards/](https://ap-southeast-1.quicksight.aws.amazon.com/sn/dashboards/)..."
        style="border:0">
    </iframe>
    ```
    
    * **Giải thích**:
        * `width="1000"` và `height="600"`: Kích thước của khung dashboard.
        * `src="..."`: URL của dashboard đã được chia sẻ.
        * `style="border:0"`: Xóa viền khung.
    
4.  Bạn có thể sao chép đoạn mã này và dán vào bất kỳ trang web nào.

#### Bước 3: Tùy chỉnh Nâng cao cho Nhúng Dashboard

Bạn có thể tùy chỉnh URL trong thẻ `iframe` để điều chỉnh hành vi của dashboard nhúng.
* **Ẩn thanh điều hướng**: Thêm `&amp;embed=true` vào cuối URL để ẩn thanh menu của QuickSight.
* **Thêm bộ lọc mặc định**: Bạn có thể truyền các tham số lọc vào URL. Ví dụ, để lọc theo `region='North America'`, bạn có thể thêm: `&amp;filter-region=North America`.

```html
<iframe
    width="1200"
    height="800"
    src="[https://ap-southeast-1.quicksight.aws.amazon.com/sn/dashboards/your-dashboard-id?&embed=true&filter-region=North%20America](https://ap-southeast-1.quicksight.aws.amazon.com/sn/dashboards/your-dashboard-id?&embed=true&filter-region=North%20America)"
    style="border:1px solid #ccc; border-radius: 8px;">
</iframe>