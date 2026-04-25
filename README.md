[README.md](https://github.com/user-attachments/files/27083875/README.md)
# 📋 Portfolio CV Website - Hướng Dẫn Sử Dụng

Chào mừng bạn đến với **MyPortfolio** - một website CV cá nhân chuyên nghiệp, hiện đại và dễ sử dụng!

## 🎯 Cấu Trúc Website

Website gồm 4 trang chính:

1. **Trang Chủ (index.html)** - Giới thiệu sơ lược với nút CTA
2. **Giới Thiệu (about.html)** - Chi tiết về kỹ năng, kinh nghiệm và giáo dục
3. **Dự Án (projects.html)** - Giới thiệu các dự án và cách thêm dự án mới
4. **Liên Hệ (contact.html)** - Form liên hệ với validation và FAQ

## 📁 Cấu Trúc Thư Mục

```
cv/
├── index.html          # Trang chủ
├── about.html          # Trang giới thiệu
├── projects.html       # Trang dự án
├── contact.html        # Trang liên hệ
├── css/
│   └── styles.css      # Toàn bộ styling
├── js/
│   └── script.js       # Toàn bộ JavaScript
└── README.md          # File này
```

## 🚀 Cách Sử Dụng

### 1. Mở Website
- Mở file `index.html` trong trình duyệt web
- Hoặc sử dụng Live Server (VS Code Extension)

### 2. Chỉnh Sửa Nội Dung

#### Thay đổi tên và thông tin cá nhân:
1. Mở các file HTML bằng trình soạn thảo văn bản (VS Code, Notepad++, v.v.)
2. Tìm và thay thế:
   - `MyPortfolio` → Tên của bạn
   - `email@example.com` → Email thực của bạn
   - `+84 123 456 789` → Số điện thoại của bạn
   - Các nội dung khác theo ý muốn

#### Thay đổi thông tin công việc:
- Mở `about.html`
- Tìm phần "Kinh Nghiệm" hoặc "Giáo Dục"
- Chỉnh sửa các công ty, chức danh, mô tả công việc

#### Thêm dự án mới:
- Mở `projects.html`
- Tìm phần `.projects-grid`
- Sao chép một `.project-card` hiện có
- Chỉnh sửa thông tin dự án:
  ```html
  <h3>Tên Dự Án Mới</h3>
  <p>Mô tả dự án của bạn</p>
  <span class="tag">Công Nghệ 1</span>
  <span class="tag">Công Nghệ 2</span>
  ```

## 🎨 Tùy Chỉnh Thiết Kế

### Thay đổi màu sắc chính:
Mở `css/styles.css` và tìm phần `:root`:

```css
:root {
    --primary-color: #1e90ff;      /* Màu xanh dương chính */
    --primary-light: #00bfff;      /* Màu xanh dương nhạt */
    /* ... các màu khác */
}
```

Bạn có thể thay đổi các mã màu này thành màu yêu thích của bạn.

### Thay đổi font chữ:
Tìm dòng này trong `styles.css`:
```css
body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
```

### Thêm hình ảnh:
1. Tạo thư mục `images/` trong thư mục `cv`
2. Thêm hình ảnh vào thư mục này
3. Thay thế các div có emoji bằng `<img>` tag:
   ```html
   <img src="images/your-image.jpg" alt="Mô tả hình">
   ```

## ✨ Các Tính Năng

### ✅ Hoàn Thành
- ✓ 4 trang HTML đầy đủ
- ✓ Thiết kế responsive (mobile-friendly)
- ✓ Hiệu ứng animation mượt mà (fade-in, slide-in, hover)
- ✓ Menu điều hướng sticky và mobile hamburger
- ✓ Form liên hệ với validation
- ✓ Skill bars với animation
- ✓ Project cards với hover effects
- ✓ Footer đầy đủ với mạng xã hội
- ✓ Dark mode ready (có thể thêm later)
- ✓ SEO friendly

## 📱 Responsive Design

Website tự động điều chỉnh để phù hợp với các kích thước màn hình:
- **Desktop**: 1400px trở lên
- **Tablet**: 768px - 1399px
- **Mobile**: Dưới 768px

Hamburger menu sẽ xuất hiện tự động trên thiết bị di động.

## 🔧 Tùy Chỉnh Form Liên Hệ

Hiện tại, form chỉ thực hiện validation phía client. Để gửi email thực sự:

### Option 1: Dùng FormSubmit.co (Miễn phí)
1. Mở `contact.html`
2. Thay đổi form action:
```html
<form action="https://formsubmit.co/YOUR_EMAIL@gmail.com" method="POST">
```
3. Thêm `<input type="hidden" name="_captcha" value="false">`

### Option 2: Dùng dịch vụ backend
- Triển khai backend API để xử lý form
- Cập nhật JavaScript để gửi dữ liệu đến API

## 🚀 Triển Khai Website

### Trên Netlify (Miễn phí & Dễ)
1. Đăng ký tại [Netlify.com](https://netlify.com)
2. Kéo thả thư mục `cv` lên Netlify
3. Website của bạn sẽ live ngay lập tức!

### Trên GitHub Pages (Miễn phí)
1. Tạo repository `username.github.io`
2. Upload tất cả file vào repository
3. Truy cập `https://username.github.io`

### Trên Web Hosting thông thường
1. Upload toàn bộ thư mục `cv` lên hosting
2. Cấu hình domain nếu có

## 📞 Support

Nếu bạn gặp vấn đề hoặc muốn thêm tính năng:
- Kiểm tra console browser (F12) để xem lỗi
- Đọc lại các comment trong code
- Tham khảo các resource web development

## 📝 Ghi Chú

- Website sử dụng vanilla HTML, CSS, JavaScript (không cần build tools)
- Tất cả styles nằm trong `styles.css` - dễ quản lý
- JavaScript được modularize với các comment rõ ràng
- Responsive design được test trên tất cả kích thước màn hình

## 🎓 Học Tập

Nếu bạn muốn học thêm:
- **HTML**: [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/HTML)
- **CSS**: [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS)
- **JavaScript**: [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

## 📄 License

Website này được tạo ra cho mục đích cá nhân và giáo dục.

---

**Chúc bạn thành công với portfolio của mình! 🌟**
