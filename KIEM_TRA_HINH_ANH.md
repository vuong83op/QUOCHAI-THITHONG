# 🔍 Kiểm Tra Lỗi Mất Hình Ảnh

## ❓ Các Nguyên Nhân Có Thể:

### 1. Thư mục `www.ewedinvite.site/images/` chưa được upload
**Kiểm tra:**
- Vào GitHub repository
- Xem có thư mục `www.ewedinvite.site/` không?
- Trong đó có thư mục `images/` không?
- Thư mục `images/` có đầy đủ các file .jpg không?

### 2. Cấu trúc thư mục trên GitHub không đúng
**Đúng phải là:**
```
QUOCHAI-THITHONG/
├── index.html
├── www.ewedinvite.site/
│   ├── images/
│   │   ├── anh1.jpg
│   │   ├── anh2.jpg
│   │   └── ... (tất cả ảnh)
```

### 3. Đường dẫn trong code
**Đường dẫn hiện tại:** `/www.ewedinvite.site/images/anh1.jpg`
**URL đầy đủ sẽ là:** `https://vuong83op.github.io/QUOCHAI-THITHONG/www.ewedinvite.site/images/anh1.jpg`

## 🔧 Cách Kiểm Tra:

1. **Mở Developer Tools (F12)**
2. Vào tab **Console** - xem có lỗi gì không
3. Vào tab **Network** - xem các file ảnh có load được không (status 404 = không tìm thấy)

## 💡 Giải Pháp Nếu Hình Ảnh Ở Root:

Nếu bạn muốn đơn giản hơn, có thể di chuyển thư mục `images/` lên root:
- Di chuyển từ: `www.ewedinvite.site/images/`
- Đến: `images/` (ở root)
- Đổi đường dẫn trong code thành: `/images/anh1.jpg`

---

**Vui lòng kiểm tra trên GitHub xem thư mục `www.ewedinvite.site/images/` có tồn tại không!**

