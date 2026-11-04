# Portfolio CV – Đỗ Việt Hoàng

## Mô tả

**Portfolio CV – Đỗ Việt Hoàng** là trang web giới thiệu cá nhân, kỹ năng Frontend Developer và các dự án tiêu biểu. Dự án được xây dựng theo hướng tĩnh, đáp ứng đa kích thước màn hình và không yêu cầu máy chủ backend hay cơ sở dữ liệu.

Trang web sử dụng bố cục mobile-first, nội dung bằng tiếng Việt, và có thể được mở trực tiếp bằng trình duyệt hoặc triển khai lên GitHub Pages, dịch vụ hosting tĩnh hoặc Docker.

## Tính năng

- Trang giới thiệu và giới thiệu nghề nghiệp Frontend Developer.
- Danh sách kỹ năng HTML5, CSS3, JavaScript, responsive design, Git/GitHub và Figma.
- Danh mục dự án tiêu biểu hiển thị bằng thẻ và bố cục CSS Grid/Flexbox.
- Menu điều hướng cuộn mượt đến các phần nội dung.
- Giao diện tương thích desktop, tablet và mobile.
- Thông tin liên hệ qua email và mạng xã hội.
- Hỗ trợ chuyển động giảm (`prefers-reduced-motion`) và cú pháp HTML ngữ nghĩa.

## Công nghệ sử dụng

- **HTML5** – cấu trúc và nội dung trang.
- **CSS3** – thiết kế giao diện, biến CSS, Flexbox và Grid.
- **JavaScript ES6+** – kỹ năng trình bày trong CV; dự án hiện tại chủ yếu là trang HTML/CSS tĩnh.
- **Git và GitHub** – quản lý mã nguồn và triển khai.
- **Docker và Nginx** – tùy chọn chạy trang web trong môi trường container.

## Cấu trúc thư mục

```text
.
├── index.html             # Nội dung chính của trang web
├── README.md              # Tài liệu hướng dẫn dự án
├── BAOCAO-A2.1.docx       # Báo cáo bài tập
└── assets/
    ├── css/
    │   └── styles.css     # Toàn bộ giao diện và media query
    └── img/
        ├── 2.jpg          # Ảnh đại diện
        └── 4.jpg          # Ảnh minh họa dự án
```

## Yêu cầu môi trường

### Chạy trực tiếp

- Trình duyệt hiện đại: Google Chrome, Microsoft Edge, Firefox hoặc Safari.
- Không bắt buộc Node.js, Python, cơ sở dữ liệu hoặc framework frontend.

### Với Git

- Git **2.x trở lên** nếu muốn tải mã nguồn bằng lệnh Git.

### Với Docker

- Docker Desktop (Windows/macOS) hoặc Docker Engine (Linux).
- Docker Compose không bắt buộc.

## Cài đặt

### Windows

Mở **PowerShell** hoặc **Command Prompt**, sau đó chạy:

```powershell
git clone https://github.com/viethoangxinhiu-ship-it/my-CV.git
cd my-CV
```

Nếu không có Git, hãy tải mã nguồn dạng ZIP từ GitHub, giải nén rồi mở thư mục dự án bằng File Explorer.

### macOS

Mở **Terminal**, sau đó chạy:

```bash
git clone https://github.com/viethoangxinhiu-ship-it/my-CV.git
cd my-CV
```

Có thể cài Git bằng Homebrew nếu chưa có:

```bash
brew install git
```

### Linux

Mở **Terminal**, cài Git theo hệ điều hành rồi tải dự án:

```bash
# Debian/Ubuntu
sudo apt update
sudo apt install git

# Fedora
sudo dnf install git

# Clone dự án
git clone https://github.com/viethoangxinhiu-ship-it/my-CV.git
cd my-CV
```

## Cấu hình

Dự án hiện không có file biến môi trường hoặc cấu hình API riêng vì là trang HTML/CSS tĩnh.

### Thay đổi thông tin cá nhân

Chỉnh sửa nội dung trong [index.html](index.html), chẳng hạn:

- Tên và tiêu đề nghề nghiệp trong phần Hero.
- Danh sách kỹ năng trong phần `skills`.
- Thông tin dự án trong phần `projects`.
- Email và liên kết mạng xã hội trong phần `contact`.

### Thay đổi màu sắc và kiểu chữ

Các biến giao diện tập trung tại phần đầu của [assets/css/styles.css](assets/css/styles.css):

