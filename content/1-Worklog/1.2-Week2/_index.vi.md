---
title: "Tuần 2: Mạng riêng ảo VPC & lưu trữ S3"
date: 2026-07-10
weight: 2
chapter: false
---

## Tuần 2: Thực hành mạng riêng ảo VPC và lưu trữ đối tượng S3

### Mục tiêu
* Hiểu cách thiết kế một mạng riêng ảo an toàn trên AWS.
* Làm quen với dịch vụ lưu trữ đối tượng S3 và cách quản lý quyền truy cập bằng IAM.

### Nhật ký công việc theo ngày

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| ---- | ---- | ---- | ---- | ---- |
| 2 | Tìm hiểu khái niệm CIDR, Subnet public/private, Internet Gateway, NAT Gateway, Route Table trong VPC. | 27/04/2026 | 27/04/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 3 | Tự tay dựng một VPC gồm 1 subnet public và 1 subnet private, kiểm tra máy trong subnet private không truy cập Internet trực tiếp được. | 28/04/2026 | 28/04/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 4 | Tìm hiểu S3: khái niệm Bucket, Object, Storage Class, Versioning. Tạo bucket thử nghiệm, upload/xóa object qua Console và CLI. | 29/04/2026 | 29/04/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 5 | Đọc về IAM Policy dạng JSON, thử viết một policy tùy chỉnh chỉ cho phép đọc (GetObject) trên một bucket cụ thể. | 30/04/2026 | 30/04/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 6 | Gắn policy vừa viết cho IAM User thử nghiệm, kiểm tra thực tế quyền bị giới hạn đúng như mong đợi (không xóa/upload được). | 01/05/2026 | 01/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 7 | Tổng hợp lại kiến thức 2 tuần đầu, phác thảo sơ bộ ý tưởng dự án cá nhân sẽ làm ở tuần 3. | 02/05/2026 | 03/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Kết quả đạt được
* Dựng thành công một mô hình VPC cơ bản với subnet công khai và riêng tư tách biệt.
* Thao tác thành thạo với S3: tạo bucket, upload, phân quyền, hiểu sự khác biệt giữa quyền ở cấp Bucket Policy và IAM Policy.
* Viết được IAM Policy tùy chỉnh theo đúng nguyên tắc cấp quyền tối thiểu cần thiết.
