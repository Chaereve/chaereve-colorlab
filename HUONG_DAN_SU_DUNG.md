# 🎨 ACO Color Viewer Pro — Hướng dẫn sử dụng

Công cụ xem, trộn và xuất bảng màu Photoshop (`.aco`) chạy ngay trên trình duyệt.
**Không cần cài đặt, không cần tải dữ liệu lên mạng** — mọi thứ xử lý ngay trên máy bạn.

---

## Mục lục
1. [Bắt đầu](#1-bắt-đầu)
2. [Tab "Xem ACO"](#2-tab-xem-aco)
3. [Tab "Trộn màu"](#3-tab-trộn-màu)
4. [Xuất ảnh & dữ liệu](#4-xuất-ảnh--dữ-liệu)
5. [Lịch sử trộn](#5-lịch-sử-trộn)
6. [Giao diện sáng/tối](#6-giao-diện-sángtối)
7. [Câu hỏi thường gặp](#7-câu-hỏi-thường-gặp)

---

## 1. Bắt đầu

- Mở file `index.html` bằng bất kỳ trình duyệt nào (Chrome, Edge, Firefox, Safari…).
- Trang có **2 tab** chính ở đầu:
  - **📁 Xem ACO** — xem, sao chép, xuất bảng màu từ file `.aco`.
  - **🎨 Trộn màu** — pha trộn nhiều màu thành một màu mới.

---

## 2. Tab "Xem ACO"

### Mở file
- **Kéo thả** file `.aco` vào ô giữa màn hình, **hoặc** click vào ô để chọn file.
- Hỗ trợ file ACO **v1 và v2**, đọc được **tên màu** và các hệ màu RGB / HSB / CMYK / Lab / Grayscale.

### Xem màu
- Mỗi màu hiển thị dạng thẻ: **số thứ tự** (1, 2, 3…), ô màu, tên màu, mã HEX, giá trị RGB và hệ màu gốc.
- Số thứ tự đi theo **thứ tự trong file ACO**, giúp bạn dễ đối chiếu.

### Sao chép mã màu
- **Click vào thẻ màu** để copy mã (định dạng tùy chọn: HEX / RGB / HSL — chọn ở menu "HEX" trên thanh công cụ).
- Nút **📋 Sao chép tất cả** để copy toàn bộ màu dưới dạng: danh sách HEX, CSS Variables, SCSS, JSON hoặc RGB.

### Chọn nhiều màu
- Click dấu **✓** ở góc thẻ để chọn/bỏ chọn màu.
- Nút **☑ Chọn** → Chọn tất cả / Bỏ chọn / Đảo ngược.

### Tìm kiếm & sắp xếp
- Ô **🔍** tìm theo tên, mã HEX hoặc RGB.
- Menu sắp xếp: theo thứ tự gốc, sắc độ (Hue), độ sáng, độ bão hòa hoặc tên.

---

## 3. Tab "Trộn màu"

Tab này dùng **độc lập**, không cần mở ACO trước.

### Thêm màu vào danh sách trộn
Có 2 cách:
1. **Ô chọn màu** + nút "➕ Thêm màu này" — chọn bất kỳ màu nào.
2. **📁 Mở file ACO** — chọn file `.aco`, sau đó hiện **lưới chọn lọc**:
   - Mặc định tất cả màu được chọn (✓).
   - **Click vào ô màu** để loại bỏ những màu bạn **không muốn trộn**.
   - Nút **Chọn tất cả / Bỏ chọn / Đảo ngược**.
   - Bấm **"➕ Thêm N màu vào trộn"** để đưa các màu đã chọn vào.

### Chỉnh lại màu mà không cần tải lại file
- Bấm nút **🔁 Chỉnh lại màu** để **mở lại lưới chọn lọc của file ACO đã tải** (không phải up file lần nữa).
- Tích/bỏ tích rồi bấm "Thêm màu vào trộn" — ứng dụng sẽ **tự thêm màu mới và bỏ màu bạn đã bỏ chọn**.

### Tỷ lệ màu
- Tỷ lệ mỗi màu được **tự động chia đều** theo số lượng màu (ví dụ 4 màu → mỗi màu 25%).
- Nút **⚖️ Cân bằng tỷ lệ** để chia đều lại bất cứ lúc nào.
- **Kéo thanh trượt** để tăng/giảm tỷ lệ riêng từng màu — phần còn lại tự tính lại cho khớp 100%.

### Kết quả trộn
- Ô kết quả hiển thị màu đã trộn cùng mã **HEX / RGB / HSL**, cập nhật tức thời khi bạn đổi tỷ lệ.
- **📋 Copy HEX / RGB / HSL** để sao chép nhanh.
- **💾 Lưu vào lịch sử** để lưu lại màu vừa trộn.

---

## 4. Xuất ảnh & dữ liệu

Trong tab **Xem ACO**, chọn các màu muốn xuất rồi bấm **⬇ Xuất ảnh & dữ liệu**. Một cửa sổ cho phép:

- **Bố cục**: dải ngang / dải dọc / lưới (tùy số cột).
- **Kích thước ô** và **khoảng cách** giữa các ô.
- **Nhãn**: HEX / HEX + Tên / không nhãn.
- **Nền**: trắng hoặc trong suốt.
- **Xem trước** trực tiếp trước khi tải.

Các định dạng xuất:
| Định dạng | Mô tả |
|-----------|-------|
| 🖼 PNG | Ảnh bảng màu (nét cao) |
| 📐 SVG | Vector, chỉnh sửa được |
| 🎨 CSS | Biến màu `--color-1: #…;` |
| { } JSON | Dữ liệu màu có cấu trúc |
| 📄 TXT | Danh sách mã HEX, mỗi dòng một màu |

---

## 5. Lịch sử trộn

- Nằm ở cuối tab **Trộn màu**.
- Mỗi khi bạn **copy** hoặc **lưu** một màu trộn, màu đó tự thêm vào lịch sử.
- **Click vào ô màu** trong lịch sử để copy lại ngay.
- Nút **✕** xóa từng màu, nút **🗑 Xóa lịch sử** xóa toàn bộ.
- Lịch sử được **lưu tự động** trên trình duyệt (vẫn còn khi mở lại trang).

---

## 6. Cài đặt làm App (PWA)

Ứng dụng có thể cài thành app thật trên cả máy tính và điện thoại:

| Nền tảng | Cách cài |
|----------|----------|
| **Máy tính** (Chrome/Edge) | Mở link → bấm nút **📲** ở góc phải hoặc biểu tượng cài đặt trên thanh địa chỉ → **Install** |
| **Android** (Chrome) | Mở link → menu **⋮** → **Thêm vào Màn hình chính** |
| **iPhone/iPad** (Safari) | Mở link → nút **Chia sẻ** → **Thêm vào Màn hình chính** |

Sau khi cài: app có **icon riêng**, mở **cửa sổ độc lập** (không có thanh địa chỉ), và chạy được **cả khi không có mạng** (offline).

> **Yêu cầu:** app phải được mở qua **HTTPS** (link deploy như GitHub Pages/Netlify/Vercel). Không cài được khi mở file `file://` trực tiếp.

---

## 7. Giao diện sáng/tối

- Nút **🌙 / ☀️** ở góc phải trên để đổi giao diện.
- Lựa chọn của bạn được ghi nhớ cho những lần mở sau.

---

## 8. Câu hỏi thường gặp

**Hỏi:** Tôi mở file nhưng không thấy màu nào?
**Đáp:** Kiểm tra file có đúng định dạng `.aco` không. Một số file xuất từ phần mềm khác có thể dùng cấu trúc khác.

**Hỏi:** Dữ liệu của tôi có bị tải lên mạng không?
**Đáp:** Không. Ứng dụng chạy hoàn toàn trên trình duyệt, không gửi bất kỳ dữ liệu nào ra ngoài.

**Hỏi:** Trộn màu kiểu gì?
**Đáp:** Ứng dụng hòa trộn các màu theo tỷ lệ (trung bình có trọng số) — giống pha sơn. Kéo thanh trượt để màu nào đó "nặng" hơn.

**Hỏi:** Làm sao để trộn chỉ một phần màu trong file ACO?
**Đáp:** Bấm "📁 Mở file ACO", bỏ chọn (click) những màu không muốn, rồi bấm "Thêm màu vào trộn".
