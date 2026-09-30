# HƯỚNG DẪN CUSTOM LOGIN VỚI SPRING BOOT + SECURITY (VD2)

Dự án bài tập cấu hình chức năng Custom Login linh hoạt bằng Username hoặc Email sử dụng Spring Boot và Spring Security. 

## 🚀 Công nghệ sử dụng
- **Backend:** Spring Boot 4.1.1
- **Security:** Spring Security 7.1.x
- **Java:** JDK 26 (hoặc tương thích 17/21)
- **Database:** H2 (In-memory Database)
- **ORM:** Spring Data JPA / Hibernate
- **View:** Thymeleaf & Thymeleaf Layout Dialect
- **Mapper:** MapStruct 1.6.3
- **Build Tool:** Maven

## 🎯 Chức năng chính
- **Custom Login:** Cho phép người dùng đăng nhập bằng cả **Username** hoặc **Email**.
- **User Interface:** Giao diện trang đăng nhập, trang chủ, thanh điều hướng header (hiển thị Ảnh đại diện, Username, Email, Họ tên, Role của user đăng nhập thành công).
- **Phân quyền truy cập:** Cấu hình Security bảo vệ các route (trang chủ cần đăng nhập, trang quản trị yêu cầu quyền ADMIN...).
- **Tự động khởi tạo dữ liệu:** Tự động tạo dữ liệu mẫu mỗi khi ứng dụng khởi động.

## ⚙️ Hướng dẫn cài đặt và chạy dự án

### 1. Chuẩn bị
Ứng dụng sử dụng cơ sở dữ liệu **H2 (In-memory)**, do đó bạn không cần phải cài đặt hay cấu hình bất kỳ hệ quản trị cơ sở dữ liệu ngoài (như MySQL hay SQL Server). Hệ thống sẽ tự động cấu hình và tạo Database trực tiếp trên RAM mỗi khi khởi động.

### 2. Chạy ứng dụng
Mở project bằng IDE (IntelliJ IDEA, Eclipse, VS Code...) và chạy file `Springboot19Application.java`.

### 3. Đăng nhập thử
Ứng dụng tự động tạo sẵn một tài khoản trong cơ sở dữ liệu để bạn test:
- **Tài khoản (Username):** `user01`
- **Hoặc Email:** `user01@gmail.com`
- **Mật khẩu:** `123456`

- Mặc định ứng dụng chạy trên port `8080`. Bạn truy cập vào: `http://localhost:8080/` để sử dụng.
