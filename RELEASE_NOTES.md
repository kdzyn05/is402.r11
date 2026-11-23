# Bản nộp IS402 BT05

- Commit nguồn: `4b8aa3c5e4b8125063d8f43b7fdb366c66eb3285`.
- Gói nguồn gồm 309 tệp từ allowlist; SHA-256: `486ce78df9987769e383b2e763581a1239fcb3f6e28c9bc47f5faf924b125459`. File này được thêm sau khi xuất gói. Mã và tài liệu có phần do AI hỗ trợ.
- `putThumbnail` xử lý `409 BlobAlreadyExists` như lượt gửi lại, không ghi đè blob. `412` vẫn trả về `created: false`; các mã `409` khác vẫn báo lỗi. Lint đạt; `npm test` đạt 532, lỗi 0, bỏ qua 1 ca Terraform cần CLI và provider cache. Bộ test Blob/Function đạt 50/50.
- Bản nộp chỉ chứa mã nguồn, cấu hình mẫu và dữ liệu kiểm thử giả lập. Không kèm hồ sơ vận hành nội bộ, tài khoản demo, dữ liệu thật hoặc giá trị cấu hình môi trường. Dùng `docs/development.md` và `docs/testing.md` để chạy cục bộ. Các liên kết đến hồ sơ nội bộ không có đích trong bản nộp.
- Bản nộp không triển khai hay đổi phiên bản staging; kết quả tại chỗ không thay minh chứng Azure. Không áp dụng cấu hình hạ tầng mẫu vào một subscription đang sử dụng nếu chưa rà scope, quyền và chi phí.
