TÊN DỰ ÁN: ADVANCED ANALYTICS VỚI QUICKSIGHT VÀ CUSTOM VISUALIZATIONS

(Phát triển nền tảng phân tích nâng cao với QuickSight, hình ảnh hóa tùy chỉnh, phân tích nhúng, quản lý người dùng. Phát triển hình ảnh hóa, triển khai nhúng, quản lý người dùng, tối ưu hóa hiệu suất, phân tích chi phí, thiết lập giám sát, quy trình vận hành, tài liệu đào tạo.)

CHƯƠNG 1. TÓM TẮT NỘI DUNG

1.1. Tổng quan dự án

Trong bối cảnh doanh nghiệp ngày càng phụ thuộc vào dữ liệu để ra quyết định, nhu cầu về một hệ thống phân tích hiện đại, trực quan và dễ tích hợp trở nên cấp thiết. Dự án “Nâng cao phân tích dữ liệu doanh nghiệp bằng Amazon QuickSight và trực quan hóa tùy chỉnh” nhằm giải quyết bài toán phân tích và trực quan hóa dữ liệu một cách linh hoạt, nhanh chóng và tiết kiệm chi phí trên nền tảng AWS.

1.2. Giải pháp tổng thể

Giải pháp sử dụng Amazon QuickSight làm công cụ chính để xây dựng hệ thống dashboard phân tích dữ liệu bán hàng và hành vi khách hàng. Dữ liệu được thu thập từ Amazon S3, xử lý bằng AWS Glue, truy vấn bằng Athena, và trực quan hóa bằng QuickSight. Dashboard sau đó sẽ được nhúng (embedded) vào hệ thống CRM nội bộ của doanh nghiệp thông qua iframe. Giải pháp hỗ trợ phân quyền truy cập theo vai trò người dùng (Row-Level Security), đảm bảo bảo mật và tuân thủ.

Giải pháp không chỉ cải thiện hiệu suất xử lý và truy cập dữ liệu, mà còn giúp rút ngắn thời gian tạo báo cáo từ 2–3 ngày xuống dưới 15 phút, đồng thời tiết kiệm tới 40% chi phí so với hệ thống BI truyền thống.

Giải pháp này không chỉ cải thiện hiệu suất truy cập và xử lý dữ liệu, mà còn giúp giảm thời gian tạo báo cáo từ 2 ngày xuống còn 15 phút, đồng thời giảm chi phí triển khai hệ thống Business Intelligence truyền thống lên đến 40%.

1.3. Các tính năng chính của giải pháp

Tự động thu thập và cập nhật dữ liệu từ S3 nhờ AWS Glue Crawler và Data Catalog.

Truy vấn dữ liệu linh hoạt bằng Amazon Athena mà không cần thiết lập máy chủ.

Dashboard phân tích động sử dụng QuickSight, có thể tạo biểu đồ đa dạng: line chart, bar chart, heatmap, v.v.

Tích hợp vào hệ thống CRM nội bộ qua tính năng nhúng iframe.

Quản lý người dùng và phân quyền bảo mật bằng Amazon Cognito và QuickSight Row-Level Security.

Khả năng mở rộng dễ dàng cho các loại dữ liệu khác như dữ liệu vận hành, marketing, chăm sóc khách hàng.

1.4. Lợi ích kinh doanh và ROI

Giải pháp mang lại nhiều lợi ích rõ ràng về mặt vận hành và chiến lược:

| Hạng mục | Trước khi triển khai | Sau khi triển khai |
| --- | --- | --- |
| Thời gian tạo báo cáo | 2–3 ngày | < 15 phút |
| Tỷ lệ lỗi dữ liệu | ~10% | < 2% |
| Số lượng người dùng có thể tự tạo dashboard | 0 | > 80% |
| Chi phí vận hành hệ thống BI | ~800 USD/tháng | ~300 USD/tháng |
| ROI ước tính | — | ~62% sau 3 tháng |


Giải pháp không chỉ giảm đáng kể chi phí vận hành mà còn giúp doanh nghiệp tăng tốc độ ra quyết định, nhờ có khả năng truy cập dữ liệu gần như thời gian thực (near real-time). Đây là yếu tố sống còn trong các môi trường có tốc độ biến đổi cao như thương mại điện tử, bán lẻ và dịch vụ.

1.5. Yêu cầu đầu tư và thời gian

Chi phí hạ tầng AWS: khoảng 300 USD/tháng cho 5 người dùng (QuickSight, Glue, Athena)

Chi phí phát triển ban đầu: 1.000 USD (chi phí nhân lực)

Thời gian triển khai: 6 tuần (theo kế hoạch chi tiết)

Yêu cầu nhân sự: 1 kỹ sư dữ liệu, 1 kiến trúc sư AWS, 1 nhân sự kiểm thử/đào tạo

1.6. Kết quả mong đợi & chỉ số thành công

Giải pháp đặt ra các chỉ số thành công (KPI) cụ thể như sau:

Giảm thời gian tạo báo cáo xuống dưới 15 phút

Tăng độ chính xác dữ liệu trên 98%

Tăng khả năng sử dụng dashboard bởi các phòng ban: > 80%

Tăng tần suất truy cập dashboard > 30% so với hệ thống cũ

Giảm chi phí vận hành BI truyền thống ít nhất 40%

Về lâu dài, doanh nghiệp sẽ có một hệ thống phân tích hiện đại, dễ mở rộng, có thể tích hợp thêm dữ liệu từ các nền tảng như Google Ads, Facebook, hệ thống CRM, hệ thống vận chuyển,... Điều này giúp gia tăng năng lực phân tích toàn diện và năng lực cạnh tranh trên thị trường.

CHƯƠNG 2. ĐẶT VẤN ĐỀ

2.1. Phân tích tình hình hiện tại

Trong kỷ nguyên số, dữ liệu không chỉ là tài sản mà còn là nền tảng của khả năng cạnh tranh. Tuy nhiên, ở nhiều doanh nghiệp vừa và nhỏ, đặc biệt trong lĩnh vực bán lẻ và thương mại điện tử, hạ tầng phân tích dữ liệu vẫn còn rời rạc, kém hiệu quả và chưa đủ linh hoạt để hỗ trợ ra quyết định nhanh chóng.

Một số đặc điểm phổ biến của hệ thống hiện tại:

Phân tán dữ liệu: Thông tin được lưu trữ ở nhiều nơi như Google Sheets, file Excel nội bộ, phần mềm bán hàng, CRM và các nền tảng quảng cáo (Google Ads, Facebook Ads) mà không có hệ thống tập trung.

Báo cáo thủ công: Việc thu thập và tổng hợp dữ liệu phải thực hiện bằng tay mỗi lần, phụ thuộc nhiều vào nhân sự IT hoặc Data Analyst.

Hạn chế truy cập: Người dùng phải gửi yêu cầu mới có thể nhận được báo cáo. Hệ thống không cung cấp giao diện cho phép người dùng chủ động khám phá dữ liệu.

