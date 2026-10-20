# Lexicology & Semantics – Group 5

Website học Chương 3: Cấu trúc từ và phương thức tạo từ, chuyển thể từ PowerPoint 189 slide do người dùng cung cấp.

## Nội dung và chức năng

- 7 chủ đề, 47 mục nội dung: từ, hình vị, phụ tố, chuyển loại, ghép từ, hòa trộn, rút gọn.
- Tiếng Việt, English hoặc song ngữ VI + EN; bản dịch và giải thích được biên soạn cho web.
- 46 câu luyện tập từ slide, lọc theo chủ đề, chấm điểm, đáp án và giải thích.
- Tìm kiếm không phân biệt dấu tiếng Việt; đánh dấu đã học và lưu tiến độ trên thiết bị bằng localStorage.
- Giao diện thích ứng điện thoại và máy tính, chế độ in/lưu PDF.
- Không cần cài đặt, không có thư viện hay dịch vụ bên ngoài. Mở trực tiếp `index.html` để học offline. Tải cả repo để dùng đường dẫn kho văn bản gốc.

## Mở web bằng GitHub Pages

Repo chưa bật Pages tại thời điểm tạo web. Chủ repo vào **Settings → Pages → Build and deployment**, chọn **Deploy from a branch → main → /(root) → Save**.

Sau khi GitHub triển khai thành công, địa chỉ dự kiến: https://duckxyz06.github.io/Lexiconlogy/

Đây là địa chỉ dự kiến, chưa phải xác nhận đã triển khai.

## Nguồn và biên tập

Tài liệu nguồn: *Black and White Modern Thesis Defense Presentation (6).pptx*, 189 slide. Bài học và câu hỏi ghi số slide để đối chiếu. Các slide lặp để hiện đáp án được gộp. Nội dung nằm trong ảnh về định nghĩa “word”, biến thể hình vị, biến hình/phái sinh và yếu tố Hy Lạp–La-tinh đã được đưa vào các bài tương ứng.

`source-slides.json` lưu văn bản trích xuất từ cả 189 slide để đối chiếu; không chứa hình ảnh và không phải bản sao đầy đủ của PowerPoint. Bản dịch tiếng Việt nằm trong nội dung bài học, không phải trong kho văn bản gốc này.

Tham chiếu cách trình bày: https://github.com/Duckxyz06/Phonology- (chuyển Việt/Anh và nội dung theo màu). Mã ứng dụng được viết riêng.

Các sửa đổi học thuật/biên tập được ghi ở mục **Nguồn & Nhóm 5**: sửa lỗi chính tả, căn lại đáp án cắt ngắn, gộp câu trùng, thay ví dụ microwave → mic thiếu rõ ràng, và ghi chú những phân loại tùy khung phân tích. Quan điểm của các học giả được ghi theo phần tóm lược trong slide, chưa đối chiếu trực tiếp với sách gốc.

Giảng viên: Lê Huỳnh Thanh Huy. Thành viên Nhóm 5: Trần Xuân Hương, Nguyễn Hồng Đào, Nguyễn Thị Anh Đào, Nguyễn Thị Như Ý, Nguyễn Nhật An Khương, Võ Trường Thịnh, Nguyễn Việt Đức.

## Kiểm tra

Chạy `node verify.mjs` (Node.js 18+). Bộ kiểm tra dùng DOM mô phỏng, kiểm tra chuyển ngôn ngữ, tìm kiếm, lọc đề, chấm điểm và lưu tiến độ. Chưa kiểm tra bố cục trên trình duyệt thật trong môi trường tạo web.

## Chỉnh sửa

Ứng dụng trong `index.html`, gồm CSS, dữ liệu `LESSONS`, dữ liệu `QUESTIONS` và JavaScript. Không có bước build. Khi thêm câu hỏi, `ans` là chỉ số lựa chọn đúng bắt đầu từ 0.
