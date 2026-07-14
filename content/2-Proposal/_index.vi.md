---
title: "Đề xuất dự án"
date: 2026-07-10
weight: 3
chapter: false
pre: " <b> 2. </b> "
---

## SmartDorm — Đề xuất xây dựng hệ thống quản lý ký túc xá

### Bối cảnh & lý do chọn đề tài
Trong quá trình tìm hiểu thực tế, tôi nhận thấy việc quản lý phòng trọ, ký túc xá tại nhiều nơi vẫn đang dựa vào sổ sách giấy tờ hoặc file Excel rời rạc: ghi chỉ số điện nước bằng tay, lưu hợp đồng bằng bản in, nhắc thanh toán qua tin nhắn cá nhân. Cách làm này dễ thất lạc dữ liệu, tốn thời gian đối chiếu và khó mở rộng khi số lượng phòng tăng lên. Từ đó tôi đề xuất xây dựng **SmartDorm**, tập trung giải quyết bài toán này bằng một Backend vững chắc chạy trên AWS, còn phần giao diện tôi chỉ tham gia hỗ trợ ở mức cơ bản cùng một bạn khác trong nhóm.

### Phạm vi công việc của tôi trong dự án
*   Thiết kế và xây dựng toàn bộ **Backend API** bằng ASP.NET Core: quản lý phòng, hồ sơ đăng ký, hợp đồng, hóa đơn điện nước.
*   Thiết kế cơ sở dữ liệu quan hệ trên PostgreSQL và triển khai chính thức lên Amazon RDS.
*   Viết hạ tầng bằng Terraform (Infrastructure as Code) và triển khai Backend theo mô hình serverless trên AWS Lambda.
*   Hỗ trợ ở mức cơ bản cho phần giao diện: cung cấp tài liệu API, ví dụ gọi API mẫu, và cùng kiểm thử luồng nghiệp vụ khi frontend đã sẵn sàng.

### Bài toán cần giải quyết
*   Ghi chép chỉ số điện, nước thủ công dễ sai lệch và khó tổng hợp cuối tháng.
*   Không có nơi lưu trữ tập trung cho hồ sơ sinh viên và hợp đồng thuê phòng.
*   Việc duy trì một máy chủ chạy 24/7 chỉ để phục vụ vài chục request mỗi ngày là lãng phí chi phí không cần thiết.

### Hướng giải pháp kỹ thuật (AWS)
Tôi lựa chọn kiến trúc serverless để tối ưu chi phí vận hành trong giai đoạn thử nghiệm:
*   **AWS Lambda** chạy Backend ASP.NET Core, chỉ tính phí theo lượt gọi thực tế thay vì phí giờ máy chủ cố định.
*   **Amazon API Gateway (HTTP API)** làm cổng vào cho toàn bộ request từ client.
*   **Amazon RDS PostgreSQL** lưu trữ dữ liệu quan hệ, chọn instance tối ưu chi phí phù hợp Free Tier.
*   **Amazon S3** lưu ảnh đại diện, ảnh CCCD do người dùng tải lên, đồng thời cũng là nơi chứa mã tĩnh của phần giao diện demo.

### Kế hoạch triển khai theo 3 giai đoạn
*   **Giai đoạn 1 (Tuần 1-4):** Ôn tập nền tảng AWS, thiết kế ERD, dựng khung Backend và kết nối database local.
*   **Giai đoạn 2 (Tuần 5-9):** Phát triển đầy đủ các API nghiệp vụ (phòng, hồ sơ, hợp đồng, hóa đơn), bổ sung xác thực JWT, phối hợp cùng bạn phụ trách giao diện để có bản demo cơ bản.
*   **Giai đoạn 3 (Tuần 10-12):** Viết hạ tầng Terraform, deploy Backend lên môi trường serverless thật, chuyển việc lưu file sang S3 và hoàn thiện tài liệu bàn giao.

### Rủi ro đã lường trước
*   **Lambda không ghi được file cục bộ:** do hệ thống tệp chỉ đọc, tôi đã dự trù trước phương án chuyển hẳn sang S3 thay vì lưu local ngay từ đầu.
*   **Lỗi CORS khi frontend và backend khác domain:** cấu hình rõ policy CORS ở cả tầng ứng dụng lẫn API Gateway để tránh phát sinh giữa chừng.