Không có phân quyền rõ ràng: Mọi người cùng xem một báo cáo tổng, thiếu kiểm soát và bảo mật thông tin nhạy cảm.

Không thể mở rộng: Khi dữ liệu phát sinh nhiều hơn (ví dụ tăng số sản phẩm, tăng số chiến dịch), hệ thống trở nên chậm chạp, gây tắc nghẽn và làm giảm hiệu quả hoạt động.

2.2. Xác định điểm đau & tác động định lượng

Các điểm đau chính có thể được chia thành ba nhóm: (1) vận hành, (2) kỹ thuật và (3) kinh doanh.

2.2.1. Vận hành

| Vấn đề | Tác động |
| --- | --- |
| Báo cáo thủ công, phụ thuộc IT | Mất 2–3 ngày để tổng hợp 1 báo cáo tổng quan |
| Thiếu khả năng tự phục vụ | Người dùng kinh doanh không thể chủ động khai thác dữ liệu |
| Thiếu dashboard tổng thể | Quản lý không nhìn thấy toàn cảnh hiệu suất doanh nghiệp |


2.2.2. Kỹ thuật

| Vấn đề | Tác động |
| --- | --- |
| Dữ liệu phân mảnh | Khó phân tích toàn diện, thiếu tính kết nối giữa các nguồn |
| Không có hệ thống kiểm thử/bảo trì | Rủi ro sai sót khi chỉnh sửa công thức |
| Thiếu khả năng mở rộng | Mỗi thay đổi dữ liệu đều phải can thiệp bằng tay |


2.2.3. Kinh doanh

| Vấn đề | Tác động định lượng |
| --- | --- |
| Tốc độ ra quyết định chậm | Mất 2–3 ngày để ra quyết định dựa trên dữ liệu |
| Lỗi dữ liệu ảnh hưởng KPI | Tỷ lệ sai lệch số liệu ~10% gây sai lệch trong kế hoạch kinh doanh |
| Chi phí vận hành cao | ~800 USD/tháng cho nhân sự và hệ thống phân tích cũ |


2.3. Các bên liên quan và mối quan tâm

Việc triển khai hệ thống phân tích hiện đại sẽ ảnh hưởng đến nhiều bộ phận trong doanh nghiệp. Dưới đây là phân tích các nhóm chính:

| Bên liên quan | Vai trò | Mối quan tâm chính |
| --- | --- | --- |
| Quản lý cấp cao (CEO) | Quyết định chiến lược toàn doanh nghiệp | Có cái nhìn tổng thể về hiệu suất, dòng tiền, tăng trưởng |
| Quản lý bộ phận (CMO, Sales Lead) | Vận hành chiến dịch marketing, bán hàng | Muốn theo dõi realtime hiệu quả từng chiến dịch, sản phẩm, khu vực |
| Nhân viên văn phòng | Thực hiện công việc hằng ngày | Cần dashboard dễ hiểu, dễ sử dụng, không cần học kỹ thuật |
| Bộ phận Kỹ thuật/IT | Bảo trì và tích hợp hệ thống | Muốn hệ thống ổn định, dễ triển khai, ít bảo trì |
| Nhân viên phân tích dữ liệu | Tổng hợp, phân tích, lập báo cáo | Muốn tự động hóa và tối ưu quy trình tạo báo cáo thay vì làm tay mỗi ngày |


2.4. Hậu quả nếu không hành động

Nếu tiếp tục duy trì hệ thống báo cáo cũ, doanh nghiệp sẽ đối mặt với những hậu quả sau:

Chậm trễ trong phản ứng thị trường: Khi không thể cập nhật dữ liệu nhanh chóng, các quyết định bị trễ, mất cơ hội kinh doanh.

Chi phí nhân lực và vận hành tăng cao: Việc tạo báo cáo bằng tay cần nhiều nhân sự chuyên môn, không bền vững khi doanh nghiệp mở rộng.

Thiếu bảo mật và tuân thủ: Không có phân quyền dữ liệu sẽ gây rủi ro rò rỉ thông tin nhạy cảm giữa các phòng ban.

Khó cạnh tranh với đối thủ: Đối thủ đã chuyển sang các nền tảng BI hiện đại, cho phép hành động nhanh và chính xác hơn.

Không sẵn sàng tích hợp AI/ML trong tương lai: Nếu hệ thống không chuẩn hóa và hiện đại, sẽ rất khó tích hợp các tính năng phân tích nâng cao sau này.

2.5. Cơ hội thị trường và động lực chuyển đổi

Theo báo cáo của Gartner (2024):

“85% doanh nghiệp sẽ áp dụng chiến lược Cloud BI-first vào năm 2026, nhằm tận dụng tính linh hoạt, hiệu suất và chi phí thấp của nền tảng đám mây.”

Ngoài ra:

Nền tảng Amazon QuickSight hiện đang phục vụ hơn 100.000 khách hàng toàn cầu, bao gồm Siemens, 3M, Amazon.com.

Doanh nghiệp có thể tiết kiệm 40–60% chi phí BI so với các giải pháp on-premise hoặc nền tảng truyền thống như Power BI Enterprise hoặc Tableau Server.

Thời gian triển khai trung bình cho hệ thống phân tích trên AWS chỉ từ 4–6 tuần, thấp hơn nhiều so với các giải pháp cũ cần vài tháng.

CHƯƠNG 3. KIẾN TRÚC GIẢI PHÁP

3.1. Mục tiêu và nguyên tắc thiết kế kiến trúc

Mục tiêu chính:

Dự án hướng tới việc xây dựng một hệ thống phân tích dữ liệu trên nền tảng AWS với những yêu cầu sau:

Hiệu quả về chi phí (Cost-effective): Không cần đầu tư hạ tầng vật lý, trả phí theo mức sử dụng.

Phân tích dữ liệu đa nguồn linh hoạt: Có thể thu thập từ các file thủ công, hệ thống CRM, nền tảng quảng cáo (Facebook Ads, Google Ads),...

Dễ sử dụng và trực quan: Người dùng không cần kiến thức kỹ thuật vẫn có thể sử dụng dashboard.

Tích hợp liền mạch: Dashboard được nhúng trực tiếp vào hệ thống nội bộ mà không phải rời khỏi nền tảng chính.

Bảo mật & phân quyền rõ ràng: Dữ liệu được bảo vệ theo từng người dùng, từng phòng ban.

Dễ mở rộng trong tương lai: Có thể tích hợp AI/ML, realtime analytics nếu cần.

Nguyên tắc kiến trúc:

Modular hóa từng thành phần (ETL, Query, BI) để dễ thay thế và bảo trì

Không máy chủ (Serverless) để giảm chi phí quản lý và tăng khả năng mở rộng

Automation-first: Tối ưu tự động hóa từ ingest → transform → visualize

Security-by-design: Thiết kế bảo mật ngay từ đầu bằng Cognito, IAM, RLS

Hệ thống kiến trúc:

Hình 3.1 – Kiến trúc hệ thống phân tích dữ liệu sử dụng Amazon QuickSight

