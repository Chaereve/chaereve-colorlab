# 🎨 ACO Color Viewer Pro

> [🇬🇧 English](README.md) · **🇻🇳 Tiếng Việt**

Công cụ **xem, trộn và xuất bảng màu Photoshop (`.aco`)** — chạy **ngay trên trình duyệt**. Không cần cài đặt, không cần đăng ký, không tải dữ liệu lên mạng.

> Mọi dữ liệu được xử lý **hoàn toàn cục bộ** trên máy/điện thoại của bạn.

**🌐 Giao diện song ngữ:** app có sẵn nút chuyển **Tiếng Việt ↔ English** (nút `EN` / `VI` ở góc phải trên).

---

## ✨ Tính năng

### 📁 Xem ACO
- Kéo thả (hoặc click) file `.aco` để mở.
- Hỗ trợ **ACO v1 & v2**, đọc được **tên màu** và các hệ màu RGB / HSB / CMYK / Lab / Grayscale.
- Mỗi màu hiển thị **số thứ tự**, tên màu, HEX, RGB và hệ màu gốc.
- **Tìm kiếm** theo tên/HEX/RGB và **sắp xếp** theo sắc độ, độ sáng, bão hòa, tên.

### 📋 Sao chép
- Click thẻ màu để copy mã (**HEX / RGB / HSL** — tùy chọn).
- **Copy tất cả** dưới dạng: danh sách HEX, CSS variables, SCSS, JSON, RGB.

### 🎨 Trộn màu (dùng độc lập — không cần mở ACO)
- Thêm màu bằng **ô chọn màu** hoặc **mở file ACO** ngay trong tab này.
- Lưới chọn lọc giúp **loại bỏ màu không muốn trộn** bằng một click.
- **Chỉnh lại lựa chọn** mà không cần tải lại file.
- Tỷ lệ **tự động chia đều** theo số lượng màu; kéo thanh trượt để chỉnh riêng.
- **Lịch sử trộn** tự lưu, click để copy lại.

### 🎲 Random màu (cho từng thành viên)
- Sinh 1–100 màu ngẫu nhiên cho từng "thành viên", hoàn toàn ngẫu nhiên hoặc theo họ màu (đỏ / cam / vàng / xanh lá / cyan / xanh dương / tím / hồng), có chế độ không trùng màu.

### 🛠 Công cụ thiết kế
- **Palette Generator** — complementary / analogous / triadic / split / tetradic.
- **Gradient Generator** — gradient CSS tuyến tính/hướng tâm, copy mã CSS.
- **Contrast Checker** — tỷ lệ tương phản WCAG kèm huy hiệu AA/AAA.
- **Color Blindness Preview** — protanopia / deuteranopia / tritanopia / grayscale.
- **Image → Palette / Chấm màu** — chấm vào ảnh lấy màu, hoặc trích màu chủ đạo.
- **Bảng chi tiết màu** — HEX / RGB / HSL / HSV / CMYK / Lab, độ sáng, tương phản.
- **Phát hiện trùng lặp** và **tìm màu tương tự**.

### ⬇ Xuất
- **PNG / SVG / CSS / JSON / TXT** với tùy chọn bố cục, kích thước, nhãn, nền (kể cả trong suốt).
- **Xuất .aco** (v2, có tên màu) từ các màu đã chọn.

### 🌙 Giao diện
- Chủ đề **tối / sáng** (mặc định tối).
- **Chuyển ngôn ngữ: Tiếng Việt / English**.
- Animation mượt, giao diện ưu tiên mobile (nav dưới cùng, bottom-sheet, nút to vừa tay).

### 📲 Cài làm app (PWA)
- Cài được trên **máy tính (Windows/macOS/Linux)** và **điện thoại (Android/iOS)**.
- Có icon riêng, mở cửa sổ độc lập, chạy **offline**.

