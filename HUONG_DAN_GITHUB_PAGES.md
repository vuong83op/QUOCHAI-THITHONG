# Hướng Dẫn Sửa Lỗi 404 GitHub Pages

## 🔍 Nguyên Nhân Lỗi

Lỗi 404 xảy ra vì:
1. **Đường dẫn không khớp**: File trên GitHub khác với đường dẫn trong URL
2. **File hoặc thư mục chưa được upload đầy đủ** lên GitHub

## ✅ Giải Pháp

### Cách 1: Nếu file ở ROOT trên GitHub (khuyến nghị)

Nếu trên GitHub, file `QUOCHAI&THITHONG.html` nằm ở root (như trong hình), bạn cần:

**Bước 1:** Đảm bảo file nằm ở root repository:
```
QUOCHAI-THITHONG/
├── QUOCHAI&THITHONG.html  ← File ở đây
├── index.html
└── ...
```

**Bước 2:** URL đúng sẽ là:
```
https://vuong83op.github.io/QUOCHAI-THITHONG/QUOCHAI%26THITHONG.html
```
(Lưu ý: `%26` là mã URL của ký tự `&`)

**Bước 3:** Kiểm tra file `index.html` đã được cập nhật để redirect đúng

### Cách 2: Nếu muốn file nằm trong thư mục `www.ewedinvite.site`

Nếu bạn muốn giữ cấu trúc thư mục như local, bạn cần:

**Bước 1:** Upload TOÀN BỘ thư mục `www.ewedinvite.site` lên GitHub

**Bước 2:** Cấu trúc sẽ là:
```
QUOCHAI-THITHONG/
├── www.ewedinvite.site/
│   ├── QUOCHAI&THITHONG.html
│   ├── images/
│   └── ...
└── index.html
```

**Bước 3:** URL sẽ là:
```
https://vuong83op.github.io/QUOCHAI-THITHONG/www.ewedinvite.site/QUOCHAI%26THITHONG.html
```

## ⚙️ Cấu Hình GitHub Pages

1. Vào repository trên GitHub: `vuong83op/QUOCHAI-THITHONG`
2. Click vào **Settings** (Cài đặt)
3. Scroll xuống phần **Pages**
4. Chọn branch **main** trong "Source"
5. Chọn folder **/ (root)**
6. Click **Save**

Đợi vài phút để GitHub Pages build lại.

## 📝 Lưu Ý Quan Trọng

1. **Case sensitivity**: GitHub Pages phân biệt hoa/thường. Đảm bảo tên file khớp chính xác.
2. **Ký tự đặc biệt**: Ký tự `&` trong tên file sẽ thành `%26` trong URL
3. **Thời gian deploy**: Sau khi push code lên GitHub, đợi 1-2 phút để Pages cập nhật

## 🔗 Các URL Có Thể Dùng

- Trang chủ: `https://vuong83op.github.io/QUOCHAI-THITHONG/`
- File HTML (nếu ở root): `https://vuong83op.github.io/QUOCHAI-THITHONG/QUOCHAI%26THITHONG.html`
- File HTML (nếu trong thư mục): `https://vuong83op.github.io/QUOCHAI-THITHONG/www.ewedinvite.site/QUOCHAI%26THITHONG.html`

## ❓ Nếu Vẫn Bị Lỗi

1. Kiểm tra file có đúng tên: `QUOCHAI&THITHONG.html` (không phải `QUOCHAI&THITHONG.HTML`)
2. Kiểm tra tất cả hình ảnh và file liên quan đã được upload
3. Đợi thêm vài phút sau khi push code
4. Clear cache trình duyệt (Ctrl+F5)

