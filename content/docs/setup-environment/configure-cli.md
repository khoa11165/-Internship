---
title: "Cấu hình AWS CLI"
weight: 2
---

## 1.2. Cấu hình AWS CLI

### Bước 1: Cài đặt AWS CLI

Nếu bạn chưa cài đặt AWS CLI, hãy truy cập trang [Cài đặt AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) để tải về và cài đặt phiên bản phù hợp với hệ điều hành của bạn (Windows, macOS, Linux).

### Bước 2: Cấu hình tài khoản AWS CLI

Sau khi cài đặt, bạn cần cấu hình AWS CLI để nó có thể tương tác với tài khoản của bạn.
1.  Mở terminal hoặc Command Prompt.
2.  Chạy lệnh sau:
    ```bash
    aws configure
    ```
3.  Lệnh sẽ yêu cầu bạn nhập các thông tin sau:
    * **AWS Access Key ID**: Đăng nhập vào AWS Console, vào mục **IAM**, chọn **Users**, chọn user của bạn và tạo một Access Key.
    * **AWS Secret Access Key**: Sao chép và dán Secret Access Key vào đây.
    * **Default region name**: Nhập khu vực mặc định mà bạn muốn làm việc, ví dụ: `ap-southeast-1` (Singapore) hoặc `us-east-1` (Bắc Virginia).
    * **Default output format**: Để mặc định là `json`.

### Bước 3: Kiểm tra cấu hình

Để đảm bảo AWS CLI đã được cấu hình đúng, bạn hãy chạy lệnh sau để kiểm tra danh sách S3 bucket của mình:
```bash
aws s3 ls