Hệ thống gồm các thành phần chính:

External Sources (CRM, Ads, etc.): Thu thập dữ liệu từ các hệ thống bên ngoài như CRM, Google Ads, Facebook Ads.

Internal Uploads (Excel, CSV…): Nhập dữ liệu thủ công hoặc định kỳ từ nhân sự văn phòng.

Amazon S3: Lưu trữ dữ liệu thô với khả năng mở rộng và chi phí thấp.

AWS Glue Crawler + Data Catalog: Tự động phát hiện schema và xây dựng metadata catalog phục vụ cho Athena.

Amazon Athena: Truy vấn dữ liệu trực tiếp từ S3 bằng SQL mà không cần xây dựng hạ tầng máy chủ.

Amazon QuickSight: Trực quan hóa dữ liệu, cung cấp dashboard theo phân quyền người dùng (RLS).

Embedded Iframe (CRM): Nhúng dashboard QuickSight vào hệ thống CRM nội bộ, tạo trải nghiệm liền mạch cho người dùng.

3.2. Mô hình tổng quan kiến trúc hệ thống

| Tầng chức năng | Mô tả |
| --- | --- |
| Tầng lưu trữ (Storage) | Amazon S3 lưu trữ dữ liệu thô từ nhiều nguồn (CSV, CRM, API...) |
| Tầng xử lý & chuyển đổi | AWS Glue + Glue Crawler để tự động tạo schema và xử lý dữ liệu |
| Tầng truy vấn (Query) | Amazon Athena để viết truy vấn SQL trực tiếp lên dữ liệu trong S3 |
| Tầng trực quan hóa | Amazon QuickSight để xây dựng dashboard với biểu đồ, bộ lọc, drill-down dữ liệu |
| Tầng nhúng & bảo mật | Nhúng iframe vào CRM nội bộ, quản lý phân quyền bằng Amazon Cognito & QuickSight RLS |


3.3. Mô tả luồng dữ liệu chi tiết

  Ingestion:

Dữ liệu đầu vào từ CRM, file CSV Excel, Facebook Ads, Google Ads,... được đồng bộ hoặc tải lên Amazon S3 theo từng phân vùng thời gian.

Mỗi lần dữ liệu được cập nhật, Glue Crawler sẽ tự động quét và cập nhật schema (không cần ETL thủ công).

  Data Cataloging:

Glue Catalog giữ metadata và schema của từng bảng, làm nền tảng cho việc truy vấn qua Athena và tạo bảng trong QuickSight.

  Query và phân tích:

Athena được dùng để viết truy vấn SQL linh hoạt (JOIN, GROUP BY, WINDOW FUNCTION...) trực tiếp trên S3.

Không cần cài đặt máy chủ hoặc DB cố định → tiết kiệm chi phí vận hành.

  Visualization:

QuickSight đọc kết quả từ Athena và kết nối SPICE để tăng tốc độ hiển thị dashboard.

Người dùng có thể tương tác với biểu đồ (lọc theo ngày, khu vực, sản phẩm...).

  Embedding và phân quyền:

Dashboard được nhúng (embed) vào hệ thống CRM nội bộ bằng iframe.

Quyền truy cập được kiểm soát bằng Amazon Cognito, kết hợp Row-Level Security (RLS) để chỉ hiển thị dữ liệu tương ứng cho từng user.

3.4. Giải thích lựa chọn dịch vụ AWS

| Dịch vụ AWS | Vai trò chính | Lý do lựa chọn |
| --- | --- | --- |
| Amazon S3 | Lưu trữ dữ liệu | Dung lượng không giới hạn, chi phí rẻ, hỗ trợ nhiều định dạng (CSV, JSON, Parquet) |
| AWS Glue Crawler | Khám phá và tạo schema | Tự động nhận diện cột, loại dữ liệu → không cần viết schema bằng tay |
| AWS Glue Catalog | Metadata trung tâm | Là nguồn chính để Athena và QuickSight đọc schema |
| Amazon Athena | Truy vấn dữ liệu | SQL trực tiếp trên S3, chi phí tính theo số GB dữ liệu truy vấn |
| Amazon QuickSight | Tạo dashboard phân tích | Giao diện BI hiện đại, hỗ trợ embedding và phân quyền |
| Amazon Cognito | Quản lý người dùng và phân quyền | Tạo user, đăng nhập, phân quyền chi tiết theo nhóm |


3.5. Kiến trúc bảo mật và tuân thủ

| Thành phần bảo mật | Chi tiết triển khai |
| --- | --- |
| Authentication | Sử dụng Amazon Cognito để đăng nhập người dùng, cấp token |
| Authorization | Sử dụng QuickSight Row-Level Security để chỉ hiển thị dữ liệu người dùng được phép |
| Encryption | Dữ liệu S3 được mã hóa tự động bằng AWS-KMS hoặc SSE-S3 |
| Access Logging | CloudTrail ghi lại truy cập, cấu hình và thao tác trên Glue, Athena, QuickSight... |
| IAM Roles | Giới hạn quyền theo nguyên tắc Least Privilege |


3.6. Khả năng mở rộng & hiệu suất

| Yếu tố mở rộng | Cách giải quyết cụ thể |
| --- | --- |
| Tăng người dùng | QuickSight có thể phục vụ hàng trăm user nhờ SPICE Engine |
| Tăng nguồn dữ liệu | Glue Crawler có thể quét bất kỳ S3 folder nào mới thêm |
| Tăng loại phân tích | Có thể viết thêm truy vấn SQL trên Athena hoặc mô hình ML với SageMaker |
| Tăng khối lượng dữ liệu | Glue & Athena scale tự động (không phải provisioning EC2 hay RDS thủ công) |


3.7. Tích hợp với hệ thống hiện tại

- CRM nội bộ (hoặc hệ thống web quản trị) có thể nhúng dashboard thông qua iframe URL với user token đã đăng nhập.

- Giao diện người dùng có thể thiết kế đơn giản như sau:

<iframe src="https://quicksight.aws.amazon.com/.../embedUrl" width="100%" height="800"></iframe>

- Người dùng chỉ cần đăng nhập một lần bằng tài khoản Cognito → được truy cập đúng dashboard, đúng dữ liệu.

3.8. Mở rộng tương lai

| Hướng mở rộng | Mô tả cụ thể |
| --- | --- |
| Tích hợp AI/ML | Dùng Amazon SageMaker để dự đoán doanh thu, phân loại khách hàng |
| Realtime Streaming | Dùng Amazon Kinesis Data Firehose + Lambda để xử lý dữ liệu realtime |
| Alerting + Automation | Dùng Amazon CloudWatch và SNS để gửi cảnh báo khi KPI vượt ngưỡng |
| Data Lake Architecture | Kết hợp thêm Data Lake S3 + Lake Formation để phân quyền và phân tích sâu rộng hơn |


CHƯƠNG 4. TRIỂN KHAI KỸ THUẬT

4.1. Các giai đoạn triển khai

