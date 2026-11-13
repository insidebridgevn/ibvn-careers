# IBVN Careers

Trang tuyển dụng của INSIDE BRIDGE VIETNAM (GitHub Pages).

- Giao diện: `index.html` (một file, không cần build).
- Dữ liệu: đọc trực tiếp từ Google Sheet tuyển dụng (tab **Jobs**, **Settings**) qua Apps Script.
- Ứng tuyển: form gửi về Apps Script → lưu dòng mới ở tab **Applications**, CV vào Drive, gửi email như cũ.

## Cấu hình

Mở `index.html`, tìm phần `CONFIG` ở đầu thẻ `<script>`:

```js
var API_URL = '';   // link /exec của Apps Script trang tuyển dụng
var ZALO_URL = 'https://zalo.me/g/wju1y4lhlnjsjofo7noc';   // link trong thông báo ghim
```

`API_URL` để trống thì trang chạy ở chế độ xem trước với dữ liệu mẫu.

## Thêm / sửa / đóng vị trí

Sửa trong Google Sheet, tab **Jobs** — không cần đụng code. Cột **Status** = `Open` thì hiện, `Closed` thì ẩn.
