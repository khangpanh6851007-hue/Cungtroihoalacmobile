# 🌌 Cung Trời Hóa Lạc – Ultra 2026

Ứng dụng web mô phỏng tích lũy **Năng Lượng Thiên Giới** và **Phước Đức**, với giao diện tối ưu cho điện thoại và máy tính.

## ✨ Tính năng

- 20 hoạt động thiện và 20 hoạt động ác.
- Theo dõi thanh Năng Lượng Thiên Giới và Phước Đức.
- Hệ thống danh hiệu và tiến trình thăng cấp.
- Điểm danh hằng ngày và phần thưởng.
- Thành tựu, thống kê và lịch sử hoạt động.
- Tùy chỉnh tên và giá trị hoạt động.
- Tìm kiếm hoạt động thiện/ác.
- Tự động lưu dữ liệu trong trình duyệt.
- Xuất và nhập bản sao lưu JSON.
- Giao diện Ultra 2026 responsive cho mobile và desktop.

## 📁 Cấu trúc repository

```text
.
├── index.html
├── README.md
└── .github/
    └── workflows/
        └── deploy.yml
```

> Đặt file ứng dụng HTML đã nâng cấp tại thư mục gốc repository và đặt tên chính xác là `index.html`. Không đặt file trong thư mục con nếu muốn GitHub Pages phục vụ trực tiếp từ artifact triển khai này.

## 🚀 Chạy trên máy

1. Tải hoặc clone repository.
2. Mở `index.html` bằng trình duyệt hiện đại.
3. Dữ liệu trò chơi được lưu trong bộ nhớ cục bộ của trình duyệt trên thiết bị đó.

Không cần cài đặt backend hoặc cơ sở dữ liệu để chạy các chức năng phía trình duyệt.

## 🌐 Triển khai GitHub Pages tự động

1. Tạo một repository trên GitHub.
2. Tải `index.html`, `README.md` và thư mục `.github/workflows/` lên repository.
3. Mở **Settings → Pages**.
4. Trong phần **Build and deployment**, chọn **GitHub Actions** làm nguồn triển khai.
5. Commit và push lên nhánh `main` (hoặc `master` nếu đã chỉnh workflow).
6. Mở tab **Actions** để theo dõi workflow `Deploy to GitHub Pages`.
7. Khi workflow hoàn tất, mở đường dẫn GitHub Pages hiển thị trong **Settings → Pages**.

Workflow nằm tại `.github/workflows/deploy.yml` và tự động chạy khi có push lên `main`, hoặc có thể chạy thủ công từ tab Actions.

### Nếu repository dùng nhánh khác

Mở `.github/workflows/deploy.yml`, sửa `branches` và điều kiện `push` từ `main` sang tên nhánh mặc định của repository.

## 💾 Lưu trữ dữ liệu

- Dữ liệu được lưu bằng `localStorage` trên trình duyệt.
- Dữ liệu không tự đồng bộ giữa các trình duyệt hoặc thiết bị.
- Dùng chức năng **Xuất Sao Lưu JSON** để lưu bản sao; dùng **Nhập Sao Lưu** để khôi phục.
- Xóa dữ liệu trang web hoặc dùng trình duyệt khác có thể làm mất dữ liệu cục bộ nếu chưa sao lưu.

## 🔐 Quyền GitHub Actions

Workflow cần các quyền tối thiểu để triển khai GitHub Pages:

- `contents: read`
- `pages: write`
- `id-token: write`

## 🛠️ Công nghệ

- HTML5
- CSS3
- JavaScript
- GitHub Actions
- GitHub Pages

## 📜 Ghi chú

Đây là ứng dụng chạy phía trình duyệt. Điểm số và danh hiệu là dữ liệu mô phỏng trong ứng dụng, không phải hệ thống xác thực hoặc lưu trữ tập trung.

---
**Cung Trời Hóa Lạc – Ultra 2026**
