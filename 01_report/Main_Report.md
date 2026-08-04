# Báo cáo Báo cáo Kiểm thử GUI, Usability & Cross-Platform (EMS System)

| **Thông tin** | **Chi tiết** |
|---|---|
| **Mã bài tập** | HW03-AI (Phiên bản EMS) |
| **Họ và tên sinh viên** | HỒ GIA HUY |
| **Mã số sinh viên** | 23127376 |
| **Lớp / Khóa** | 23KTPM2 / 23CLC |
| **Kịch bản phụ trách** | Kịch bản D — Người dùng yêu cầu Support và Admin hỗ trợ |
| **Các màn hình kiểm thử** | D1 (User Form), D2 (User History), D3 (Admin List), D4 (Admin Detail) |

---

## 1. Giới thiệu & Phạm vi Kiểm thử

Bài báo cáo này trình bày kết quả kiểm thử toàn diện giao diện người dùng (GUI), tính tiện dụng (Usability) và độ tương thích đa nền tảng (Cross-Platform) trên hệ thống **Event Management System (EMS)**. 

### Kịch bản được phân công: Kịch bản D (Support Request Lifecycle)
- **D1 (User Form):** Form tạo Support Request có đính kèm ảnh (User).
- **D2 (User History):** Trang "Yêu cầu của tôi" (My Requests) và xem chi tiết phản hồi (User).
- **D3 (Admin Requests):** Danh sách Support Requests Admin, chuyển tab Pending/Resolved và Tìm kiếm (Admin).
- **D4 (Admin Detail):** Chi tiết Support Request phía Admin kèm Lightbox ảnh và nội dung phản hồi.

---

## 2. Task 1 — GUI Checklist & Kết quả Thực thi (Task 1A & 1B)

### 2.1. Thiết kế Checklist dùng chung (Task 1A)
Nhóm đã xây dựng bộ **Shared GUI Checklist** gồm **45 mục kiểm thử** phủ đầy đủ 4 chiều giao diện (Interface Aspects - IA) dựa trên các nguyên lý Heuristic của Nielsen, Norman và Shneiderman:
- **IA-01 (Chuẩn UI chung):** Layout, canh lề, typography, màu sắc, i18n, empty/loading states (15 mục).
- **IA-02 (Forms):** Label, validation, vị trí báo lỗi, upload file, rich-text editor (15 mục).
- **IA-03 (Navigation):** Menu, breadcrumb, tab, sidebar, deep link, nút back (8 mục).
- **IA-04 (Feedback & State):** Toast, badge, dialog xác nhận, progress bar, real-time update (16 mục).

### 2.2. Kết quả Thực thi trên 4 Màn hình D1 - D4 (Task 1B)

| Màn hình | Số mục Passed | Số mục Failed | Số mục N/A | Tổng mục | Tỉ lệ Pass |
|---|---|---|---|---|---|
| **D1 (User Form)** | 28 | 5 | 12 | 45 | 84.8% |
| **D2 (User History)** | 26 | 4 | 15 | 45 | 86.7% |
| **D3 (Admin List)** | 27 | 6 | 12 | 45 | 81.8% |
| **D4 (Admin Detail)** | 29 | 3 | 13 | 45 | 90.6% |
| **Tổng thể Kịch bản D** | **110** | **18** | **52** | **180** | **85.9%** |

### 2.3. Các lỗi GUI tiêu biểu phát hiện được (Task 1B Bugs)
1. **Lỗi Outline Focus (IA02-12 — Failed):** Khi chuyển tab bằng phím Tab vào ô input hoặc danh sách request trên D1/D3, viền bao quanh không rõ ràng, màu sắc chói gây khó quan sát.
2. **Lỗi Cập nhật Real-time (IA04-14 — Failed):** Khi Admin duyệt/xử lý request ở D3, màn hình D2 phía User không tự động cập nhật trạng thái mà phải bấm F5 reload lại trang.
3. **Lỗi Breadcrumb & Navigation (IA03-01 — Failed):** Từ trang chi tiết D4 phía Admin không có nút quay lại (Back) hoặc Breadcrumb để trở về danh sách D3 một cách nhanh chóng.

---

## 3. Task 2 — Usability Testing với 5 Người dùng thật (Usability Report)

### 3.1. Kịch bản tác vụ & Tuyển chọn người tham gia
Đã tổ chức 5 phiên kiểm thử độc lập với 5 người dùng thật ngoài lớp học (Sinh viên, Khách tham gia, Quản trị viên). Người dùng thực hiện tác vụ tạo yêu cầu hỗ trợ sự kiện bị lỗi và theo dõi quá trình xử lý.

