# KP Auto 0.9.7

Bộ chạy giải phóng bộ nhớ tạm sau từng lệnh native và mỗi vòng chờ, tránh
cộng dồn các đối tượng tạm trong lượt CHECK nhiều tài khoản. Bổ sung biên nhận
dừng native không chứa tài khoản, mật khẩu hoặc nội dung trang để kiểm tra sự cố.

CHECK JavaScript 1.0.13 được cập nhật riêng, không nhúng trong gói DEB.
Lỗi đã xác định ở từng tài khoản được lưu FAIL rồi chuyển sang tài khoản kế
sau khi xác nhận đóng Chrome và chế độ máy bay OFF. DATA và vùng chứa của tài
khoản lỗi được giữ để kiểm tra; thao tác Crane hoặc mạng chưa rõ vẫn dừng để
đối chiếu, không tự lặp lại.

Giữ popup CHECK nhỏ phía trên, hiển thị bước và thời gian đang chạy; dùng
cài đặt tự khóa hiện tại của iPhone. Giữ các bản sửa Chrome, Crane, CSV,
báo cáo CHECK với key che một nửa và hỗ trợ Yamada/CYUSEN.
Giữ DATA, cấu hình, lịch sử, kết quả, kịch bản và license khi cập nhật.

Chọn đúng gói RootHide hoặc Dopamine rootless trên iOS 16. Gói native không
chứa webhook, tài khoản hoặc dữ liệu khách hàng.