Quy trình triển khai giải pháp gồm 5 giai đoạn chính, được lập kế hoạch trong khoảng 6 tuần, cụ thể:

| Giai đoạn | Thời gian | Sản phẩm đầu ra |
| --- | --- | --- |
| 1. Phân tích yêu cầu và thiết kế | Tuần 1 | Tài liệu yêu cầu dữ liệu, sơ đồ kiến trúc, phân quyền người dùng |
| 2. Chuẩn hóa dữ liệu đầu vào | Tuần 2 | S3 bucket chứa dữ liệu, schema định nghĩa trong Glue Data Catalog |
| 3. Triển khai pipeline xử lý | Tuần 3–4 | Glue crawler, ETL jobs, bảng Athena kết nối dữ liệu |
| 4. Xây dựng dashboard QuickSight | Tuần 5 | 3–5 dashboard cho các nhóm chức năng (marketing, bán hàng, quản lý điều hành) |
| 5. Nhúng, phân quyền và kiểm thử | Tuần 6 | Tính năng nhúng iframe, xác thực Cognito, kiểm thử và nghiệm thu nội bộ |


4.2. Yêu cầu kỹ thuật

4.2.1. Tài nguyên AWS

| Dịch vụ | Vai trò |
| --- | --- |
| Amazon S3 | Lưu trữ dữ liệu gốc (CSV, JSON, log), chia theo partition ngày/tháng |
| AWS Glue | Tự động crawl schema và chạy ETL nếu cần chuẩn hóa dữ liệu đầu vào |
| AWS Athena | Truy vấn dữ liệu trực tiếp từ S3 không cần hạ tầng máy chủ |
| Amazon QuickSight | Trực quan hóa dữ liệu, dùng SPICE để tăng tốc độ |
| Amazon Cognito | Xác thực người dùng, phân quyền login và bảo mật dashboard |
| IAM | Quản lý quyền truy cập giữa các dịch vụ AWS |


4.2.2. Phần mềm bổ trợ

- Google Sheets API / Facebook Ads API (nếu mở rộng): để crawl dữ liệu marketing.

- Python script: viết script ETL cục bộ khi cần xử lý dữ liệu đặc thù.

- Bash/CLI: quản lý quyền IAM, kiểm thử truy cập bằng AWS CLI.

4.3. Phương pháp phát triển và chiến lược kiểm thử

4.3.1. Phương pháp phát triển

Áp dụng mô hình phát triển Agile – lặp và cải tiến liên tục, ưu tiên demo sớm:

Mỗi dashboard sẽ được xây dựng theo chu kỳ: Thu thập yêu cầu → Prototype → Demo → Hoàn thiện

Dữ liệu mẫu sẽ được sử dụng trước khi có dữ liệu thực

Giao diện nhúng iframe sẽ được thiết kế tương thích responsive với CRM hiện tại

4.3.2. Chiến lược kiểm thử

| Loại kiểm thử | Mục tiêu |
| --- | --- |
| Kiểm thử đơn vị (unit) | Kiểm tra query Athena, biểu đồ QuickSight, quyền người dùng |
| Kiểm thử tích hợp | Đảm bảo liên kết mượt mà giữa Glue – Athena – QuickSight |
| Kiểm thử hiệu năng | Đo thời gian tải dashboard, tốc độ query dưới 3 giây với SPICE |
| Kiểm thử bảo mật | Đảm bảo người dùng chỉ thấy được dữ liệu theo vai trò (RLS) |
| Kiểm thử UAT (người dùng chấp nhận) | Thực hiện với nhóm nhỏ end-user nội bộ trước khi triển khai đại trà |


4.3.3. Chiến lược kiểm thử cụ thể

| Loại kiểm thử | Công cụ/Giải pháp | Mục tiêu |
| --- | --- | --- |
| Unit Test | PyTest (cho script Athena query) | Đảm bảo câu lệnh SQL đúng logic |
| Integration Test | Postman / Insomnia + QuickSight Embed SDK | Kiểm thử tích hợp iframe, xác thực SSO |
| Load Test | Apache JMeter / Locust | Đo lường khả năng phản hồi của iframe embed |
| Security Test | IAM Policy Simulator, Cognito Token Check | Đảm bảo người dùng chỉ truy cập đúng dữ liệu |
| UAT (Acceptance) | Excel so sánh kết quả với dashboard | Đảm bảo độ chính xác, UX tốt với người dùng |


4.4. Kế hoạch triển khai và khôi phục

4.4.1. Kế hoạch triển khai

Triển khai theo từng dashboard: Không triển khai toàn bộ cùng lúc, tránh gián đoạn

Tài liệu hóa chi tiết: Checklist hướng dẫn cấu hình, kết nối và cách thêm người dùng mới

Đào tạo nhanh: Slide đào tạo + 1 video hướng dẫn sử dụng QuickSight

4.4.2. Kế hoạch khôi phục (Disaster Recovery)

| Tình huống lỗi | Giải pháp dự phòng |
| --- | --- |
| Dashboard không load được | Khôi phục phiên bản cũ đã lưu trong QuickSight hoặc cache SPICE |
| Glue ETL thất bại | Kiểm tra log CloudWatch, chạy lại thủ công bằng Glue console |
| Dữ liệu không đồng bộ | Thiết lập kiểm tra định kỳ → alert qua SNS → tự động re-crawl Glue |
| Mất quyền truy cập user | Thiết lập backup cấu hình Cognito và snapshot định kỳ quyền IAM |


4.5. Quản lý cấu hình

Sử dụng AWS CloudFormation để quản lý hạ tầng dưới dạng mã (IaC), đảm bảo có thể:

Tự động triển khai lại toàn bộ stack nếu cần

Quản lý version schema & dashboard dễ dàng hơn

Giảm sai sót do cấu hình thủ công

Ngoài ra, IAM policy, QuickSight group, và Cognito App Client cũng được ghi nhận trong file cấu hình lưu trữ nội bộ (hoặc dùng Terraform nếu mở rộng hạ tầng lớn).

CHƯƠNG 5. DÒNG THỜI GIAN & CÁC MỐC TRIỂN KHAI

5.1. Phân tích tổng thể giai đoạn dự án

Dự án “Nâng cao phân tích dữ liệu doanh nghiệp bằng Amazon QuickSight và trực quan hóa tùy chỉnh” được chia làm 5 giai đoạn chính, kéo dài trong khoảng 6 tuần. Mỗi giai đoạn bao gồm các đầu việc cụ thể, sản phẩm bàn giao (deliverables), và thời lượng dự kiến. Kế hoạch được xây dựng đảm bảo có thời gian đệm xử lý rủi ro và kiểm thử hệ thống.

