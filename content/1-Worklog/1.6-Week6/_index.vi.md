---
title: "Tuần 6: Tự động duyệt hồ sơ & sinh hợp đồng"
date: 2026-07-10
weight: 6
chapter: false
---

## Tuần 6: Tự động hóa quy trình duyệt hồ sơ và sinh hợp đồng

### Nhật ký công việc theo ngày

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| ---- | ---- | ---- | ---- | ---- |
| 2 | Xây dựng API cho phép Admin duyệt (`APPROVED`) hoặc từ chối (`REJECTED`) một đơn đăng ký thuê phòng. | 25/05/2026 | 25/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 3 | Viết logic: khi đơn được duyệt, hệ thống tự sinh bản ghi `Contract` mới và cập nhật trạng thái phòng sang `OCCUPIED`. | 26/05/2026 | 26/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 4 | Bọc toàn bộ thao tác trên trong một transaction để đảm bảo không xảy ra tình trạng phòng bị "duyệt trùng" cho hai sinh viên khác nhau. | 27/05/2026 | 27/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 5 | Viết thêm cơ chế kiểm tra race-condition đơn giản: kiểm tra lại trạng thái phòng ngay trong transaction trước khi duyệt. | 28/05/2026 | 28/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 6 | Viết API `PUT /api/requests/{id}/reject`, cập nhật trạng thái và lưu lý do từ chối do Admin nhập. | 29/05/2026 | 29/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 7 | Viết vài Integration Test mô phỏng 2 request duyệt cùng lúc cho 1 phòng để kiểm tra transaction hoạt động đúng. | 30/05/2026 | 31/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Kết quả đạt được
*   Luồng duyệt - sinh hợp đồng - cập nhật trạng thái phòng chạy chính xác trong mọi kịch bản đã test.
*   Không còn xảy ra tình trạng dữ liệu không nhất quán giữa `TenantRequests`, `Contracts` và `Rooms`.
