# Tool By Khắc Phong · Nguồn Sileo

Nguồn công khai: https://nhokcrazy.github.io/khac-phong-repo/

Trong Sileo → Sources → +, dán URL trên rồi tìm **KP Auto**. Sau khi cập nhật, respring để nạp bản mới.

KP Auto **0.8.6 / build 26** có hai gói dành cho iOS 16:

- **Dopamine thường/rootless**: `iphoneos-arm64`, cần ElleKit.
- **Dopamine RootHide**: `iphoneos-arm64e`, cần RootHide và ElleKit.

Hai gói cùng ID `com.khacphong.auto`; Sileo chọn theo kiến trúc jailbreak. App/runner arm64 và ba dylib hệ thống universal arm64 + arm64e được build bằng Xcode 16.4, ký và kiểm tra từng slice.

Bản 0.8.6 đồng bộ giao diện Yamada Cyusen trên hai loại jailbreak, gồm DONE/FAIL và kết quả theo vùng chứa. Sửa lỗi bộ chạy không khởi động trên Dopamine thường. Khi tắt hẳn rồi mở lại tool, phiên mới về **Sẵn Sàng**, không tự chạy tiếp; cấu hình, DATA và kết quả đã lưu vẫn được giữ.

Đã cài và kiểm tra trực tiếp trên iPhone SE2: Dopamine thường/iOS 16.6.1 và Dopamine RootHide/iOS 16.0.2. Bộ chạy và kết nối DOM hoạt động trên cả hai máy. Các lượt kiểm tra trạng thái thành công, thất bại và đang chạy đều về Sẵn Sàng sau khi tắt/mở lại; trở lại cùng phiên đang chạy vẫn giữ lượt hiện tại. Người dùng đã xác nhận hai giao diện giống nhau. Chưa gửi đăng ký Cyusen thật trong lần kiểm tra.

Repository này chứa các gói phát hành và chỉ mục APT. Mã nguồn build được lưu trong repository riêng tư của chủ tài khoản.
