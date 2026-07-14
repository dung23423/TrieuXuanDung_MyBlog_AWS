---
title: "Tuần 7: Module tính tiền điện nước & hóa đơn"
date: 2026-07-10
weight: 7
chapter: false
---

## Tuần 7: Xây dựng module tính tiền điện nước và hóa đơn

### Nhật ký công việc theo ngày

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| ---- | ---- | ---- | ---- | ---- |
| 2 | Thiết kế bảng `UtilityUsage` lưu chỉ số điện, nước đầu kỳ và cuối kỳ theo từng phòng, từng tháng. | 01/06/2026 | 01/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 3 | Viết Service tính tiền: tiền điện, tiền nước theo đơn giá cấu hình sẵn, cộng thêm tiền phòng và phí dịch vụ để ra tổng hóa đơn. | 02/06/2026 | 02/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 4 | Xây dựng API `POST /api/invoices/generate` chạy theo lô (batch), tự động tạo hóa đơn cho toàn bộ phòng đang có người ở trong tháng. | 03/06/2026 | 03/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 5 | Phát hiện lỗi: quên xử lý trường hợp chỉ số cuối kỳ nhỏ hơn đầu kỳ dẫn tới tiền điện âm, bổ sung validate chặn trường hợp này. | 04/06/2026 | 04/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 6 | Viết Unit Test riêng cho phần tính toán số tiền, dùng nhiều bộ dữ liệu khác nhau để đảm bảo công thức không bị sai khi đơn giá thay đổi. | 05/06/2026 | 05/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 7 | Chạy thử API lập hóa đơn trên bộ dữ liệu thử nghiệm gồm 10 phòng có mức tiêu thụ khác nhau. | 06/06/2026 | 07/06/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Kết quả đạt được
*   API lập hóa đơn tự động chạy đúng trên bộ dữ liệu thử nghiệm.
*   Bộ Unit Test cho phần tính toán đạt 100% pass.
