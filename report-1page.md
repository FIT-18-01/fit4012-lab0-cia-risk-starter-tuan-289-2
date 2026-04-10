# FIT4012 - Report 1 Page
## Lab 01 - CIA & Risk: Hệ thống lưu điểm

### 1. Mục tiêu bài lab
- Nhận diện tài sản cần bảo vệ trong một hệ thống thông tin đơn giản.
- Phân biệt Confidentiality, Integrity, Availability.
- Xác định threat, vulnerability, mitigation.
- Thực hành workflow GitHub cơ bản để nhận và nộp bài.

### 2. Cách làm
- Đọc bối cảnh và xác định các thành phần quan trọng của hệ thống.
- Phân tích từng sự cố theo bộ ba CIA.
- Chọn sự cố B để phân tích sâu hơn theo threat - vulnerability - mitigation.
- Hoàn thiện bài làm trong repo và commit/push lên GitHub.

### 3. Kết quả chính
**Assets:**
- Dữ liệu điểm số của sinh viên (Grade Database)
- Tính sẵn sàng của hệ thống (System Availability/Uptime)

**CIA mapping:**
- Sự cố A -> A (Availability)
- Sự cố B -> I (Integrity)
- Sự cố C -> C (Confidentiality)

**Phân tích sự cố B:**
- Threat: Một kẻ tấn công hoặc người dùng có quyền truy cập vào hệ thống cơ sở dữ liệu có khả năng thay đổi điểm số mà không được phép.
- Vulnerability: Thiếu kiểm soát truy cập, không có hệ thống đăng nhập kiểm toán, xác thực yếu, và không có quy trình xác nhận thay đổi.
- Mitigation: Triển khai RBAC, ghi lại tất cả các thay đổi, yêu cầu MFA, và tạo quy trình phê duyệt hai cấp cho thay đổi điểm số. 

### 4. Kết luận ngắn
Bài lab này giúp tôi nhận thức sâu hơn về tầm quan trọng của bộ ba CIA trong bảo mật thông tin. Phần khó nhất là xác định chính xác threat và vulnerability cho từng sự cố, vì cùng một hệ thống có thể phát sinh nhiều vấn đề an toàn khác nhau. Điều quan trọng là cần hiểu rõ ngữ cảnh và mục tiêu của kẻ tấn công để đề xuất các biện pháp giảm thiểu (mitigation) thích hợp. Khi phân tích sự cố, cần xem xét toàn diện từ góc độ người dùng, quản trị viên, và kẻ tấn công tiềm ẩn.
