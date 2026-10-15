# Tool By Khắc Phong · Nguồn Sileo

Nguồn công khai: https://nhokcrazy.github.io/khac-phong-repo/

Trong Sileo → Sources → +, dán URL trên rồi tìm **KP Auto**. Người đã thêm nguồn chỉ cần làm mới nguồn, cập nhật KP Auto rồi **Respring** để nạp bản mới.

KP Auto **0.8.9 / build 29** có hai gói dành cho iOS 16:

- **Dopamine thường/rootless**: `iphoneos-arm64`, cần ElleKit.
- **Dopamine RootHide**: `iphoneos-arm64e`, cần RootHide và ElleKit.

Hai gói cùng ID `com.khacphong.auto`; Sileo chọn theo kiến trúc jailbreak. App/runner arm64 và ba dylib hệ thống universal arm64 + arm64e được build bằng Xcode 16.4, ký và kiểm tra từng slice.

Bản 0.8.9 sửa thời gian chờ IPC bị cắt ở 30 giây trong khi thao tác Crane có thể cần tới 40 giây. Bộ chạy nay giữ đủ cửa sổ chờ phản hồi 41 giây, vẫn giới hạn tối đa 45 giây; khi kết quả không rõ ràng vẫn dừng, không tự lặp thao tác đổi/tạo vùng chứa.

Bộ thu cảm ứng duyệt cả sự kiện con, với giới hạn số lượng/độ sâu và chống vòng lặp. Sau Respring, thao tác chạm thật khi mở và dùng KP Auto cung cấp định danh cảm ứng cho phiên mới.

Các trạng thái API `app.state.running`, `touchReady` và cờ hiển thị/ghi thao tác được trả về đúng kiểu boolean `true/false`, tránh việc một kịch bản so sánh chặt hiểu nhầm số `1` thành trạng thái chưa chạy. Hai loại jailbreak dùng chung API và cùng nội dung runtime JavaScript; có thể nhập cùng file kịch bản trên cả hai máy. Kịch bản vẫn cần đúng ứng dụng, trang, cấu hình, dữ liệu và các thành phần mà nó sử dụng.

Đã kiểm tra trực tiếp trên iPhone SE2 chạy Dopamine thường/iOS 16.6.1 và Dopamine RootHide/iOS 16.0.2: cài gói 0.8.9, chạy cùng file kiểm tra API, đối chiếu trạng thái ứng dụng, kết nối WebView/DOM và kiểm tra đọc trạng thái Crane. Bộ kiểm tra native xác nhận phản hồi Mach sau 35 giây và 57 kiểm tra kiểu boolean/JSON trên từng máy. Các kiểm tra này không gửi đăng ký, đặt mua hoặc thử toàn bộ nghiệp vụ của mọi website.

Khi tắt hẳn rồi mở lại tool, phiên mới về **Sẵn Sàng**, không tự chạy tiếp; cấu hình, DATA và DONE/FAIL đã lưu vẫn được giữ. Gói cập nhật giữ các kịch bản JS đã nhập trong thư mục Scripts; không kèm hoặc ghi đè kịch bản, tài khoản hay dữ liệu riêng của khách.

Repository này chứa các gói phát hành và chỉ mục APT. Mã nguồn build được lưu trong repository riêng tư của chủ tài khoản.
