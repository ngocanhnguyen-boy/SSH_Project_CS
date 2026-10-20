# SSH_Project_ANM
Bảo vệ truy cập từ xa bằng SSH và kênh truyền an toàn bởi 3 sinh viên UTH

# Đồ án Lab: Bảo vệ truy cập từ xa bằng SSH và Kênh truyền an toàn (UTH)

## Thành viên nhóm & Phân công công việc
1. **Sinh viên 1 (Hạ tầng & Sơ đồ):**
   - Dựng sơ đồ mạng trên VMware (địa chỉ IP Server, Client).
   - Thiết lập baseline và chuẩn bị môi trường máy ảo Linux ban đầu.
2. **Sinh viên 2 (Cấu hình & Bảo mật):**
   - Cài đặt và cấu hình OpenSSH (Xác thực bằng khóa, tắt đăng nhập mật khẩu, tắt root trực tiếp).
   - Cấu hình tường lửa (UFW/nftables) hạn chế nguồn truy cập quản trị.
3. **Sinh viên 3 (Kiểm thử & Báo cáo):**
   - Dùng Wireshark/tcpdump bắt và so sánh gói tin.
   - Thực hiện test kịch bản cho phép (Allow) và từ chối (Deny), thu thập log và chụp ảnh minh chứng.

---

## Roadmap (Lộ trình thực hiện)

- [ ] **Giai đoạn 1: Chuẩn bị & Thiết kế (SV1)**
  - Cài đặt máy ảo VMware (Ubuntu Server & Client).
  - Hoàn thiện sơ đồ mạng và tài liệu thiết kế ban đầu.
- [ ] **Giai đoạn 2: Cấu hình & Hardening hệ thống (SV2)**
  - Tạo cặp khóa SSH (`ssh-keygen`), cấu hình `sshd_config`.
  - Thiết lập tường lửa UFW/nftables để lọc IP truy cập.
- [ ] **Giai đoạn 3: Kiểm thử, Bắt gói tin & Tổng hợp (SV3)**
  - Dùng Wireshark so sánh lưu lượng.
  - Test thực tế các trường hợp đăng nhập thành công/thất bại.
  - Hoàn thiện file báo cáo chi tiết và đẩy lên GitHub nộp bài.
