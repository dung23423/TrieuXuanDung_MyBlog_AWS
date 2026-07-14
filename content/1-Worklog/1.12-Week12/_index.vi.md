---
title: "Tuần 12: Lưu trữ S3 & tổng kết dự án"
date: 2026-07-10
weight: 12
chapter: false
---

## Tuần 12: Lưu trữ tệp trên S3 và tổng kết dự án

### Nhật ký công việc theo ngày

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| ---- | ---- | ---- | ---- | ---- |
| 2 | Phát hiện AWS Lambda có hệ thống tệp chỉ đọc (trừ `/tmp`), cách lưu file cục bộ ở tuần 8 không dùng được trên serverless. | 06/07/2026 | 06/07/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 3 | Chuyển toàn bộ logic upload sang dùng AWS SDK for S3, ảnh được đẩy thẳng lên S3 Bucket. | 07/07/2026 | 07/07/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 4 | Cấu hình IAM Policy cho phép Lambda ghi vào đúng bucket cần thiết, khai báo qua Terraform. | 08/07/2026 | 08/07/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 5 | Kiểm thử lại toàn bộ luồng nghiệp vụ chính từ đầu đến cuối trên môi trường đã deploy. | 09/07/2026 | 09/07/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 6 | Hỗ trợ nhóm hoàn thiện việc đưa giao diện demo lên hosting (Vercel), xác nhận giao diện gọi đúng API Backend đã deploy trên Lambda. | 10/07/2026 | 10/07/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 7 | Viết lại tài liệu Swagger/README tổng hợp toàn bộ endpoint đã xây dựng trong 12 tuần. | 11/07/2026 | 12/07/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Kết quả đạt được
*   Chức năng upload ảnh hoạt động ổn định trên môi trường serverless kết hợp S3.
*   Toàn bộ luồng nghiệp vụ chính của SmartDorm hoạt động thông suốt trên môi trường đã deploy thật.
*   Có bộ tài liệu API đầy đủ, thuận tiện cho việc bàn giao hoặc mở rộng dự án sau này.

### Nhìn lại 12 tuần
Sau 12 tuần, tôi tự tin hơn nhiều với việc thiết kế và xây dựng một Backend hoàn chỉnh bằng ASP.NET Core, quản lý hạ tầng AWS bằng Terraform, và vận hành ứng dụng theo mô hình serverless. Phần frontend tôi chỉ tham gia hỗ trợ ở mức cơ bản, nhưng qua đó cũng hiểu rõ hơn cách hai phía Backend - Frontend cần phối hợp với nhau về định dạng dữ liệu và xác thực.
