# Tool By Khắc Phong · Nguồn Sileo

Nguồn công khai: https://nhokcrazy.github.io/khac-phong-repo/

Trong Sileo → Sources → +, dán URL trên rồi tìm **KP Auto**. Sau khi cập nhật, respring để nạp bản mới.

KP Auto **0.8.7 / build 27** có hai gói dành cho iOS 16:

- **Dopamine thường/rootless**: `iphoneos-arm64`, cần ElleKit.
- **Dopamine RootHide**: `iphoneos-arm64e`, cần RootHide và ElleKit.

Hai gói cùng ID `com.khacphong.auto`; Sileo chọn theo kiến trúc jailbreak. App/runner arm64 và ba dylib hệ thống universal arm64 + arm64e được build bằng Xcode 16.4, ký và kiểm tra từng slice.

Bản 0.8.7 đồng bộ giao diện Settings của Yamada CYUSEN 1.0.8 trên cả hai loại jailbreak. Mục Tenpo hỗ trợ chọn nhiều cửa hàng, tìm kiếm và lọc theo tỉnh/khu vực. Với file CYUSEN 1.0.8 đã nhập, danh sách có 338 Tenpo; tích các cửa hàng muốn dùng rồi **LƯU** danh sách và **LƯU** Settings.

Khi tắt hẳn rồi mở lại tool, phiên mới về **Sẵn Sàng**, không tự chạy tiếp; cấu hình, DATA và DONE/FAIL đã lưu vẫn được giữ. Gói cập nhật KP Auto giữ các kịch bản JS đã nhập trong thư mục Scripts; không kèm hoặc ghi đè file CYUSEN của khách.

Phần giao diện Tenpo đã được kiểm tra trực tiếp trên Dopamine thường và RootHide trước lần phát hành này. Các kiểm tra mở lại sau thành công, thất bại và đang chạy xác nhận phiên mới về Sẵn Sàng và giữ cấu hình/kết quả. Hai gói DEB 0.8.7 được kiểm tra cấu trúc, checksum, kiến trúc và chữ ký; chưa được cài thử trong lượt xuất bản này.

Repository này chứa các gói phát hành và chỉ mục APT. Mã nguồn build được lưu trong repository riêng tư của chủ tài khoản.