### 🖥 Bản desktop (.exe)
- Đóng gói thành **bộ cài Windows** bằng Electron — xem thư mục `electron-app/`.

---

## 🚀 Cách dùng

### Trên máy tính / điện thoại
Mở `index.html` bằng trình duyệt bất kỳ (nhấp đúp), hoặc truy cập link đã deploy.

### Quy trình nhanh
1. Mở tab **📁 Xem ACO** → kéo thả file `.aco`.
2. Click màu để copy, hoặc tick nhiều màu để xuất.
3. Mở tab **🎨 Trộn màu** → thêm màu → xem kết quả trộn ngay.
4. Bấm **⬇ Xuất ảnh & dữ liệu** để tải bảng màu.

---

## 🌐 Chuyển ngôn ngữ

Bấm nút **`EN` / `VI`** (cạnh nút sáng/tối, góc phải trên) để đổi toàn bộ giao diện giữa **tiếng Anh** và **tiếng Việt**. Lựa chọn được ghi nhớ.

---

## 📲 Cài làm app (PWA)

Sau khi app deploy (qua HTTPS), bạn có thể cài thành app thật:

| Nền tảng | Cách cài |
|----------|----------|
| **Máy tính** (Chrome/Edge) | Mở link → nút **📲** hoặc biểu tượng cài đặt trên thanh địa chỉ → **Install** |
| **Android** (Chrome) | Mở link → menu **⋮** → **Thêm vào Màn hình chính** |
| **iPhone/iPad** (Safari) | Mở link → nút **Chia sẻ** → **Thêm vào Màn hình chính** |

> **Lưu ý:** PWA cần phục vụ qua **HTTPS** (GitHub Pages, Netlify, Vercel đều có sẵn). Không cài được khi mở `file://` trực tiếp.

---

## 🖥 Chạy thử local

```bash
# Cách 1: nhấp đúp index.html
# Cách 2: server local (tùy chọn)
python3 -m http.server 8080
# rồi mở http://localhost:8080
```

---

## 🌍 Deploy lên GitHub Pages

1. Tạo repo mới trên GitHub (ví dụ `aco-color-viewer`).
2. Upload nội dung thư mục `aco-color-viewer/` (kể cả thư mục `icons/`).
3. Vào **Settings → Pages → Source** → **Deploy from a branch** → nhánh `main`, thư mục `/ (root)` → **Save**.
4. Chờ 1–2 phút, truy cập: `https://<tên-người-dùng>.github.io/aco-color-viewer/`

---

## ❓ FAQ

**Dữ liệu có bị tải lên mạng không?**
Không. App chạy hoàn toàn trên trình duyệt.

**Mở file không thấy màu?**
Kiểm tra file có đúng `.aco` không. Một số phần mềm xuất ACO cấu trúc khác.

**Trộn màu kiểu gì?**
Pha theo tỷ lệ (trung bình có trọng số) — giống pha sơn. Kéo thanh trượt để màu "nặng" hơn.

**Muốn trộn một phần màu trong file?**
Mở ACO ở tab **Trộn màu** → bỏ chọn màu không muốn → bấm **Thêm màu vào trộn**.

---

## 📚 Hướng dẫn

- **Tiếng Việt:** [HUONG_DAN_SU_DUNG.md](HUONG_DAN_SU_DUNG.md)
- **English:** [USER_GUIDE.md](USER_GUIDE.md)
- **Từng bước (deploy + build .exe):** [HUONG_DAN_TUNG_BUOC.md](HUONG_DAN_TUNG_BUOC.md)

---

## 🛠 Công nghệ

- **HTML + CSS + JavaScript** thuần (Vanilla JS), không framework, không thư viện ngoài.
- Đọc nhị phân ACO bằng `DataView`, vẽ/xuất bằng Canvas API.
- Chạy hoàn toàn phía client.

---

## 📄 Giấy phép

Tự do sử dụng cho mục đích cá nhân và công việc.
