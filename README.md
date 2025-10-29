# Tra Cứu Hoạt Động CLB KCMC

Ứng dụng web để tra cứu thông tin hoạt động của các thành viên Câu lạc bộ Khoa học Máy tính (CLB KCMC).

## Tính Năng

- 🔍 **Tìm kiếm linh hoạt**: Tra cứu theo Họ tên, MSSV (Mã số sinh viên), hoặc Mã thành viên (KCMC00...)
- 📱 **Responsive Design**: Tương thích với tất cả các thiết bị (máy tính, tablet, điện thoại)
- 📊 **Hiển thị chi tiết**: Thông tin rõ ràng, dễ đọc với các mục:
  - Thông tin cá nhân (Mã thành viên, MSSV, Họ tên, Lớp, Khoa)
  - Trạng thái tham gia (Đóng góp, Sinh hoạt, Cài máy, Hoạt động bảo tàng)
- ✨ **Giao diện hiện đại**: UI/UX được tối ưu với gradient, shadow effects và hover states

## Hướng Dẫn Sử Dụng

### Yêu Cầu
- File `clb_kcmc_data.json` chứa dữ liệu thành viên (đặt cùng thư mục với `index.html`)

### Cài Đặt
1. Đặt file `index.html` và `clb_kcmc_data.json` trong cùng một thư mục
2. Mở file `index.html` trong trình duyệt web
3. Nhập Họ tên, MSSV hoặc Mã thành viên để tìm kiếm

### Cách Tìm Kiếm
- **Theo Họ tên**: Nhập một phần tên (không cần dấu), ví dụ: "Lộc", "Thanh"
- **Theo MSSV**: Nhập mã số sinh viên, ví dụ: "2024001"
- **Theo Mã thành viên**: Nhập mã CLB, ví dụ: "KCMC001"

## Cấu Trúc Dữ Liệu

File `clb_kcmc_data.json` cần có cấu trúc sau:
```json
[
  {
    "STT": 1,
    "Mã thành viên": "KCMC001",
    "Mã số sinh viên": "2024001",
    "Họ và tên": "Tạ Thành Lộc",
    "Lớp": "CT01",
    "Khoa": "Công nghệ thông tin",
    "Đóng góp trung thu": "Có",
    "Sinh hoạt Câu lạc bộ": "Có",
    "Tham gia cài máy tính tại Trung tâm học liệu - Thực hành": "Có",
    "Tham gia hoạt động tại bảo tàng tỉnh An Giang - Cơ sở 1": "Không"
  },
  ...
]
```

## Công Nghệ Sử Dụng

- **HTML5**: Cấu trúc trang
- **CSS3**: Responsive design với media queries
- **JavaScript**: Tính năng tìm kiếm và xử lý dữ liệu
  - Tìm kiếm không phân biệt chữ hoa/thường
  - Bỏ qua dấu khi tìm kiếm
  - Ưu tiên kết quả khớp chính xác

## Responsive Breakpoints

- **Desktop** (768px+): Hiển thị 2 cột
- **Tablet** (480px - 768px): Hiển thị 1 cột
- **Mobile** (dưới 480px): Font nhỏ, tối ưu cho small screens

## Giao Diện

- Màu sắc: Xanh dương (#2563eb) và xanh đậm (#1e3a8a)
- Font size: 32px (tiêu đề), 18px (giá trị), responsive trên mobile
- Gradient background: Hiệu ứng giảm dần giữa hai màu
- Card-based layout: Thông tin được nhóm trong các box riêng biệt

## Tác Giả

CLB KCMC - Khoa Công nghệ Thông tin

## Giấy Phép

MIT License
