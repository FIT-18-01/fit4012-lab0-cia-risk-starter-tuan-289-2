# Lab 01 Answers
## CIA & Risk: Hệ thống lưu điểm

**Họ và tên:** Nguyễn Anh Tuấn

**MSSV:** 1871020623

**Lớp/Nhóm:** CNTT18-01

---

## 1. Assets
Liệt kê ít nhất 2 assets cần bảo vệ.

- Asset 1: Dữ liệu điểm số của sinh viên (Grade Database)
- Asset 2: Tính sẵn sàng của hệ thống (System Availability/Uptime)
- Asset 3 (nếu có): Tài khoản người dùng (học sinh, giảng viên) và thông tin xác thực

---

## 2. Mapping CIA
Ghép từng sự cố với CIA.

- Sự cố A -> A (Availability)
- Sự cố B -> I (Integrity)
- Sự cố C -> C (Confidentiality)

---

## 3. Phân tích sự cố B
- Threat: Một kẻ tấn công hoặc người dùng có quyền truy cập vào hệ thống cơ sở dữ liệu/tài khoản quản trị viên có khả năng thay đổi điểm số của sinh viên mà không có sự phê duyệt.
- Vulnerability: Hệ thống thiếu cơ chế kiểm soát truy cập (Access Control), không có hệ thống đăng nhập kiểm toán (Audit Logging) để theo dõi các thay đổi, xác thực không đủ mạnh, và không có quy trình xác nhận thay đổi điểm.
- Mitigation: Triển khai kiểm soát truy cập dựa trên vai trò (RBAC), ghi lại tất cả các thay đổi điểm với thời gian và người thực hiện, yêu cầu xác thực đa yếu tố (MFA), và tạo quy trình phê duyệt hai cấp cho các thay đổi điểm số.

---

## 4. Reflection
Nếu tôi là quản trị viên hệ thống, tôi sẽ ưu tiên xử lý sự cố B (thay đổi điểm không hợp lệ) trước tiên. Vì dù sự cố A (không đăng nhập được) ảnh hưởng đến tính sẵn sàng, nhưng B ảnh hưởng trực tiếp đến tính toàn vẹn dữ liệu - một yếu tố quan trọng hơn. Việc thay đổi điểm có thể ảnh hưởng vĩnh viễn đến hồ sơ học tập của sinh viên, ảnh hưởng đến kết quả học tập, xét học bổng, xin việc... Đó là lý do B cần được ưu tiên để ngăn chặn thiệt hại phát sinh thêm, kết hợp với việc điều tra nguồn gốc cuộc tấn công.



---

## 5. Bonus Flag
`FIT4012{A-A-B-I-C-C}`

Flag của em: FIT4012{A-A-B-I-C-C}

