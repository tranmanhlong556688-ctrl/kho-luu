# NHIỆM VỤ CODEX CLOUD — ML TỰ ĐỘNG HÓA V9.2

## 1. Mục tiêu

Nâng cấp website `mltudonghoa.pro.vn` từ V9.1 lên V9.2, giữ nguyên toàn bộ chức năng đang chạy tốt, bổ sung hai bài hướng dẫn có khả năng thu hút khách hàng và tăng mức độ nổi bật của dịch vụ viết phần mềm/tạo website theo yêu cầu.

Không deploy công khai và không merge vào `main` trước khi Minh duyệt.

## 2. Mốc nguồn bắt buộc

Nguồn chuẩn là toàn bộ nội dung đã giải nén từ:

`ML_TU_DONG_HOA_V91_EMAIL_PRO_FINAL_DEPLOY_VERIFIED.zip`

Thông tin đối chiếu:

- Tổng số file V9.1: 153.
- SHA-256 ZIP: `3191a13b3fc0411c2c637a368f02573f109c0c0439f57757c7beeede4a1f38a1`.
- Email duy nhất được sử dụng: `lienhe@mltudonghoa.pro.vn`.
- Không khôi phục khối đã xóa khỏi `gioi-thieu.html`: “Sơ đồ bổ sung / Bộ công cụ được chọn theo từng loại việc / Sơ đồ bộ công cụ ML Tự Động Hóa theo từng loại việc”.

Nếu chưa có đủ nguồn V9.1 thì dừng chỉnh sửa mã, ghi rõ blocker và không dựng lại website bằng phỏng đoán.

## 3. Nhánh làm việc

- Làm việc trên `codex/v9.2`.
- Commit nhỏ, mô tả rõ phạm vi.
- Không ghi đè file tải xuống, video, ảnh, công cụ ZIP hoặc dữ liệu mẫu hiện có.

## 4. Hạng mục V9.2

### 4.1. Bài hướng dẫn 1

Tạo file:

`huong-dan-dien-du-lieu-excel-vao-pdf-tu-dong.html`

Nội dung phải bao gồm:

- Nêu bài toán thực tế: lấy dữ liệu theo từng dòng Excel và điền đúng trường/vị trí trong PDF.
- Đối tượng: hành chính, nhân sự, kế toán, QA/QC, an toàn và nhà máy.
- Phân biệt PDF có trường biểu mẫu và PDF chỉ là nền ảnh/trang tĩnh.
- Quy trình: chuẩn hóa Excel → ánh xạ trường/toạ độ → xem trước → xuất trên bản sao → kiểm tra → ghi log.
- Ví dụ minh họa, không dùng dữ liệu cá nhân thật.
- Các lỗi thường gặp: font tiếng Việt/繁體中文, lệch vị trí, trang xoay, sai kích thước, dữ liệu trống, ghi đè file.
- Checklist nghiệm thu và cảnh báo bảo mật.
- CTA: gửi 2–5 file mẫu đã ẩn dữ liệu hoặc video thao tác 1–3 phút.
- SEO title, meta description, canonical, Open Graph, JSON-LD Article/Breadcrumb phù hợp cấu trúc hiện tại.

### 4.2. Bài hướng dẫn 2

Tạo file:

`huong-dan-chuan-hoa-du-lieu-truoc-khi-nhap-erp.html`

Nội dung phải bao gồm:

- Vấn đề dữ liệu trước ERP: sai định dạng ngày/số, khoảng trắng, mã thiếu số 0, ký tự ẩn, trùng dòng, cột bắt buộc trống, mã không thuộc danh mục.
- Quy trình: sao lưu → định nghĩa schema/quy tắc → chuẩn hóa → kiểm tra danh mục → tách lỗi → đối chiếu tổng → xuất file nhập → lưu log.
- Ví dụ cho nhà máy, kho, mua hàng, nhân sự hoặc kế toán; ghi rõ “Ví dụ minh họa”.
- Không khuyến khích tự động nhập ERP khi chưa có bước xác nhận.
- Checklist nghiệm thu, rollback và bảo mật.
- CTA giống bài 1.
- SEO title, meta description, canonical, Open Graph, JSON-LD Article/Breadcrumb.

