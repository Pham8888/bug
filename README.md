# 🎬 Website Xem Phim

Đây là một website xem phim đơn giản sử dụng PHP, MySQL và HTML/CSS, được xây dựng để phục vụ mục đích học tập, thực hành lập trình web và mô phỏng các lỗi bảo mật phổ biến theo tiêu chuẩn [OWASP Top 10](https://owasp.org/Top10/).

---

## 🧩 Chức năng chính

### Người dùng:
- Đăng ký, đăng nhập, đăng xuất
- Xem danh sách phim và từng tập cụ thể
- Tìm kiếm phim theo tên
- Bình luận từng phim hoặc tham gia diễn đàn
- Quản lý hồ sơ, nạp tiền (cash)

### Quản trị viên:
- Quản lý phim và từng tập phim (thêm, sửa, xóa)
- Quản lý người dùng
- Quản lý bình luận
- Theo dõi nhật ký giao dịch
- Quản lý phản hồi liên hệ

---

## 🗂️ Cấu trúc thư mục

bug/
├── admin/ # 📂 Trang quản trị
│ ├── dashboard.php # Bảng điều khiển admin
│ ├── movie_manage.php # Quản lý phim (thêm/sửa/xóa)
│ ├── episode_manage.php # Quản lý từng tập phim
│ ├── transaction_log.php # Xem lịch sử nạp tiền
│ ├── user_manage.php # Quản lý người dùng
│ ├── contact_manage.php # Quản lý liên hệ từ người dùng
│ └── comment_manage.php # Quản lý bình luận (xóa)
│
├── main/ # 📂 Đăng nhập / đăng ký / menu dùng chung
│ ├── login.php
│ ├── register.php
│ ├── logout.php
│ └── menu.php # Menu ngang dùng toàn trang
│
├── pages/ # 📂 Trang người dùng
│ ├── index.php # Trang chủ: hiển thị danh sách phim
│ ├── movie.php # Xem chi tiết phim + bình luận
│ ├── forum.php # Gợi ý phim, thảo luận chung
│ ├── profile.php # Hồ sơ cá nhân
│ ├── cash.php # Nạp tiền
│ ├── watch.php # Xem video
│ ├── contact.php # Gửi phản hồi
│ └── search.php # Kết quả tìm kiếm
│
├── assets/ # 📂 Tài nguyên tĩnh
│ ├── episodes/ # Video các tập phim (mp4)
│ ├── images/ # Ảnh poster phim
│ └── trailers/ # Trailer phim
│
├── config.php # ⚙️ Cấu hình thông số CSDL
├── db.php # Kết nối MySQL
└── movie_db.sql
