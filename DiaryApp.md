# DailyCanvas - Your Digital Diary Companion

*A personal journaling platform for capturing life's moments*

## 1. Spec (Specification)

### 1.1. Mục tiêu
- Tạo một ứng dụng web cho phép người dùng viết, lưu trữ và quản lý nhật ký cá nhân.
- Đảm bảo tính riêng tư và bảo mật cho dữ liệu người dùng.
- Cung cấp trải nghiệm người dùng đơn giản, dễ sử dụng.

### 1.2. Tính năng chính

#### 1.2.1. Đăng ký và Đăng nhập
- Người dùng có thể đăng ký tài khoản bằng email và mật khẩu.
- Xác thực email sau khi đăng ký.
- Đăng nhập bằng email/mật khẩu hoặc OAuth (Google, Facebook).
- Quên mật khẩu và đặt lại mật khẩu.

#### 1.2.2. Quản lý nhật ký
**Tạo nhật ký mới:**
- Tiêu đề và nội dung.
- Thêm hình ảnh, video hoặc tệp đính kèm (tùy chọn).
- Gắn thẻ (tags) để phân loại.
- Chỉnh sửa và xóa nhật ký.

**Xem danh sách nhật ký:**
- Hiển thị theo thời gian (mới nhất hoặc cũ nhất).
- Tìm kiếm nhật ký bằng từ khóa hoặc thẻ.
- Lưu nhật ký nháp (draft) để hoàn thành sau.

#### 1.2.3. Tính năng bổ sung
**Nhắc nhở viết nhật ký:**
- Người dùng có thể đặt lịch nhắc nhở hàng ngày.

**Xuất nhật ký:**
- Xuất nhật ký dưới dạng file PDF hoặc văn bản.

**Tùy chỉnh giao diện:**
- Thay đổi theme (sáng/tối).
- Tùy chỉnh font chữ và kích thước chữ.

#### 1.2.4. Bảo mật
- Mã hóa dữ liệu nhật ký.
- Xác thực hai yếu tố (2FA) để tăng cường bảo mật.
- Tùy chọn khóa ứng dụng bằng mã PIN hoặc vân tay (nếu hỗ trợ).

### 1.3. Yêu cầu kỹ thuật

#### 1.3.1. Công nghệ
- Frontend: HTML, CSS, JavaScript (React.js hoặc Vue.js).
- Backend: Node.js (Express.js) hoặc Python (Django/Flask).
- Cơ sở dữ liệu: MongoDB hoặc PostgreSQL.
- Lưu trữ file: AWS S3 hoặc Firebase Storage.
- Xác thực: JWT (JSON Web Token) hoặc OAuth.

#### 1.3.2. Hiệu suất
- Thời gian tải trang dưới 3 giây.
- Hỗ trợ tối thiểu 1.000 người dùng đồng thời.

#### 1.3.3. Bảo mật
- Mã hóa dữ liệu nhạy cảm (AES-256).
- Ngăn chặn các cuộc tấn công phổ biến (SQL Injection, XSS, CSRF).

### 1.4. Giao diện người dùng (UI/UX)
- Màu sắc: Tông màu nhẹ nhàng, dễ chịu (pastel).
- Font chữ: Sans-serif (ví dụ: Roboto, Open Sans).
- Layout: Đơn giản, tập trung vào nội dung.

## 2. Prototype

### 2.1. Wireframe (Low-fidelity)

**Trang chủ (Home)**
- Header: Logo, nút đăng nhập/đăng ký.
- Body: Giới thiệu ngắn về ứng dụng, nút "Bắt đầu ngay".

**Trang đăng nhập (Login)**
- Form đăng nhập với email và mật khẩu.
- Nút "Quên mật khẩu" và "Đăng nhập bằng Google/Facebook".

**Trang dashboard**
- Sidebar: Menu với các tùy chọn (Tạo nhật ký, Danh sách nhật ký, Cài đặt).
- Main Content: Danh sách nhật ký (tiêu đề, ngày tạo, thẻ).

**Trang tạo/chỉnh sửa nhật ký**
- Tiêu đề: Ô nhập tiêu đề.
- Nội dung: Trình soạn thảo văn bản (WYSIWYG).
- Tùy chọn: Thêm hình ảnh, video, thẻ.

### 2.2. High-fidelity Prototype (Figma)
- Link demo: Figma Prototype (giả định).
- Chi tiết:
  - Giao diện trực quan với các nút bấm, hiệu ứng hover và chuyển trang.
  - Mô phỏng quy trình đăng nhập, tạo nhật ký và xem danh sách nhật ký.

### 2.3. Tương tác người dùng

**Tạo nhật ký:**
1. Nhấn nút "Tạo nhật ký".
2. Nhập tiêu đề và nội dung.
3. Thêm hình ảnh hoặc thẻ (tùy chọn).
4. Nhấn "Lưu" để lưu nhật ký hoặc "Lưu nháp" để hoàn thành sau.

**Tìm kiếm nhật ký:**
1. Nhập từ khóa vào ô tìm kiếm.
2. Kết quả hiển thị ngay lập tức. 