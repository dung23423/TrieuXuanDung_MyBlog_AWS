---
title: "Tuần 11: Triển khai serverless với Lambda"
date: 2026-07-10
weight: 11
chapter: false
---

## Tuần 11: Triển khai serverless với AWS Lambda

### Nhật ký công việc theo ngày

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| ---- | ---- | ---- | ---- | ---- |
| 2 | Tìm hiểu package `Amazon.Lambda.AspNetCoreServer` để chuyển ứng dụng ASP.NET Core sang chạy được trên AWS Lambda. | 29/06/2026 | 29/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 3 | Đóng gói Backend thành file zip theo đúng cấu trúc AWS Lambda yêu cầu, upload lên S3. | 30/06/2026 | 30/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 4 | Tạo Lambda Function từ file zip, kết nối Lambda với API Gateway (loại HTTP API v2). | 01/07/2026 | 01/07/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 5 | Gặp lỗi CORS khi thử gọi API từ giao diện demo, cấu hình `AddCors` trong `Program.cs` để xử lý. | 02/07/2026 | 02/07/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 6 | Khai báo policy CORS tương ứng ở API Gateway để xử lý dứt điểm lỗi cross-origin. | 03/07/2026 | 03/07/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 7 | Cập nhật lại mã Terraform ở tuần 10 để tự động hóa việc tạo Lambda Function và API Gateway. | 04/07/2026 | 05/07/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Kết quả đạt được
*   Backend chạy ổn định trên môi trường serverless, không còn cần duy trì EC2 chạy 24/7.
*   Lỗi CORS được giải quyết hoàn toàn.
