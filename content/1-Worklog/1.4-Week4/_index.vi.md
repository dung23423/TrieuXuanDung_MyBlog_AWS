---
title: "Tuần 4: Dựng khung Backend ASP.NET Core"
date: 2026-07-10
weight: 4
chapter: false
---

## Tuần 4: Dựng khung Backend với ASP.NET Core và PostgreSQL

### Nhật ký công việc theo ngày

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| ---- | ---- | ---- | ---- | ---- |
| 2 | Khởi tạo project Web API bằng ASP.NET Core (.NET 10) với `dotnet new webapi`. | 11/05/2026 | 11/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 3 | Tự tổ chức lại cấu trúc thư mục theo hướng phân lớp: `Controllers`, `Entities`, `DTOs`, `Services`, `Repositories`, giúp code dễ maintain hơn khi dự án lớn dần. | 12/05/2026 | 12/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 4 | Dựng PostgreSQL bằng Docker Compose để chạy local, không cần cài đặt trực tiếp lên máy. | 13/05/2026 | 13/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 5 | Gặp lỗi kết nối do container Docker PostgreSQL chưa mở đúng port ra ngoài, khắc phục bằng cách kiểm tra lại `docker-compose.yml` và mapping port `5432:5432`. | 14/05/2026 | 14/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 6 | Cài `Npgsql.EntityFrameworkCore.PostgreSQL`, viết `DbContext` ánh xạ 6 thực thể đã thiết kế ở tuần 3. | 15/05/2026 | 15/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 7 | Chạy migration đầu tiên, kiểm tra bảng được tạo đúng trong PostgreSQL bằng DBeaver, bật Swagger UI để tự kiểm tra API. | 16/05/2026 | 17/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Kết quả đạt được
*   Backend chạy được, kết nối ổn định tới PostgreSQL local qua Docker.
*   Toàn bộ 6 bảng dữ liệu được migrate thành công, khớp với ERD.
*   Bật Swagger UI để tự kiểm tra API ngay trong lúc code, chưa cần công cụ ngoài như Postman.
