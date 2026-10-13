# Máy tính khoa học web — giai đoạn khởi đầu

Đây là bộ khung chạy được để phát triển dần theo tài liệu Casio fx-580VN X; chưa phải bản giả lập đầy đủ hoặc tương đương firmware gốc.

## Chạy
- Mở `index.html` trong trình duyệt để thử các phép tính cơ bản. Service Worker yêu cầu HTTP/HTTPS.
- Để thử offline/PWA và kiểm thử ổn định, phục vụ thư mục qua máy chủ tĩnh hoặc GitHub Pages.
- Mở `tests/runner.html` để chạy bộ kiểm thử lõi trong trình duyệt.

## Triển khai GitHub Pages
1. Tạo repository và tải toàn bộ tệp/thư mục lên nhánh `main`.
2. Vào Settings → Pages.
3. Chọn Deploy from a branch, branch `main`, folder `/ (root)`, rồi Save.
4. Mở URL Pages được GitHub cung cấp. Truy cập trang ít nhất một lần khi có mạng trước khi thử offline.

## Giới hạn hiện tại
- Chỉ một tập con của Calculate được triển khai; giao diện hiện có chủ đích vô hiệu hóa các chế độ khác.
- Chưa có phân số chính xác, biểu thức MathI/MathO đầy đủ, số phức, ma trận, vectơ, thống kê, phân phối, phương trình, bất phương trình, Verify hay Ratio.
- Chưa đối chiếu trực tiếp với máy vật lý; kết quả số thực được tính bằng JavaScript Number.
- Các phím giao diện là bố cục phát triển, chưa khẳng định khớp từng vị trí với bàn phím vật lý.
- Service Worker cache các tài nguyên cốt lõi; khi phát hành phiên bản mới cần tăng CACHE trong service-worker.js.
