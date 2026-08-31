# 🎨 ACO Color Viewer Pro

Công cụ xem, trộn và xuất bảng màu Photoshop (`.aco`) chạy **ngay trên trình duyệt** — không cần cài đặt, không cần đăng ký, không tải dữ liệu lên mạng.

> Mọi dữ liệu được xử lý **hoàn toàn cục bộ** trên máy/điện thoại của bạn.

---

## ✨ Tính năng

### 📁 Xem ACO
- Kéo thả hoặc chọn file `.aco` để mở
- Hỗ trợ **ACO v1 & v2**, đọc được **tên màu** và các hệ màu RGB / HSB / CMYK / Lab / Grayscale
- Mỗi màu hiển thị kèm **số thứ tự**, tên màu, mã HEX, RGB và hệ màu gốc
- **Tìm kiếm** theo tên/HEX/RGB, **sắp xếp** theo sắc độ, độ sáng, bão hòa, tên

### 📋 Sao chép
- Click thẻ màu để copy mã (**HEX / RGB / HSL** — tùy chọn)
- **Copy tất cả** dưới dạng: danh sách HEX, CSS Variables, SCSS, JSON, RGB

### 🎨 Trộn màu (dùng độc lập, không cần mở ACO)
- Thêm màu bằng **ô chọn màu** hoặc **mở file ACO** ngay trong mục này
- Lưới chọn lọc: **loại bỏ màu không muốn trộn** bằng một cú click
- **Chỉnh lại lựa chọn** mà không cần tải lại file
- Tỷ lệ mỗi màu **tự động chia đều**, kéo thanh trượt để chỉnh riêng
- **Lịch sử trộn** tự lưu, click để copy lại

### ⬇ Xuất
- **PNG / SVG / CSS / JSON / TXT**
- Tùy chọn bố cục (dải ngang / dải dọc / lưới), kích thước, nhãn, nền trong suốt
- Xem trước trực tiếp trước khi tải

### 🌙 Giao diện
- Chế độ **sáng / tối**, giao diện hiện đại
- **Thiết kế riêng cho điện thoại** (nav dưới cùng, bottom-sheet, nút to vừa tay)

### 📲 Cài đặt làm App (PWA)
- Cài được trên **máy tính (Windows/Mac/Linux)** và **điện thoại (Android/iOS)**
- Có **icon riêng**, mở cửa sổ độc lập, chạy **offline** không cần mạng

### 🖥 Bản desktop (.exe)
- Đóng gói thành **ứng dụng cài đặt trên Windows** bằng Electron — xem thư mục `electron-app/`

---

## 🚀 Cách sử dụng

### Trên máy tính / điện thoại
Chỉ cần mở file `index.html` bằng trình duyệt (double-click), hoặc truy cập link web đã deploy.

### Quy trình nhanh
1. Chọn tab **📁 Xem ACO** → kéo thả file `.aco` vào
2. Click màu để copy, hoặc tick chọn nhiều màu để xuất
3. Chọn tab **🎨 Trộn màu** → thêm màu → xem kết quả trộn ngay
4. Bấm **⬇ Xuất ảnh & dữ liệu** để tải bảng màu

---

## 📲 Cài đặt làm App (PWA)

Sau khi app được deploy (có link https), bạn có thể cài thành app thật:

### Trên máy tính (Chrome / Edge)
1. Mở link web của app
2. Bấm biểu tượng **📲** (nút "Cài đặt" xuất hiện ở góc phải) **hoặc** biểu tượng cài đặt trên thanh địa chỉ
3. Chọn **Install / Cài đặt** → app xuất hiện trên Desktop và menu Start

### Trên Android (Chrome)
1. Mở link web của app
2. Bấm menu **⋮ → "Thêm vào Màn hình chính"** (Add to Home Screen)
3. App có icon riêng, mở toàn màn hình như app thường

### Trên iPhone / iPad (Safari)
1. Mở link web của app
2. Bấm nút **Chia sẻ** (hình vuông + mũi tên) → **"Thêm vào Màn hình chính"**
3. App xuất hiện trên màn hình chính

> **Lưu ý quan trọng:** PWA yêu cầu phục vụ qua **HTTPS** (GitHub Pages, Netlify, Vercel đều hỗ trợ sẵn). Không cài được khi mở file trực tiếp `file://` hoặc qua `http://` không an toàn (trừ localhost).

---

## 🖥 Chạy thử trên máy (không cần deploy)

```bash
# Cách 1: Mở trực tiếp
#   Nhấp đúp vào file index.html

# Cách 2: Chạy server local (tùy chọn)
python3 -m http.server 8080
# rồi mở trình duyệt tại http://localhost:8080
```

---

## 🌐 Deploy lên GitHub Pages

1. Tạo repo mới trên GitHub (ví dụ `aco-color-viewer`)
2. Upload file `index.html` vào repo
3. Vào **Settings → Pages → Source** chọn **Deploy from a branch** → nhánh `main` → thư mục `/ (root)`
4. Chờ 1–2 phút, truy cập: `https://<tên-người-dùng>.github.io/aco-color-viewer/`

> App là **một file HTML tự chứa** (không cần backend, không cần CDN) nên chạy được trên mọi dịch vụ hosting tĩnh: GitHub Pages, Netlify, Vercel, Cloudflare Pages...

---

## ❓ Câu hỏi thường gặp

**Dữ liệu của tôi có bị tải lên mạng không?**
Không. Ứng dụng xử lý hoàn toàn trên trình duyệt, không gửi dữ liệu ra ngoài.

**Mở file nhưng không thấy màu?**
Kiểm tra file có đúng định dạng `.aco` không. Một số phần mềm xuất file với cấu trúc khác.

**Trộn màu kiểu gì?**
Ứng dụng hòa trộn các màu theo tỷ lệ (trung bình có trọng số) — giống pha sơn. Kéo thanh trượt để màu nào "nặng" hơn.

**Làm sao trộn chỉ một phần màu trong file?**
Mở file ACO trong mục Trộn màu → click bỏ chọn màu không muốn → bấm "Thêm màu vào trộn".

---

## 📚 Hướng dẫn chi tiết

Xem file **[HUONG_DAN_SU_DUNG.md](HUONG_DAN_SU_DUNG.md)** để có hướng dẫn đầy đủ từng chức năng.

---

## 🛠 Công nghệ

- **HTML + CSS + JavaScript** thuần (Vanilla JS), không framework, không thư viện ngoài
- Xử lý nhị phân ACO bằng `DataView`, vẽ/export bằng Canvas API
- Hoàn toàn chạy phía client (client-side)

---

## 📄 Giấy phép

Tự do sử dụng cho mục đích cá nhân và công việc.
