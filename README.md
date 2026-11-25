# WEBSITE HỆ THỐNG QUẢN LÝ NHÀ SÁCH - MƯỢN VÀ TRẢ SÁCH THƯ VIỆN

# Phạm vi dự án

-   Hiện với sự phát triển của Công Nghệ Thông Tin thì việc ứng dụng các sản
    phẩm công nghệ vào đời sống cũng như công việc là điều tất yếu, bởi lẽ nó mang đến
    cho con người sự tiện lợi, linh hoạt và hiệu quả mà các phương pháp truyền thống
    vẫn chưa thể đáp ứng được. Trong đó, Hệ thống quản lý mượn trả sách trực tuyến là
    một giải pháp công nghệ thông tin nhằm đơn giản hóa quy trình quản lý và nâng cao
    trải nghiệm của người dùng trong các thư viện, trung tâm học liệu. Trong đề tài này, hệ thống cung cấp các tính năng sau:

- Tích hợp trò chuyện trực tiếp giữa quản trị viên và người dùng.
- Hiển thị chi tiết vị trí đặt sách trong thư viện.
- Quản lý giao dịch mượn trả sách một cách minh bạch và trực quan.
- Tự động hóa quy trình đánh dấu trả sách, giảm thiểu thao tác thủ công.
Các chức năng được thiết kế dựa trên các công nghệ như Vue.js, Laravel và cơ
sở dữ liệu quan hệ. Hệ thống không chỉ cải thiện hiệu suất quản lý mà còn tăng tính thân thiện và tiện lợi đối với người dùng.
Lợi ích khi sử dụng hệ thống :
- Nâng cao hiệu quả làm việc: Tự động hóa các công việc thủ công, giảm thiểu
sai sót.
- Tiết kiệm thời gian: Quản lý thông tin nhanh chóng, chính xác.
- Tăng cường trải nghiệm người dùng: Dễ dàng tìm kiếm và mượn sách.
- Quản lý tài sản hiệu quả: Theo dõi tình trạng sách, giảm thiểu thất thoát.

-   Công nghệ sử dụng
    ⮚ HTML5/ CSS3, Javascript, Vue.js, PHP/Laravel, Ajax, MySQL

## DEMO
-   Youtube: https://youtu.be/UuvmZWTOgls?si=LrGgtOLnGI21_Gad

# Tài khoản

-   Admin: admin@gmail.com - admin123456
-   Độc giả: reader@gmail.com - admin123456

## Cài đặt

Để cài đặt dự án, bạn cần thực hiện các bước sau:

1. Clone repository

2. Cài đặt các phụ thuộc:

    ````bash
    composer install

3. Tạo file .env:

    ```bash
    cp .env.example .env

    ```

4. Cấu hình file .env:
   Mở file .env và cấu hình các thông số kết nối cơ sở dữ liệu, ứng dụng, và các thông tin khác cần thiết cho dự án.

5. Tạo khóa ứng dụng:

    ```bash
    php artisan key:generate

    ```

6. Chạy migration:

    ```bash
    php artisan migrate

    ```

7. Chạy seeder:

    ```bash
    php artisan db:seed

    ```

8. Run project:

    ```bash
    php artisan serve

    ```

9. Truy cập vào đường dẫn để xem ứng dụng:
    ```bash
    http://127.0.0.1:8000
    ```

Đóng góp
Nếu bạn muốn đóng góp cho dự án, vui lòng tạo pull request và tuân thủ các quy tắc đóng góp.

Giấy phép
Dự án này được cấp phép theo MIT License.
