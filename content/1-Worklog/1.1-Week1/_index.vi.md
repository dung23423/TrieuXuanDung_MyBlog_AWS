---
title: "Tuần 1: Làm quen chương trình & nền tảng AWS"
date: 2026-07-10
weight: 1
chapter: false
---

## Tuần 1: Làm quen chương trình thực tập & Nền tảng điện toán đám mây AWS

### Mục tiêu
* Làm quen với mentor, các bạn thực tập sinh và quy trình làm việc của chương trình FCJ.
* Xây dựng nền tảng kiến thức về điện toán đám mây và các dịch vụ cốt lõi của AWS.
* Thực hành thao tác cơ bản với máy chủ ảo EC2 qua Console và CLI.

### Nhật ký công việc theo ngày

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| ---- | ---- | ---- | ---- | ---- |
| 2 | Tham gia buổi kickoff chương trình, giới thiệu bản thân với mentor và nhóm. Nắm lịch trình 12 tuần và cách báo cáo tiến độ hàng tuần. | 17/04/2026 | 18/04/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 3 | Đọc tài liệu tổng quan Cloud Computing: mô hình IaaS/PaaS/SaaS, lợi ích so với hạ tầng vật lý truyền thống. | 21/04/2026 | 21/04/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 4 | Đăng ký tài khoản AWS Free Tier, bật MFA cho tài khoản root, tạo IAM User riêng để không dùng root cho công việc hàng ngày. | 22/04/2026 | 22/04/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 5 | Cài AWS CLI v2 trên máy cá nhân, chạy `aws configure` và thử một số lệnh liệt kê tài nguyên (`aws ec2 describe-instances`). | 23/04/2026 | 23/04/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 6 | Thực hành tạo EC2 instance Ubuntu, cấu hình Security Group, tạo Key Pair và SSH vào máy chủ để kiểm tra kết nối. | 24/04/2026 | 25/04/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| 7 | Ghi chú lại các lệnh CLI đã dùng trong tuần, tự tổng hợp thành file cheat-sheet cá nhân để tra cứu nhanh. | 25/04/2026 | 26/04/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Kết quả đạt được
* Hiểu được vai trò của Managed Service trên AWS và lý do doanh nghiệp chuyển dịch lên cloud.
* Tài khoản AWS Free Tier và IAM User cá nhân đã sẵn sàng, có thiết lập cảnh báo ngân sách để tránh phát sinh chi phí ngoài ý muốn.
* Có thể tự khởi tạo, kết nối và tắt một EC2 instance thông qua cả Console lẫn CLI.
