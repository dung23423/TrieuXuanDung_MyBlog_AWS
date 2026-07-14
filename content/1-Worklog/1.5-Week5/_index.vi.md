---
title: "Tuần 5: API quản lý phòng & đơn thuê"
date: 2026-07-10
weight: 5
chapter: false
---

## Tuần 5: Phát triển API quản lý phòng trọ và đơn đăng ký thuê

### Nhật ký công việc theo ngày

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| ---- | ---- | ---- | ---- | ---- |
| 2 | Xây dựng nhóm API `/api/rooms`: thêm, sửa, xóa, tìm kiếm phòng theo trạng thái và mức giá. | 18/05/2026 | 18/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 3 | Xây dựng API `/api/requests` để sinh viên gửi đơn đăng ký thuê phòng, gồm thông tin cá nhân và phòng mong muốn. | 19/05/2026 | 19/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 4 | Viết các lớp validator riêng (FluentValidation) thay vì validate thủ công trong Controller, giúp code sạch hơn. | 20/05/2026 | 20/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 5 | Áp dụng DTO (Data Transfer Object) để tách biệt dữ liệu trả về API với Entity trong database, tránh lộ thông tin nhạy cảm không cần thiết. | 21/05/2026 | 21/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 6 | Học cách viết custom validation rule bằng FluentValidation, ví dụ kiểm tra định dạng số điện thoại Việt Nam bằng regex. | 22/05/2026 | 22/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 7 | Test thủ công toàn bộ API qua Swagger với hơn 15 trường hợp khác nhau (dữ liệu hợp lệ/không hợp lệ). | 23/05/2026 | 24/05/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Kết quả đạt được
*   Bộ API quản lý phòng và tiếp nhận đơn hoạt động ổn định.
*   Học được cách viết custom validation rule bằng FluentValidation.