```css
:root {
  --color-primary: #e0e3e8;
  --color-primary-dark: #9c68a0;
  --color-accent: #70579c;
  --color-bg: #faaaaa;
  --font-base: system-ui, -apple-system, "Segoe UI", Arial, sans-serif;
}
```

Nên sửa các biến trong khối `:root` thay vì thay màu riêng lẻ ở nhiều vị trí.

### Thay đổi ảnh

- Ảnh đại diện mặc định nằm tại `assets/img/2.jpg`.
- Ảnh minh họa dự án nằm tại `assets/img/4.jpg`.
- Có thể thay ảnh bằng cách giữ nguyên tên file hoặc cập nhật thuộc tính `src` tương ứng trong `index.html`.

## Chạy thử

### Windows

#### Cách 1: Mở trực tiếp

Mở thư mục dự án, nhấp đúp vào `index.html`, hoặc chạy trong PowerShell:

```powershell
Start-Process .\index.html
```

#### Cách 2: Dùng máy chủ tĩnh

Nếu đã cài Node.js, có thể dùng một máy chủ tĩnh đơn giản:

```powershell
npx serve .
```

Sau đó truy cập địa chỉ hiển thị trong terminal, thường là `http://localhost:3000`.

#### Cách 3: Dùng PHP

```powershell
php -S localhost:8080
```

Mở trình duyệt tại `http://localhost:8080`.

### macOS

#### Cách 1: Mở trực tiếp

```bash
open index.html
```

#### Cách 2: Dùng máy chủ Python

```bash
python3 -m http.server 8080
```

Truy cập `http://localhost:8080`, sau đó nhấn `Control+C` để dừng máy chủ.

### Linux

#### Cách 1: Mở trực tiếp

```bash
xdg-open index.html
```

#### Cách 2: Dùng máy chủ Python

```bash
python3 -m http.server 8080
```

Truy cập `http://localhost:8080`, sau đó nhấn `Control+C` để dừng máy chủ.

### Docker

Thực hiện tại thư mục chứa dự án.

#### Windows (PowerShell)

```powershell
docker run --rm -d --name my-cv -p 8080:80 -v "${PWD}:/usr/share/nginx/html:ro" nginx:alpine
```

#### macOS và Linux

```bash
docker run --rm -d --name my-cv -p 8080:80 -v "$(pwd):/usr/share/nginx/html:ro" nginx:alpine
```

Sau đó truy cập `http://localhost:8080`.

Kiểm tra container đang chạy:

```bash
docker ps
```

Dừng container:

```bash
docker stop my-cv
```

> Khi dùng Docker Desktop trên Windows, cần bật **Settings → Resources → File Sharing / Shared folders** cho ổ đĩa hoặc thư mục chứa dự án nếu Docker chưa truy cập được volume.

## Kiểm tra nhanh

Trước khi hoàn tất, xác nhận:

1. Trang không hiển thị lỗi 404 cho các liên kết ảnh và CSS.
2. Menu cuộn đúng đến phần Giới thiệu, Kỹ năng, Dự án và Liên hệ.
3. Giao diện hiển thị ổn trên desktop, tablet và mobile.
4. Đường dẫn trong phần liên hệ đã được cập nhật đúng tài khoản cá nhân.

## Triển khai GitHub Pages

1. Đẩy mã nguồn lên nhánh `main` của repository GitHub.
2. Mở **Settings → Pages** trong repository.
3. Trong mục **Build and deployment**, chọn nguồn `Deploy from a branch`.
4. Chọn nhánh `main` và thư mục `/ (root)`.
5. Lưu cấu hình và chờ GitHub hoàn tất triển khai.

Trang web có thể truy cập theo dạng:

```text
https://viethoangxinhiu-ship-it.github.io/my-CV/
```

## Thông tin liên hệ

- **Tên:** Đỗ Việt Hoàng
- **Vai trò:** Frontend Developer
- **Email:** [viethoangxinhiu@gmail.com](mailto:viethoangxinhiu@gmail.com)
- **GitHub:** [github.com/viethoangxinhiu-ship-it](https://github.com/viethoangxinhiu-ship-it)

Các liên kết mạng xã hội, ảnh đại diện và thông tin dự án trong trang có thể được cập nhật trực tiếp tại [index.html](index.html).

## Giấy phép

Dự án được tạo cho mục đích học tập và trình bày hồ sơ cá nhân. Khi sử dụng lại, vui lòng ghi công tác giả và thay thông tin cá nhân bằng thông tin của bạn.