| Giai đoạn | Thời gian | Nội dung chính | Deliverables chính |
| --- | --- | --- | --- |
| 1. Khởi động dự án | Tuần 1 (2 ngày) | Phân tích yêu cầu, thống nhất phạm vi, lên kiến trúc sơ bộ | Tài liệu yêu cầu, sơ đồ kiến trúc ban đầu |
| 2. Triển khai dữ liệu | Tuần 1–2 | Cấu hình S3, Glue, tạo crawler, chuẩn hóa dữ liệu đầu vào | S3 bucket, Glue Crawler, Glue Catalog, mẫu dữ liệu |
| 3. Phân tích và truy vấn | Tuần 2–3 | Thiết lập Athena, viết query, tạo view phân tích, chuẩn hóa schema | Athena view/table, script truy vấn mẫu |
| 4. Trực quan hóa & tích hợp | Tuần 4–5 | Xây dựng dashboard QuickSight, tích hợp iframe vào CRM | Dashboard mẫu, iframe tích hợp, RLS policy |
| 5. Kiểm thử & Đào tạo | Tuần 6 | Kiểm thử hiệu suất, bảo mật, hướng dẫn người dùng cuối | Báo cáo test, tài liệu hướng dẫn, demo cho stakeholder |


5.2. Lược đồ dòng thời gian Gantt

Tuần  | 1   | 2   | 3   | 4   | 5   | 6

------------------------------------------

G1   | ███ |

G2       | █████ |

G3           | ███ |

G4               | █████ |

G5                   | ███ |

G1 – Khởi động: Chuẩn bị tài liệu, phân quyền, khởi tạo môi trường

G2 – Dữ liệu: Thiết lập và kết nối nguồn dữ liệu

G3 – Athena: Truy vấn, tạo logic phân tích

G4 – QuickSight: Tạo dashboard và nhúng

G5 – Kiểm thử/Đào tạo: Đảm bảo vận hành và hỗ trợ người dùng

5.3. Các mốc quan trọng (Milestones)

| Mốc | Tuần | Tiêu chí thành công |
| --- | --- | --- |
| M1: Phê duyệt yêu cầu | Tuần 1 | Có tài liệu phân tích yêu cầu đã được duyệt, sơ đồ kiến trúc hoàn chỉnh |
| M2: Hoạt động Glue | Tuần 2 | Crawler thu được dữ liệu đúng schema từ S3, không lỗi |
| M3: Truy vấn thành công | Tuần 3 | Athena trả kết quả chính xác, nhanh < 3s với dữ liệu demo |
| M4: Dashboard hoàn thiện | Tuần 5 | Dashboard thể hiện đầy đủ biểu đồ và có thể lọc tương tác |
| M5: Kiểm thử đạt chuẩn | Tuần 6 | Kiểm thử thành công trên các vai trò người dùng, tài liệu hướng dẫn hoàn tất |


5.4. Phân tích đường dẫn quan trọng (Critical Path)

Các tác vụ trong đường dẫn quan trọng (phải hoàn thành đúng hạn):

Tạo Glue Crawler & Catalog 

Tạo bảng và query Athena 

Kết nối vào QuickSight 

Tạo dashboard 

Nhúng iframe vào CRM 

Kiểm thử bảo mật & phân quyền

Nếu bất kỳ khâu nào trong chuỗi trên bị trì hoãn, toàn bộ tiến độ triển khai sẽ bị ảnh hưởng. Do đó, ưu tiên tài nguyên và nhân lực cho những bước này là cần thiết.

5.5. Phân bổ nguồn lực

| Nhân sự | Vai trò | Thời gian phân bổ |
| --- | --- | --- |
| Kỹ sư dữ liệu | Thiết lập S3, Glue, chuẩn hóa dữ liệu | 50% toàn dự án |
| Kỹ sư phân tích (BI) | Tạo query, thiết kế dashboard | 70% tuần 2–5 |
| Kỹ sư AWS / DevOps | Cấu hình IAM, Athena, QuickSight, iframe | 60% tuần 1–4 |
| Kiểm thử & Đào tạo | Viết tài liệu hướng dẫn, kiểm thử hệ thống | 100% tuần 6 |
| Quản lý dự án | Giám sát tiến độ, kiểm tra milestone | 30% toàn bộ dự án |


5.6. Kế hoạch dự phòng và thời gian đệm

| Nguy cơ trì hoãn | Hướng xử lý |
| --- | --- |
| Chậm kết nối QuickSight | Dự phòng 2 ngày để xử lý IAM hoặc quota vùng AWS |
| Athena query chạy chậm | Chuẩn bị sẵn mẫu dữ liệu nhỏ hơn để demo tạm thời |
| Không thể tích hợp iframe | Dự phòng phương án mở dashboard QuickSight độc lập |
| RLS sai phân quyền | Có 1 buổi test trước với từng nhóm người dùng |
| Người dùng không hiểu dashboard | Tổ chức training session nội bộ, kèm theo video hướng dẫn |


CHƯƠNG 6. DỰ TOÁN NGÂN SÁCH

6.1. Mục tiêu ngân sách

Mục tiêu của dự toán ngân sách là xác định rõ các chi phí cần thiết để triển khai và duy trì giải pháp phân tích nâng cao với Amazon QuickSight và các dịch vụ AWS liên quan. Bản dự toán bao gồm:

Chi phí cơ sở hạ tầng AWS

Chi phí phát triển ban đầu

Chi phí hoạt động định kỳ

Chi phí đào tạo & hỗ trợ

Phân tích ROI (Return on Investment)

Chiến lược tối ưu hóa chi phí

6.2. Chi phí hạ tầng AWS (ước tính hàng tháng)

| Hạng mục | Dịch vụ AWS liên quan | Mức sử dụng dự kiến | Chi phí (USD/tháng) |
| --- | --- | --- | --- |
| Trực quan hóa dữ liệu | Amazon QuickSight Standard (5 users) | 5 người dùng x $9 | $45 |
| Truy vấn dữ liệu | Amazon Athena | ~50GB scan/tháng | $25 |
| Lưu trữ dữ liệu | Amazon S3 (dữ liệu đầu vào & logs) | 50GB dữ liệu phân tích | $3 |
| Metadata & ETL | AWS Glue Crawler + Data Catalog | 30 job/tháng | $15 |
| Quản lý người dùng | Amazon Cognito | <100 MAU | $0 (Free Tier) |
| Giám sát & logs | Amazon CloudWatch | Cảnh báo đơn giản + log query | $5 |


6.3. Chi phí phát triển ban đầu.

| Hạng mục | Mô tả | Ước tính (USD) |
| --- | --- | --- |
| Phân tích yêu cầu, thiết kế kiến trúc | Lập kế hoạch, sơ đồ, lựa chọn dịch vụ AWS | $300 |
| Phát triển ETL và cấu hình Glue | Tạo job crawl, ETL pipeline | $200 |
| Cấu hình Athena và chuẩn hóa dữ liệu | Viết query, cấu trúc schema truy vấn | $150 |
| Xây dựng dashboard QuickSight | Thiết kế biểu đồ, tạo dashboard | $200 |
| Tích hợp iframe vào CRM | Cấu hình embedding, user access | $100 |
| Đào tạo & kiểm thử người dùng | Hướng dẫn sử dụng, kiểm thử UAT | $50 |
| Tổng cộng chi phí ban đầu |  | ~$1,000 USD |


