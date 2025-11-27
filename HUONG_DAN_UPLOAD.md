# Hướng Dẫn Upload Lên GitHub

## ✅ Đã Hoàn Thành

Tôi đã tạo file `index.html` ở root với nội dung trang thiệp cưới. Bây giờ khi bạn truy cập:
```
https://vuong83op.github.io/QUOCHAI-THITHONG/
```
Sẽ tự động hiển thị trang thiệp cưới QUỐC HẢI & THỊ THÔNG!

## 📋 Các File Cần Upload

Khi upload lên GitHub, bạn cần upload **TOÀN BỘ** cấu trúc sau:

```
QUOCHAI-THITHONG/
├── index.html                    ← File chính (đã có)
├── backblue.gif                  ← File hỗ trợ
├── fade.gif                      ← File hỗ trợ
├── www.ewedinvite.site/          ← Thư mục chứa hình ảnh
│   ├── QUOCHAI&THITHONG.html     ← File backup
│   ├── images/                   ← THƯ MỤC QUAN TRỌNG
│   │   ├── anh1.jpg
│   │   ├── anh2.jpg
│   │   ├── ... (tất cả ảnh)
│   └── webcake/                  ← Tài nguyên webcake
├── content.pancake.vn/           ← Nếu có (các file tài nguyên)
├── api.webcake.io/               ← Nếu có (CSS, fonts)
└── a.pancake.vn/                 ← Nếu có (JavaScript)
```

## 🚀 Các Bước Upload

### Cách 1: Dùng GitHub Desktop (Dễ nhất)

1. Mở **GitHub Desktop**
2. Chọn repository `QUOCHAI-THITHONG`
3. Kéo thả **TOÀN BỘ** thư mục `C:\ThiepCuoi` vào GitHub Desktop
4. Commit với message: "Upload thiệp cưới QUỐC HẢI & THỊ THÔNG"
5. Click **Push origin**

### Cách 2: Dùng Git Command

```bash
cd C:\ThiepCuoi
git add .
git commit -m "Upload thiệp cưới QUỐC HẢI & THỊ THÔNG"
git push origin main
```

### Cách 3: Upload Thủ Công Trên GitHub

1. Vào repository trên GitHub: `vuong83op/QUOCHAI-THITHONG`
2. Click **Add file** → **Upload files**
3. Kéo thả **TOÀN BỘ** nội dung từ thư mục `C:\ThiepCuoi` vào
4. Click **Commit changes**

## ⚙️ Kích Hoạt GitHub Pages

1. Vào repository trên GitHub
2. Click **Settings** (Cài đặt)
3. Scroll xuống phần **Pages**
4. Trong **Source**, chọn:
   - Branch: **main**
   - Folder: **/ (root)**
5. Click **Save**
6. Đợi 1-2 phút để GitHub build lại

## 🔗 URL Truy Cập

Sau khi upload xong, bạn có thể truy cập:

- **Trang chủ**: `https://vuong83op.github.io/QUOCHAI-THITHONG/`
- **File backup**: `https://vuong83op.github.io/QUOCHAI-THITHONG/www.ewedinvite.site/QUOCHAI%26THITHONG.html`

## ⚠️ Lưu Ý Quan Trọng

1. **Phải upload đầy đủ**:
   - ✅ File `index.html` ở root
   - ✅ Thư mục `www.ewedinvite.site/` và tất cả nội dung bên trong
   - ✅ Các thư mục tài nguyên khác nếu có

2. **Đường dẫn đã được cập nhật**:
   - ✅ Tất cả đường dẫn hình ảnh đã được cập nhật để hoạt động từ root
   - ✅ Không cần chỉnh sửa gì thêm

3. **Nếu bị lỗi 404**:
   - Đợi thêm 2-3 phút sau khi push
   - Clear cache trình duyệt (Ctrl + F5)
   - Kiểm tra lại tên file có đúng không

## ✅ Checklist

- [ ] Upload file `index.html` lên root
- [ ] Upload thư mục `www.ewedinvite.site/` và tất cả nội dung
- [ ] Kích hoạt GitHub Pages
- [ ] Test URL: `https://vuong83op.github.io/QUOCHAI-THITHONG/`
- [ ] Kiểm tra hình ảnh hiển thị đúng

---

🎉 **Chúc bạn thành công!**

