---
title: "Tuần 10: Terraform & RDS PostgreSQL"
date: 2026-07-10
weight: 10
chapter: false
---

## Tuần 10: Hạ tầng dưới dạng mã với Terraform và RDS

### Nhật ký công việc theo ngày

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| ---- | ---- | ---- | ---- | ---- |
| 2 | Học và thực hành Terraform: `provider`, `resource`, `variable`, `output`, `state file`. | 22/06/2026 | 22/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 3 | Viết mã Terraform định nghĩa VPC, Subnet, Internet Gateway, Route Table và Security Group riêng cho môi trường triển khai dự án. | 23/06/2026 | 23/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 4 | Khởi tạo Amazon RDS PostgreSQL bằng Terraform, chọn instance `db.t4g.micro` để tận dụng Free Tier. | 24/06/2026 | 24/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 5 | Gặp lỗi thiếu quyền IAM khi chạy `terraform apply`, bổ sung policy `AmazonRDSFullAccess` và `AmazonVPCFullAccess` tạm thời cho user thực hành. | 25/06/2026 | 25/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 6 | Bổ sung Security Group rule cho phép kết nối từ IP cá nhân tới RDS sau khi phát hiện không connect được từ máy local. | 26/06/2026 | 26/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 7 | Tổ chức lại mã nguồn Terraform theo module (`network`, `database`) để dễ tái sử dụng cho các tài nguyên khác ở tuần sau. | 27/06/2026 | 28/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Kết quả đạt được
*   RDS PostgreSQL chạy ổn định trên AWS, Backend local kết nối thành công.
*   Có thể tái tạo toàn bộ hạ tầng chỉ bằng `terraform apply` và dọn dẹp bằng `terraform destroy`.
