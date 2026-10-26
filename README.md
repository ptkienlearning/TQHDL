# Bán lẻ thông minh — Dashboard tương tác (tiếng Việt)

Website tĩnh phân tích 240 giao dịch bán lẻ tại TP.HCM năm 2025. Không cần backend, framework, cài đặt hay build. Biểu đồ được vẽ trực tiếp bằng SVG và JavaScript nên không phụ thuộc CDN biểu đồ.

## Tệp trong dự án
- `index.html`: cấu trúc giao diện tiếng Việt
- `style.css`: giao diện responsive
- `app.js`: lọc dữ liệu, KPI, biểu đồ SVG, tương tác, bảng, xuất CSV/JSON
- `data.js`: dữ liệu giao dịch nhúng trong trang

## Chạy thử
Mở `index.html` bằng trình duyệt hiện đại. Dữ liệu và biểu đồ chạy cục bộ; kết nối Internet chỉ cần nếu muốn tải phông chữ Google Fonts.

## Tương tác có sẵn
- Lọc theo cửa hàng, ngành hàng, nhóm khách, tháng, ngày bắt đầu/kết thúc, mức giảm giá, từ khóa, giao dịch lỗ và điểm đánh giá.
- Nhấp vào thanh biểu đồ để lọc theo cửa hàng/ngành hàng/nhóm khách; nhấp vào tháng trên biểu đồ đường để lọc tháng.
- Nhấp vào điểm trên biểu đồ phân tán để xem chi tiết giao dịch; mở chi tiết từ bảng và nhảy đến giao dịch tương ứng.
- Sắp xếp bảng theo tiêu đề cột, chọn số dòng mỗi trang, chuyển trang, xuất dữ liệu lọc ra CSV hoặc JSON.
- Biểu đồ SVG không phụ thuộc Chart.js CDN, tránh tình trạng trang không tải được thư viện nên biểu đồ trống.

## Deploy GitHub Pages
1. Tạo repository tên `<MSHV>_DataViz_Midterm` theo yêu cầu bài tập.
2. Upload bốn tệp vào thư mục gốc: `index.html`, `style.css`, `app.js`, `data.js`.
3. Vào **Settings → Pages → Deploy from a branch**, chọn `main` và `/(root)`, rồi Save.
4. Đợi deploy hoàn tất và mở URL do GitHub Pages cung cấp.
5. Kiểm tra bộ lọc, biểu đồ, bảng và chức năng tải CSV/JSON.

## Lưu ý dữ liệu
Các biểu đồ và KPI được tính từ tập dữ liệu hiện hành. Tiền được hiển thị theo đơn vị số liệu gốc; ký hiệu “tr” trong biểu đồ nghĩa là triệu đơn vị dữ liệu, không tự khẳng định loại tiền tệ. Các mối quan hệ trong dữ liệu không tự chứng minh quan hệ nhân quả.