### 3.2. Bảng kết quả định lượng & Điểm SUS

| Người tham gia | Vai trò | Màn hình | Task Success | Time on Task | Số lần do dự | Điểm SUS (0-100) |
|---|---|---|---|---|---|---|
| P1 (Võ Lê Ngọc Hiếu) | Sinh viên | D1 + D2 | Complete | 1 phút 10s | 3 lần | 47.5 (Poor) |
| P2 (Đoàn Minh Trí) | Khách | D1 + D2 | Complete | 2 phút 00s | 2 lần | 60.0 (OK) |
| P3 (Đào Sỹ Duy Minh) | Sinh viên | D1 + D2 | Partial | 6 phút 00s | 6 lần | 75.0 (Good) |
| P4 (Lê Hoàng Minh Nhật) | Khách / Admin | D3 + D4 | Complete | 3 phút 00s | 0 lần | 67.5 (OK) |
| P5 (Nguyễn Trường Duy) | Sinh viên | D1 + D2 | Complete | 2 phút 15s | 2 lần | 62.5 (OK) |
| **Trung bình** | | | **80% Complete** | **2.8 phút** | **2.6 lần** | **62.5 / 100 (OK)** |

### 3.3. Các điểm đau Usability chính (Usability Pain Points)
- **Thiếu lối vào Support tại trang sự kiện:** Người dùng kỳ vọng nút báo lỗi ngay tại trang sự kiện thay vì phải tìm trên menu chính.
- **Rào cản ngôn ngữ Tiếng Anh:** Giao diện mặc định Tiếng Anh và nút chuyển đổi ngôn ngữ bằng lá cờ gây khó nhận biết cho người dùng mới.

---

## 4. Task 3 — Cross-Browser & Cross-Platform Testing

### 4.1. Ma trận Tương thích đã thực thi
Ma trận kiểm thử phủ 3 Hệ điều hành (Windows 11, macOS Sonoma, Android 14), 5 Trình duyệt (Chrome, Firefox, Edge, Safari, Opera) và 3 Loại thiết bị (Desktop, Tablet, Mobile Phone).

| Thiết bị / Hệ điều hành | Trình duyệt | Màn hình D1 | Màn hình D2 | Màn hình D3 | Màn hình D4 | Kết quả |
|---|---|---|---|---|---|---|
| Desktop Windows 11 | Chrome 126 | Pass | Pass | Pass | Pass | Đạt chuẩn |
| Desktop Windows 11 | Firefox 127 | Pass | Pass | Pass | Pass | Đạt chuẩn |
| Desktop Windows 11 | Edge 126 | Pass | Pass | Pass | Pass | Đạt chuẩn |
| Desktop macOS Sonoma | Safari 17 | Pass | Pass | Fail (Layout) | Pass | Tràn danh sách |
| Desktop macOS Sonoma | Opera 111 | Pass | Pass | Pass | Pass | Đạt chuẩn |
| Tablet iPadOS 17 | Safari Mobile | Pass | Fail (Scroll) | Pass | Pass | Vỡ thanh cuộn |
| Mobile Android 14 | Chrome Mobile | Fail (Responsive) | Pass | Fail (Filter) | Pass | Tràn form D1 |

### 4.2. Lỗi giao diện Cross-Platform tiêu biểu
- **Lỗi Responsive Form D1 trên Mobile (Android Chrome):** Các ô input và nút đính kèm ảnh bị vỡ khung, đè lên lề phải khi xem ở màn hình có chiều rộng < 380px.
---

## 5. Tổng hợp Findings & Khuyến nghị Cải tiến

### 5.1. Nhật ký Bug & Usability Findings Log
Toàn bộ 18 lỗi GUI và 4 điểm đau Usability đã được mã hóa đầy đủ tại tệp **`05_findings_log/Bug_Usability_Findings_Log.md`** và nộp thành công qua Google Form.

### 5.2. Kế hoạch hành động đề xuất (Action Plan)
1. **Ưu tiên 1 (Sửa gấp):** Khắc phục lỗi Responsive Form D1 trên điện thoại di động và sửa màu sắc Outline Focus.
2. **Ưu tiên 2 (Nâng cấp UX):** Thêm nút "Gửi Yêu cầu Hỗ trợ" trực tiếp vào trang chi tiết sự kiện và tối ưu nút đổi ngôn ngữ.
3. **Ưu tiên 3 (Tính năng):** Bổ sung tính năng Real-time Sync giữa giao diện Admin D3 và User D2.