6.4. Chi phí hoạt động định kỳ (hàng năm)

| Khoản mục | Ước tính hàng tháng | Ước tính hàng năm |
| --- | --- | --- |
| AWS Services | ~$93 | ~$1,116 |
| Hỗ trợ kỹ thuật (0.2 FTE) | $50/tháng | $600 |
| Đào tạo bổ sung người dùng | $100/năm | $100 |
| Tổng cộng hàng năm |  | ~$1,816 USD |


6.5. Tính toán ROI & phân tích điểm hòa vốn

| Tiêu chí | Trước triển khai | Sau triển khai | Ghi chú |
| --- | --- | --- | --- |
| Thời gian tạo báo cáo | 2–3 ngày | <15 phút | Giảm chi phí nhân sự |
| Chi phí hệ thống BI cũ | ~$800/tháng | ~$93/tháng | Giảm ~88% |
| Nhân sự xử lý thủ công báo cáo | 1–2 người toàn thời gian | <0.2 FTE | Tiết kiệm $1,200+/tháng |
| Tăng khả năng tự phục vụ báo cáo | 0 → >80 người |  | Giảm chi phí đào tạo, IT support |
| ROI ước tính sau 3 tháng | — | ~62% | Nhờ giảm nhân sự và vận hành |


6.6. Chiến lược tối ưu hóa chi phí

| Chiến lược | Mô tả |
| --- | --- |
| Sử dụng QuickSight Standard | Giá chỉ $9/user/tháng, không cần phiên bản Enterprise |
| Chia sẻ dashboard qua iframe | Giảm số lượng license cần thiết |
| Athena truy vấn hiệu quả | Dùng partition và query tối ưu để giảm chi phí tính toán |
| Glue scheduler | Chạy job theo lịch thay vì liên tục |
| Log lưu trữ lifecycle trên S3 | Thiết lập tự động chuyển log sang lớp lưu trữ rẻ hơn |
| Sử dụng Free Tier | Tận dụng miễn phí của Cognito, CloudWatch, S3 (nếu nhỏ) |


6.7. Kết luận

Giải pháp phân tích dữ liệu với Amazon QuickSight không chỉ giúp doanh nghiệp giảm chi phí hệ thống BI truyền thống mà còn gia tăng hiệu suất, khả năng truy cập dữ liệu và tính sẵn sàng phân tích.

Với chi phí ban đầu hợp lý (~$1,000) và chi phí vận hành chỉ ~$93/tháng, giải pháp hoàn toàn khả thi cho các doanh nghiệp vừa và nhỏ đang muốn hiện đại hóa nền tảng phân tích mà không cần đầu tư hệ thống phức tạp.

CHƯƠNG 7: ĐÁNH GIÁ RỦI RO

7.1. Giới thiệu

Bất kỳ hệ thống công nghệ thông tin nào, đặc biệt là các hệ thống xử lý và phân tích dữ liệu trên đám mây như QuickSight và Athena, đều tiềm ẩn các rủi ro kỹ thuật, vận hành và kinh doanh. Mục tiêu của chương này là:

Chủ động xác định các rủi ro có thể xảy ra trong suốt vòng đời dự án

Đánh giá định lượng mức độ ảnh hưởng và khả năng xảy ra

Xây dựng kế hoạch ứng phó và giảm thiểu, bảo đảm hệ thống vận hành ổn định và an toàn

7.2. Phân loại rủi ro theo nhóm

7.2.1. Rủi ro kĩ thuật

| Rủi ro | Mô tả chi tiết | Tác động | Xác suất | Mức độ ưu tiên |
| --- | --- | --- | --- | --- |
| Cấu hình sai dịch vụ AWS | Việc thiết lập sai quyền IAM, kết nối S3-Athena-QuickSight hoặc Row-Level Security có thể gây lỗi dữ liệu | Cao (data leak, sai KPI) | Trung bình | Cao |
| Giới hạn tài nguyên AWS (quota) | AWS giới hạn số lượng truy vấn Athena, số lượng người dùng QuickSight nếu không mở rộng | Trung bình (ảnh hưởng báo cáo) | Trung bình | Trung bình |
| Không đồng bộ dữ liệu | Glue Crawler không cập nhật schema mới hoặc gặp lỗi xử lý | Cao (báo cáo sai, trắng dữ liệu) | Cao | Cao |
| Hiệu suất kém của dashboard | Dữ liệu lớn hoặc query phức tạp khiến dashboard tải chậm hoặc timeout | Cao (ảnh hưởng trải nghiệm người dùng) | Trung bình | Cao |
| Tích hợp nhúng iframe lỗi | Không tương thích với trình duyệt, hoặc không cấp quyền đúng khi nhúng vào CRM | Trung bình | Thấp | Trung bình |


7.2.2. Rủi ro vận hành

| Rủi ro | Mô tả | Tác động | Xác suất | Mức độ ưu tiên |
| --- | --- | --- | --- | --- |
| Nhân sự chủ chốt rời dự án | Dự án phụ thuộc vào 1–2 kỹ sư chính. Nếu họ nghỉ việc, kiến thức có thể không được chuyển giao | Cao | Thấp | Trung bình |
| Thiếu tài liệu hóa | Nếu thiếu tài liệu vận hành, việc bảo trì hoặc mở rộng sau này sẽ khó khăn | Trung bình | Cao | Cao |
| Dashboard bị chia sẻ sai quyền | Nhân viên phòng này xem được dữ liệu nhạy cảm của phòng khác | Cao (vi phạm bảo mật) | Thấp | Cao |


7.2.3. Rủi ro kinh doanh

| Rủi ro | Mô tả | Tác động | Xác suất | Mức độ ưu tiên |
| --- | --- | --- | --- | --- |
| Không có sự đồng thuận từ lãnh đạo | Không được duyệt ngân sách hoặc chuyển hướng chiến lược giữa chừng | Cao | Thấp | Trung bình |
| Người dùng không sử dụng hệ thống | Dashboard không thân thiện, người dùng vẫn phụ thuộc Excel | Trung bình | Trung bình | Trung bình |
| Thiếu ROI rõ ràng ban đầu | Không đo lường được giá trị sinh ra từ hệ thống | Trung bình | Trung bình | Trung bình |


7.3. Ma trận rủi ro tổng hợp

|  | Xác suất thấp | Xác suất trung bình | Xác suất cao |
| --- | --- | --- | --- |
| Tác động cao | Nhân sự rời dự án | Cấu hình sai, Dashboard chậm | Dữ liệu không đồng bộ |
| Tác động trung bình | Không được lãnh đạo duyệt | Giới hạn tài nguyên, iframe lỗi | — |
| Tác động thấp | — | Không sử dụng hệ thống, thiếu ROI | — |


7.4. Chiến lược giảm thiểu rủi ro

