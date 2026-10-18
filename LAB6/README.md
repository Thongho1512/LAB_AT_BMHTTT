Hồ Ngọc Thái Thông
1150080077
Lab 6: XÁC THỰC ACTIVE DIRECTORY VÀ CHÍNH SÁCH TRUY CẬP TRÊN pfSense

- triển khai máy ảo Sophos Firewall trên VMware với 4 giao diện mạng (WAN, MGMT, LAN, DMZ). Cấu hình xong IP tĩnh cho firewall và các máy ảo thành phần gồm Domain Controller (DC01), Client-A, Client-B và máy chủ DMZ-WEB.
- Khai báo thành công máy chủ Active Directory (DC01) vào Sophos thông qua giao thức LDAP
- Bật tính năng Captive Portal cho vùng LAN trong Device Access và chỉ định AD làm nguồn xác thực, buộc Client-A và Client-B phải đăng nhập bằng tài khoản domain (sv_a, sv_b) trước khi ra mạng.
- Tạo các IP Host để định danh IP tĩnh cho người dùng (CLIENT_A, CLIENT_B) và các trang web kiểm thử trong DMZ (JOB_SITE, SOCIAL_SITE, RESTRICTED_SITE).
- Gom nhóm máy trạm thành IP Host Group (POLICY_CLIENTS) và tạo lịch trình Schedule (LUNCH_WINDOW) để chuẩn bị gán vào chính sách.
- Thực thi Firewall Rules (Kịch bản 1 - 3): Đã tạo các rule xử lý từ trên xuống (top-down) và bật Log để ghi nhận
