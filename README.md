# Tool By Khắc Phong · Nguồn Sileo

Nguồn công khai: https://nhokcrazy.github.io/khac-phong-repo/

Trong Sileo → Sources → +, dán URL trên rồi tìm **KP Auto**.

KP Auto **0.8.5 / build 25** có hai gói dành cho iOS 16:

- **Dopamine thường/rootless**: `iphoneos-arm64`, đường dẫn `/var/jb`, cần ElleKit.
- **Dopamine RootHide**: `iphoneos-arm64e`, cần RootHide và ElleKit.

Khi ghi kịch bản mới, mở menu logo → **CHỌN KẾT THÚC** → chọn chữ hoặc nút làm dấu hiệu hoàn tất. Tool lưu dấu hiệu và kết thúc ghi. Khi chạy lại, tool chờ đúng dấu hiệu xuất hiện ổn định trước khi hoàn tất lượt; không nhấn nút được chọn.

Hai gói cùng ID `com.khacphong.auto`; Sileo chọn theo kiến trúc của jailbreak. App/runner arm64 và ba dylib hệ thống universal arm64 + arm64e được build bằng Xcode 16.4, ký và kiểm tra từng slice.

Bản RootHide 0.8.5 đã cài trên SE2/iOS 16.0.2 và xác nhận controller sẵn sàng. Chưa xác minh thao tác chọn trên máy thật vì ứng dụng thử không mở được. Bản rootless chưa được chạy trên thiết bị thật.

Repository này chứa các gói phát hành và chỉ mục APT. Mã nguồn build được lưu trong repository riêng tư của chủ tài khoản.
