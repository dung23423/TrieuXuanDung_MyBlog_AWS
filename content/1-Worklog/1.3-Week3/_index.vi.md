---
title: "Tuần 3: Khởi động SmartDorm & mô hình dữ liệu"
date: 2026-07-10
weight: 3
chapter: false
---

## Tuần 3: Lên ý tưởng dự án SmartDorm và mô hình hóa dữ liệu

### Nhật ký công việc theo ngày

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| ---- | ---- | ---- | ---- | ---- |
| 2 | Đề xuất dự án cá nhân **SmartDorm** — hệ thống hỗ trợ ban quản lý ký túc xá theo dõi phòng ở, hồ sơ sinh viên, hợp đồng thuê và chi phí điện nước hàng tháng. | 04/05/2026 | 04/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 3 | Trao đổi với mentor để chốt phạm vi (scope) phù hợp trong 12 tuần, ưu tiên xây dựng phần Backend vững chắc trước, giao diện chỉ làm ở mức demo tối thiểu. | 05/05/2026 | 05/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 4 | Vẽ sơ đồ thực thể - quan hệ (ERD) trên draw.io, xác định 6 thực thể chính: `Room`, `Tenant`, `Contract`, `Invoice`, `UtilityUsage`, `Maintenance`. | 06/05/2026 | 07/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 5 | Thiết kế chi tiết từng bảng: `Room` (mã phòng, sức chứa, đơn giá, trạng thái), `Tenant` (thông tin cá nhân, CCCD), `Contract` (liên kết Room - Tenant, ngày bắt đầu/kết thúc). | 07/05/2026 | 08/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 6 | Tách riêng `Invoice` và `UtilityUsage` để dễ mở rộng; đặt chỗ thực thể `Maintenance` trong ERD để triển khai chi tiết sau. | 08/05/2026 | 08/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 7 | Tạo repository GitHub, thống nhất quy ước đặt tên nhánh (`feature/`, `fix/`), cấu trúc thư mục dự án và cài đặt môi trường code local (VS Code, .NET SDK, Docker). | 09/05/2026 | 10/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Kết quả đạt được
*   Có bản ERD hoàn chỉnh, được mentor review và góp ý điều chỉnh khóa ngoại giữa `Contract` và `Invoice`.
*   Repository dự án đã sẵn sàng, môi trường code local cài đặt xong để bắt đầu code từ tuần 4.