| Rủi ro | Chiến lược giảm thiểu cụ thể |
| --- | --- |
| Cấu hình sai dịch vụ AWS | - Tạo tài liệu cấu hình mẫu- Áp dụng AWS IAM theo Principle of Least Privilege- Kiểm thử từng bước tích hợp nhỏ |
| Không đồng bộ schema | - Thiết lập lịch Glue Crawler mỗi 6 giờ- Kết hợp kiểm tra log tự động bằng CloudWatch |
| Dashboard chậm | - Thiết kế dữ liệu dạng partition + limit- Dùng SPICE Engine (cache) của QuickSight |
| Tích hợp iframe lỗi | - Thử nghiệm trên nhiều trình duyệt- Cấu hình CSP (Content-Security-Policy) đúng cách |
| Nhân sự nghỉ việc | - Đảm bảo có người dự phòng, chuyển giao công việc định kỳ- Tài liệu hóa kỹ thuật rõ ràng |
| Người dùng không sử dụng | - Tổ chức các buổi training- Giao diện dashboard được thiết kế đơn giản, theo vai trò cụ thể |
| Thiếu ROI rõ ràng | - Đo lường KPI ngay từ đầu: thời gian tạo báo cáo, lỗi dữ liệu, số người dùng dashboard |


7.5. Kế hoạch dự phòng

| Tình huống | Phương án dự phòng |
| --- | --- |
| Athena timeout vì quota | Dùng Amazon Redshift Spectrum hoặc mở quota kịp thời |
| Dashboard sai dữ liệu | Duy trì dashboard backup mẫu và query kiểm thử định kỳ |
| Nhúng iframe lỗi | Dùng QuickSight Reader URL độc lập thay vì iframe |
| Người dùng từ chối dùng hệ thống mới | Cung cấp báo cáo dạng Excel tạm thời + hướng dẫn sử dụng dashboard từng bước |


7.6. Quy trình giám sát và phản ứng rủi ro

Công cụ & quy trình kiểm soát liên tục:

✅ Amazon CloudWatch Logs: giám sát truy vấn, crawler, lỗi hệ thống

✅ AWS Budgets: cảnh báo nếu vượt ngân sách

✅ Notion + Jira: theo dõi tất cả rủi ro mở và trạng thái xử lý

✅ Báo cáo hàng tuần: mỗi thứ Hai tổng hợp trạng thái rủi ro

✅ Họp định kỳ với quản lý dự án: cập nhật tình hình và xử lý nhanh

CHƯƠNG 8: KẾT QUẢ MONG ĐỢI

8.1. Giới thiệu

Việc triển khai giải pháp Nâng cao phân tích dữ liệu với Amazon QuickSight và trực quan hóa tùy chỉnh không chỉ là một sáng kiến kỹ thuật, mà còn mang lại giá trị chiến lược rõ rệt cho doanh nghiệp. Chương này trình bày chi tiết các chỉ số thành công (KPIs), lợi ích theo từng giai đoạn thời gian, và giá trị lâu dài, giúp đánh giá hiệu quả của hệ thống một cách cụ thể và định lượng.

8.2. Các chỉ số thành công (Success Metrics)

| Chỉ số | Mục tiêu cụ thể | Cơ sở đo lường |
| --- | --- | --- |
| Thời gian tạo báo cáo | < 15 phút | Thời gian từ truy vấn đến hiển thị dashboard |
| Độ chính xác dữ liệu | > 98% | So sánh giữa dữ liệu hệ thống BI và thực tế bán hàng |
| Khả năng sử dụng của người dùng | > 80% nhân viên có thể sử dụng dashboard | Tỷ lệ người dùng đăng nhập hàng tuần |
| Tần suất truy cập dashboard | Tăng > 30% so với hệ thống cũ | Lượt truy cập/tuần trên QuickSight |
| Tiết kiệm chi phí vận hành BI | Giảm ít nhất 40% so với hệ thống cũ | So sánh chi phí AWS vs hệ thống truyền thống |


8.3. Lợi ích ngắn hạn (0–6 tháng)

| Lĩnh vực | Lợi ích cụ thể |
| --- | --- |
| Vận hành | - Rút ngắn quy trình tạo báo cáo từ 2–3 ngày xuống còn vài phút- Giảm phụ thuộc vào IT trong việc tổng hợp dữ liệu |
| Người dùng | - Nhân viên có thể tự truy xuất số liệu theo thời gian thực- Dễ dàng trực quan hóa và chia sẻ kết quả phân tích |
| Quản lý | - Có cái nhìn tổng thể về hiệu suất bán hàng, chiến dịch marketing- Ra quyết định nhanh hơn dựa trên số liệu rõ ràng |


8.4. Lợi ích trung hạn (6–18 tháng)

| Lĩnh vực | Lợi ích cụ thể |
| --- | --- |
| Mở rộng hệ thống | - Thêm dữ liệu từ các nguồn khác: Ads, logistics, chăm sóc khách hàng- Phân tích nâng cao các chỉ số về hành vi khách hàng |
| Tăng năng suất | - Tự động hóa các báo cáo định kỳ (hằng tuần, hằng tháng)- Giảm áp lực cho bộ phận phân tích dữ liệu |
| Huấn luyện & đào tạo | - Tạo quy trình đào tạo nội bộ sử dụng QuickSight- Nâng cao năng lực data literacy cho nhân viên không chuyên kỹ thuật |


8.5. Giá trị dài hạn (18 tháng trở lên)

| Khía cạnh | Giá trị chiến lược đạt được |
| --- | --- |
| Năng lực phân tích | - Hình thành "văn hóa dữ liệu" trong toàn doanh nghiệp- Mỗi quyết định được hậu thuẫn bởi dữ liệu (data-driven decision making) |
| Khả năng mở rộng | - Dễ dàng tích hợp thêm các dịch vụ như ML (Amazon SageMaker), CDP (Customer Data Platform), hoặc Datalake |
| Lợi thế cạnh tranh | - Phản ứng nhanh hơn với thị trường- Nắm rõ hành vi khách hàng theo thời gian thực để điều chỉnh chiến lược nhanh chóng |
| Tuân thủ & bảo mật | - Kiểm soát truy cập chi tiết theo vai trò (RLS), bảo mật dữ liệu khách hàng- Sẵn sàng đáp ứng các tiêu chuẩn tuân thủ như GDPR, ISO 27001 |


8.6. Tác động đến trải nghiệm người dùng

Dashboard được thiết kế theo vai trò (role-based): Mỗi người chỉ thấy những gì liên quan đến họ (VD: Quản lý khu vực chỉ xem được số liệu khu vực mình)

Hiển thị trên đa thiết bị: Giao diện QuickSight tương thích tốt với desktop, tablet và smartphone

Thời gian phản hồi < 2 giây với dữ liệu đã được lưu trong SPICE cache

Hỗ trợ truy vấn ngôn ngữ tự nhiên (Natural Language Query) (nếu dùng phiên bản Enterprise)

8.7. Lợi ích đo lường theo phương pháp SMART