### 4.3. Tích hợp vào website

- Thêm hai bài vào `huong-dan.html` dưới dạng bài hoàn chỉnh, không còn nằm trong mục “Chủ đề sẽ được bổ sung”.
- Thẻ bài phải cùng cấu trúc và phong cách với 7 bài hiện có.
- Cập nhật bộ lọc/tìm kiếm JavaScript nếu cấu trúc hiện tại yêu cầu.
- Thêm internal link hợp lý từ trang chủ, trang dự án hoặc bài liên quan; không nhồi từ khóa.
- Cập nhật `sitemap.xml` và mọi danh mục/manifest liên quan.
- Kiểm tra breadcrumb, header, footer, CTA mobile và liên kết quay lại.

### 4.4. Làm nổi bật dịch vụ mới

Bổ sung hợp lý, không phóng đại:

- Viết phần mềm Windows theo yêu cầu.
- Tạo website theo yêu cầu.

Ưu tiên chỉnh tại trang chủ, giới thiệu dịch vụ và liên hệ. Nội dung theo cấu trúc vấn đề → cách xử lý → kết quả có thể kiểm tra → CTA. Không biến phần mở đầu thành danh sách công nghệ.

## 5. Yêu cầu nội dung và thiết kế

- Tiếng Việt tự nhiên, chính tả chuẩn, giọng B2B thực tế.
- Không bịa tên khách hàng, đánh giá, ROI, thời gian tiết kiệm hoặc thành tích.
- Ví dụ giả lập phải ghi rõ “Ví dụ minh họa”.
- Giữ nhận diện xanh đậm/xanh dương/xanh ngọc và bố cục responsive hiện có.
- Ảnh phải nhẹ, sắc nét, không đánh số, không có chữ sai và có `alt` phù hợp.
- Ưu tiên WebP; không làm tăng đáng kể dung lượng trang.

## 6. QA bắt buộc

Tạo script kiểm tra tự động khi phù hợp và thực hiện tối thiểu:

1. Mọi HTML phân tích được, không thiếu thẻ chính nghiêm trọng.
2. Không có tài nguyên/liên kết nội bộ bị thiếu.
3. Không có anchor nội bộ hỏng.
4. JavaScript không lỗi cú pháp.
5. CSS cân bằng và không gây tràn ngang ở 390 px.
6. Hai bài mới có title/meta/canonical/OG/JSON-LD/breadcrumb.
7. `sitemap.xml` hợp lệ và chứa hai URL mới.
8. Không còn email cũ; email chính thức xuất hiện đúng nơi.
9. Không có nội dung đã yêu cầu xóa khỏi trang giới thiệu.
10. Kiểm tra desktop và mobile bằng local HTTP server, không chỉ mở `file://`.

## 7. Đầu ra

Trên nhánh `codex/v9.2`, tạo:

- Toàn bộ mã nguồn V9.2.
- `CHANGELOG_V92.md`.
- `BAO_CAO_QA_V92.md` ghi số file/trang/link đã kiểm tra và các giới hạn còn lại.
- `ML_TU_DONG_HOA_V92_FINAL_DEPLOY.zip`, đóng gói đúng cấp thư mục gốc để tải lên Cloudflare Pages.
- Pull request dạng draft từ `codex/v9.2` vào `main` để Minh xem; không tự merge.

## 8. Tiêu chí hoàn thành

Chỉ đánh dấu hoàn thành khi:

- Hai bài mới mở và hiển thị đúng.
- Danh mục hướng dẫn, tìm kiếm/bộ lọc và sitemap đã cập nhật.
- Các trang chính không bị hỏng giao diện hoặc chức năng.
- Báo cáo QA không còn lỗi nghiêm trọng.
- ZIP deploy được tạo và kiểm tra lại cấu trúc.
- Pull request vẫn ở trạng thái chờ Minh duyệt.
