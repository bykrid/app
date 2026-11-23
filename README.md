# Hướng Dẫn Dự Án Web 6789 (GitHub Pages: bykrid.github.io/app/)

Dự án đã được thiết kế sẵn theo đúng yêu cầu của anh: **2 lựa chọn riêng biệt, không gộp chung, giao diện siêu mượt và tối ưu chuẩn hiện đại**.

---

## 🗂️ Cấu Trúc Dự Án Ngoài Màn Hình (`C:\Users\GPD\Desktop\app\`)

```text
Desktop/app/
│
├── index.html            👉 CỔNG CHỌN (HUB PORTAL) khi khách vào bykrid.github.io/app/
│                            Khách có 2 thẻ lựa chọn rõ ràng:
│                            [1] 6789 Store TV ➔ vào link "tv/"
│                            [2] FRP Bypass & Tools ➔ vào link "frp/"
│
├── tv/                   👉 LỰA CHỌN 1: KHO APP ANDROID TV (Mẫu ximaotv nâng cấp)
│   ├── index.html        (Giao diện Liquid Glass mượt mà, hỗ trợ Remote TV, tìm kiếm nhanh)
│   ├── admin.html        (Trang quản lý thêm/xóa app trực quan)
│   ├── data/apps.js      (Danh sách app, danh mục)
│   ├── icons/            (Icon các app TV)
│   └── apks/             (Nơi anh chứa các file apk tải thẳng)
│
└── frp/                  👉 LỰA CHỌN 2: FRP BYPASS & MOBILE TOOLS (Sao chép hellochoi tối ưu)
    └── index.html        (Giao diện Dark Mode siêu nhẹ, gọi nhanh Intent Cài đặt, Galaxy Store,
                           V-Appstore, Oppo Market, nút tải APK Bypass Android 7-8-9-10, 
                           tiện ích iOS TrollStore, Config chặn FMI...)
```

---

## 🌐 Các Đường Link Khi Đưa Lên GitHub Pages:

- **Cổng lựa chọn chính:** `https://bykrid.github.io/app/`
- **Kho ứng dụng Android TV:** `https://bykrid.github.io/app/tv/`
- **Công cụ FRP Bypass Mobile:** `https://bykrid.github.io/app/frp/`

---

## 🚀 Cách Đẩy Lên GitHub Repo:

1. Đăng nhập vào GitHub tài khoản **bykrid**.
2. Tạo repository mới tên là: **`app`** (để chế độ **Public**).
3. Đẩy toàn bộ thư mục `Desktop/app` lên repo:
   - Dùng Git dòng lệnh:
     ```bash
     cd C:\Users\GPD\Desktop\app
     git init
     git add .
     git commit -m "Khoi tao 6789 Hub - TV Store va FRP Tools"
     git branch -M main
     git remote add origin https://github.com/bykrid/app.git
     git push -u origin main
     ```
   - Hoặc kéo thả toàn bộ thư mục lên giao diện web GitHub.
4. Bật GitHub Pages:
   - Vào **Settings** của repo `app` -> Chọn **Pages** ở menu bên trái.
   - Tại mục **Branch**: Chọn `main` và `/(root)` -> Bấm **Save**.
5. Sau 1 phút, hệ thống sẽ chạy online tại: `https://bykrid.github.io/app/`.
