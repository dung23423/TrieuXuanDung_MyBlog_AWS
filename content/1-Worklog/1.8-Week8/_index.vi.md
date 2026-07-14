---
title: "Tuần 8: API tải file & hỗ trợ giao diện demo"
date: 2026-07-10
weight: 8
chapter: false
---

## Tuần 8: API tải file & hỗ trợ dựng giao diện demo

### Nhật ký công việc theo ngày

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| ---- | ---- | ---- | ---- | ---- |
| 2 | Xây dựng API cho phép tải lên ảnh đại diện và ảnh CCCD của sinh viên, lưu tạm vào thư mục `wwwroot/uploads` của Backend. | 08/06/2026 | 08/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 3 | Viết logic kiểm tra định dạng file (chỉ nhận `.jpg`, `.png`), giới hạn dung lượng tối đa 5MB. | 09/06/2026 | 09/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 4 | Sinh tên file bằng GUID để tránh trùng lặp/ghi đè, hoàn thiện API upload. | 10/06/2026 | 10/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 5 | Dành khoảng 1 buổi hỗ trợ nhóm dựng 2 trang giao diện demo đơn giản (trang chủ và trang gửi đơn thuê phòng) bằng HTML/CSS thuần — phần này không phải trọng tâm công việc, làm ở mức cơ bản nhất. | 11/06/2026 | 11/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 6 | Gọi thử API `/api/requests` từ trang demo bằng `fetch()` để xác nhận dữ liệu gửi lên đúng định dạng backend mong đợi. | 12/06/2026 | 12/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 7 | Kiểm thử API upload với nhiều loại file (đúng định dạng, sai định dạng, vượt dung lượng), xác nhận đều trả lỗi phù hợp. | 13/06/2026 | 14/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Kết quả đạt được
*   API upload file hoạt động ổn định.
*   Có bản demo giao diện tối giản đủ dùng để kiểm thử luồng gửi đơn đăng ký end-to-end, giúp phát hiện một lỗi nhỏ ở phía API validate ngày sinh.
