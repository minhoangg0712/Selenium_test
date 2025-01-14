Nguyễn Minh Hoàng - BIT220063 - 22SE1

Bài tập 3 của môn Kiểm thử phần mềm

Đề bài: Selenium Test Project

### Mô tả dự án

Dự án này sử dụng Selenium để thực hiện các bài test tự động trên giao diện web. Mục đích là đảm bảo tính đúng đắn của các chức năng và giao diện trên trang web mà bạn đang phát triển hoặc đang quản lý.

### Các tính năng chính

Kiểm tra tính năng: Thực hiện các bài test tự động để kiểm tra tính năng của các trang web.

Báo cáo chi tiết: Tự động tạo báo cáo sau khi test.

Khả năng tích hợp cao: Tích hợp Selenium với các công cụ như TestNG/JUnit để quản lý test case.

### Yêu cầu hệ thống

- Ngôn ngữ: Java.

- Công cụ: Selenium WebDriver, Maven, TestNG/JUnit.

- Hệ điều hành: Windows

- Trình duyệt: Chrome/Edge.

### Cài đặt

Clone repository:

    git clone https://github.com/minhoangg0712/Selenium_test.git

    cd FacebookLoginTest

- Import dự án vào IDE bạn sử dụng (ví dụ: IntelliJ IDEA, Eclipse)

- Cấu hình thư viện cần thiết: Maven sẽ tự động tải về các thư viện được khai báo trong tệp pom.xml.

Tải về WebDriver phù hợp:

- Đối với Chrome: ChromeDriver

- Đặt driver trong PATH của hệ thống hoặc cập nhật đường dẫn trong mã nguồn

Cài đặt các dependency qua Maven:

    <dependency>
        <groupId>org.seleniumhq.selenium</groupId>
        <artifactId>selenium-java</artifactId>
        <version>4.13.1</version>
    </dependency>

Đảm bảo trình duyệt của bạn tương thích với WebDriver.

### Hướng dẫn sử dụng

Chạy các test case:

- Mở IDE (IntelliJ IDEA/Eclipse).

- Đảm bảo WebDriver được thiết lập trong biến môi trường.

- Nhấn chuột phải và chọn "Run Tests".

Thêm test case mới:

- Tạo file test trong thư mục src/test.

- Kết hợp các bước sau đó viết logic test.

Xem báo cáo:

- Sau khi chạy test, báo cáo được lưu trong thư mục target hoặc được hiển thị trên console.

### Cấu trúc dự án

    Selenium_test/
    |-- src/
    |   |-- main/
    |   |   |-- java/
    |   |       |-- com.example.tests
    |   |-- test/
    |       |-- java/
    |           |-- com.example.tests
    |-- pom.xml
    |-- README.md


### Các trường hợp kiểm thử

Đăng nhập thành công

- Điều kiện đầu tiên: Tên đăng nhập và mật khẩu hợp lệ. Các bước:
- Truy cập trang đăng nhập.
- Nhập thông tin đăng nhập hợp lệ.
- Nhấn nút đăng nhập.
- Kết quả mong đợi: Người dùng được chuyển đến trang chủ.

Đăng nhập thất bại
- Điều kiện đầu tiên: Tên đăng nhập hoặc mật khẩu không hợp lệ. Các bước:
- Truy cập trang đăng nhập.
- Nhập thông tin đăng nhập không hợp lệ.
- Nhấn nút đăng nhập.
- Kết quả mong đợi: Thông báo lỗi được hiển thị.

Thông tin đăng nhập bị thiếu
- Điều kiện đầu tiên: Trường tên đăng nhập hoặc mật khẩu bị để trống. Các bước:
- Truy cập trang đăng nhập.
- Để trống trường tên đăng nhập hoặc mật khẩu.
- Nhấn nút đăng nhập.
- Kết quả mong đợi: Hiển thị thông báo yêu cầu nhập đầy đủ thông tin.

### Hình ảnh kết quả
![Screenshot (177)](https://github.com/user-attachments/assets/056857ae-2cfe-4dc2-8486-983a6da17c8d)
