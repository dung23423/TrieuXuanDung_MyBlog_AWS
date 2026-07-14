---
title: "Tuần 9: Xác thực JWT & kiểm thử liên kết hệ thống"
date: 2026-07-10
weight: 9
chapter: false
---

## Tuần 9: Bảo mật xác thực JWT và kiểm thử liên kết hệ thống

### Nhật ký công việc theo ngày

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| ---- | ---- | ---- | ---- | ---- |
| 2 | Tích hợp JWT Authentication cho Backend: viết API `POST /api/auth/login`, sinh Access Token chứa claim `UserId` và `Role`. | 15/06/2026 | 15/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 3 | Cấu hình `[Authorize(Roles = "Admin")]` cho các API quản trị (thêm/sửa/xóa phòng, duyệt hồ sơ) để chỉ Admin mới gọi được. | 16/06/2026 | 16/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 4 | Viết ví dụ đoạn code gọi API login bằng `fetch` để hỗ trợ bạn phụ trách giao diện áp dụng vào frontend. | 17/06/2026 | 17/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 5 | Giải thích cách gắn token vào header `Authorization: Bearer <token>` cho các request cần xác thực. | 18/06/2026 | 18/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 6 | Cùng nhóm kiểm thử luồng đăng nhập - gọi API được bảo vệ từ đầu đến cuối. | 19/06/2026 | 19/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 7 | Test token hết hạn/token giả để xác nhận API trả về đúng mã lỗi 401. | 20/06/2026 | 21/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Kết quả đạt được
*   Toàn bộ API nhạy cảm được bảo vệ đúng theo Role.
*   Xác nhận luồng đăng nhập hoạt động ổn định khi tích hợp với giao diện của nhóm.
