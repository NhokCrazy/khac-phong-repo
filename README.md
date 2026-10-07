# Tool By Khắc Phong · Nguồn Sileo

Nguồn công khai: https://nhokcrazy.github.io/khac-phong-repo/

Trong Sileo → Sources → +, dán URL trên rồi tìm **KP Auto**.

KP Auto **0.3.1** có hai gói dành cho iOS 16:

- **Dopamine thường/rootless**: `iphoneos-arm64`, đường dẫn `/var/jb`, cần ElleKit.
- **Dopamine RootHide**: `iphoneos-arm64e`, đường dẫn RootHide, cần RootHide và ElleKit.

Hai gói cùng ID `com.khacphong.auto`; Sileo chọn theo kiến trúc của jailbreak. App/runner arm64 và hai dylib universal arm64 + arm64e được build bằng Xcode 16.4, ký và kiểm tra từng slice. Bản 0.3.1 chưa được kiểm thử chạy trực tiếp trên Dopamine thường hoặc thiết bị A12+.

Repository này chứa các gói phát hành và chỉ mục APT. Mã nguồn build được lưu trong repository riêng tư của chủ tài khoản.