| Mục tiêu SMART | Chi tiết |
| --- | --- |
| S – Specific | Giảm chi phí BI, tăng khả năng sử dụng dashboard |
| M – Measurable | KPI cụ thể về thời gian báo cáo, truy cập, tỷ lệ sử dụng |
| A – Achievable | Đã có sẵn dịch vụ AWS, kỹ thuật viên được đào tạo |
| R – Relevant | Trực tiếp cải thiện năng lực vận hành và chiến lược |
| T – Time-bound | KPI chia theo từng mốc: 6 tháng, 18 tháng, dài hạn |


TÀI LIỆU THAM KHẢO

Amazon Web Services. (2024). Amazon QuickSight User Guide. Retrieved from https://docs.aws.amazon.com/quicksight/

Amazon Web Services. (2024). Embedding Amazon QuickSight dashboards. Retrieved from https://docs.aws.amazon.com/quicksight/latest/user/embedded-analytics.html

Amazon Web Services. (2024). AWS Glue Documentation. Retrieved from https://docs.aws.amazon.com/glue/

Amazon Web Services. (2024). Amazon Athena Documentation. Retrieved from https://docs.aws.amazon.com/athena/

Amazon Web Services. (2024). Amazon Simple Storage Service (Amazon S3). Retrieved from https://docs.aws.amazon.com/s3/

Amazon Web Services. (2024). Amazon Cognito Documentation. Retrieved from https://docs.aws.amazon.com/cognito/

Amazon Web Services. (2024). AWS Analytics Services Overview. Retrieved from https://aws.amazon.com/analytics/

Amazon Web Services. (2024). AWS Pricing Calculator. Retrieved from https://calculator.aws.amazon.com/

Amazon Web Services. (2024). AWS Security Best Practices – Well-Architected Framework. Retrieved from https://docs.aws.amazon.com/wellarchitected/latest/security-pillar/

Gartner. (2024). BI Trends: Cloud-First Business Intelligence Strategy. Gartner Research.

Forrester. (2023). The Forrester Wave™: Augmented BI Platforms, Q1 2023. Forrester Research Inc.

Nguyen, T. D. (2023). Implementing Serverless BI Architecture with AWS QuickSight and Glue. Medium. Retrieved from https://medium.com/tag/aws-glue

Pham, A. H. (2024). Building Real-Time Dashboards with Athena & QuickSight. Towards Data Science. Retrieved from https://towardsdatascience.com/

AWS Summit Online. (2024). Modern Analytics with Amazon QuickSight [Video]. YouTube. Retrieved from https://www.youtube.com/user/AmazonWebServices

IEEE Xplore. (2023). Cloud-Based Business Intelligence Systems: A Comparative Study. IEEE Access.

Google Scholar. (2023). Embedded Analytics and Cloud BI: Trends and Use Cases. Retrieved from https://scholar.google.com/

PHỤC LỤC

CHƯƠNG 1. TÓM TẮT NỘI DUNG2

1.1. Tổng quan dự án2

1.2. Giải pháp tổng thể2

1.3. Các tính năng chính của giải pháp2

1.4. Lợi ích kinh doanh và ROI3

1.5. Yêu cầu đầu tư và thời gian4

1.6. Kết quả mong đợi & chỉ số thành công4

CHƯƠNG 2. ĐẶT VẤN ĐỀ5

2.1. Phân tích tình hình hiện tại5

2.2. Xác định điểm đau & tác động định lượng5

2.2.1. Vận hành6

2.2.2. Kỹ thuật6

2.2.3. Kinh doanh7

2.3. Các bên liên quan và mối quan tâm7

2.4. Hậu quả nếu không hành động8

2.5. Cơ hội thị trường và động lực chuyển đổi9

CHƯƠNG 3. KIẾN TRÚC GIẢI PHÁP10

3.1. Mục tiêu và nguyên tắc thiết kế kiến trúc10

3.2. Mô hình tổng quan kiến trúc hệ thống12

3.3. Mô tả luồng dữ liệu chi tiết13

3.4. Giải thích lựa chọn dịch vụ AWS14

3.5. Kiến trúc bảo mật và tuân thủ15

3.6. Khả năng mở rộng & hiệu suất15

3.7. Tích hợp với hệ thống hiện tại16

3.8. Mở rộng tương lai16

CHƯƠNG 4. TRIỂN KHAI KỸ THUẬT18

4.1. Các giai đoạn triển khai18

4.2. Yêu cầu kỹ thuật18

4.2.1. Tài nguyên AWS18

4.2.2. Phần mềm bổ trợ19

4.3. Phương pháp phát triển và chiến lược kiểm thử19

4.3.1. Phương pháp phát triển19

4.3.2. Chiến lược kiểm thử20

4.3.3. Chiến lược kiểm thử cụ thể20

4.4. Kế hoạch triển khai và khôi phục21

4.4.1. Kế hoạch triển khai21

4.4.2. Kế hoạch khôi phục (Disaster Recovery)21

4.5. Quản lý cấu hình22

CHƯƠNG 5. DÒNG THỜI GIAN & CÁC MỐC TRIỂN KHAI23

5.1. Phân tích tổng thể giai đoạn dự án23

5.2. Lược đồ dòng thời gian Gantt24

5.3. Các mốc quan trọng (Milestones)24

5.4. Phân tích đường dẫn quan trọng (Critical Path)25

5.5. Phân bổ nguồn lực26

5.6. Kế hoạch dự phòng và thời gian đệm26

CHƯƠNG 6. DỰ TOÁN NGÂN SÁCH28

6.1. Mục tiêu ngân sách28

6.2. Chi phí hạ tầng AWS (ước tính hàng tháng)28

6.3. Chi phí phát triển ban đầu.29

6.4. Chi phí hoạt động định kỳ (hàng năm)30

6.5. Tính toán ROI & phân tích điểm hòa vốn30

6.6. Chiến lược tối ưu hóa chi phí31

6.7. Kết luận31

CHƯƠNG 7: ĐÁNH GIÁ RỦI RO33

7.1. Giới thiệu33

7.2. Phân loại rủi ro theo nhóm33

7.2.1. Rủi ro kĩ thuật33

7.2.2. Rủi ro vận hành35

7.2.3. Rủi ro kinh doanh36

7.3. Ma trận rủi ro tổng hợp36

7.4. Chiến lược giảm thiểu rủi ro37

7.5. Kế hoạch dự phòng38

7.6. Quy trình giám sát và phản ứng rủi ro39

CHƯƠNG 8: KẾT QUẢ MONG ĐỢI40

8.1. Giới thiệu40

8.2. Các chỉ số thành công (Success Metrics)40

8.3. Lợi ích ngắn hạn (0–6 tháng)41

8.4. Lợi ích trung hạn (6–18 tháng)41

8.5. Giá trị dài hạn (18 tháng trở lên)42

8.6. Tác động đến trải nghiệm người dùng43

8.7. Lợi ích đo lường theo phương pháp SMART43

TÀI LIỆU THAM KHẢO44

PHỤC LỤC46