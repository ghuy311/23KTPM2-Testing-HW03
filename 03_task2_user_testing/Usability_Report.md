# Usability Report — Kịch bản D: Support Request Lifecycle (EMS)

## 1. Giới thiệu & Phạm vi Kiểm thử

Báo cáo này tổng hợp kết quả **Usability Testing (Kiểm thử tính tiện dụng)** thực hiện trên hệ thống **EMS (Event Management System)**, thuộc **Kịch bản D (Support Request Lifecycle)**. 

### Phạm vi màn hình kiểm thử:
- **D1 (User Form):** Form tạo Support Request có đính kèm ảnh (User).
- **D2 (User History):** Trang "Yêu cầu của tôi" (My Requests) và xem chi tiết phản hồi (User).
- **D3 (Admin Requests):** Danh sách Support Requests Admin, chuyển tab Pending/Resolved và Tìm kiếm (Admin).
- **D4 (Admin Detail):** Chi tiết Support Request phía Admin kèm Lightbox ảnh và nội dung phản hồi.

---

## 2. Kịch bản Tác vụ (Task Scenario)

Kịch bản tác vụ được thiết kế theo phương pháp hướng mục tiêu (goal-oriented task design) tuân thủ tiêu chuẩn ISO 9241-11:

> **Nhiệm vụ cho người dùng (User):** "Bạn vừa cố gắng đăng ký tham gia một sự kiện học thuật trên hệ thống EMS nhưng bị báo lỗi. Hãy tìm cách gửi một yêu cầu hỗ trợ báo cáo sự cố này kèm thông tin chi tiết, sau đó theo dõi trạng thái cho đến khi nhận được phản hồi xử lý."
>
> **Nhiệm vụ cho quản trị viên (Admin):** "Với vai trò Admin, hãy truy cập vào danh sách các yêu cầu hỗ trợ, lọc các yêu cầu đang chờ xử lý (Pending), tìm kiếm yêu cầu vừa gửi và tiến hành kiểm tra chi tiết để phản hồi."

---

## 3. Bảng thông tin người tham gia (Participants Table)

Đã tiến hành tuyển chọn và thực hiện 5 phiên kiểm thử với 5 người dùng thật đại diện cho các đối tượng mục tiêu (Sinh viên, Khách tham gia, Quản trị viên).

| Mã | Họ và tên | Vai trò thực tế | Liên hệ (đã che) | Ngày test | Màn hình | Ghi chú phiên |
|---|---|---|---|---|---|---|
| P1 | Võ Lê Ngọc Hiếu | Sinh viên | 079****305 | 03/08/2027 | D1 + D2 | Hoàn thành task, vướng mắc ở focus màu form |
| P2 | Đoàn Minh Trí | Khách | 070****639 | 03/08/2027 | D1 + D2 | Hoàn thành task, loay hoay tìm menu hỗ trợ |
| P3 | Đào Sỹ Duy Minh | Sinh viên | 23122***@student.hcmus.edu.vn | 03/08/2027 | D1 + D2 | Cần gợi ý (Partial), vướng về ngôn ngữ Tiếng Anh |
| P4 | Lê Hoàng Minh Nhật | Khách (Role Admin) | 033****004 | 03/08/2027 | D3 + D4 | Thao tác mượt mà phía Admin |
| P5 | Nguyễn Trường Duy | Sinh viên | 033****833 | 03/08/2027 | D1 + D2 | Thắc mắc vì sao trang sự kiện không có nút hỗ trợ |

---

## 4. Kết quả & Chỉ số đo lường (Metrics)

### 4.1. Bảng chỉ số định lượng

| Chỉ số (Metric) | Kết quả ghi nhận | Ghi chú & Đánh giá |
|---|---|---|
| **Tỷ lệ thành công (Task Success Rate)** | **80% Complete**, **20% Partial** | 4/5 người tự hoàn thành tác vụ; 1/5 người (P3) cần gợi ý tìm menu hỗ trợ |
| **Thời gian trung bình (Time on Task)** | **2.8 phút** (từ 1 phút 10s đến 6 phút) | P1 làm nhanh nhất (1m10s), P3 tốn nhiều thời gian nhất (6m) do rào cản ngôn ngữ |
| **Số lần do dự / lỗi thao tác trung bình** | **2.6 lần / phiên** | Các lỗi chủ yếu: nhấp tìm hỗ trợ ở trang sự kiện, bấm vào ô input nhưng không thấy con trỏ |
| **Điểm SUS trung bình (System Usability Scale)** | **62.5 / 100** | Mức **OK** (Bangor et al., 2008) — Hệ thống dùng được nhưng cần cải tiến UX |

### 4.2. Chi tiết điểm SUS từng người tham gia

| Người tham gia | C1 | C2 | C3 | C4 | C5 | C6 | C7 | C8 | C9 | C10 | Điểm quy đổi (0-40) | Điểm SUS (0-100) | Xếp loại |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| P1 | 3 | 2 | 4 | 3 | 2 | 2 | 2 | 3 | 1 | 3 | 19 | **47.5** | Poor |
| P2 | 5 | 3 | 3 | 2 | 4 | 3 | 4 | 4 | 3 | 3 | 24 | **60.0** | OK |
| P3 | 5 | 1 | 4 | 2 | 4 | 2 | 4 | 2 | 3 | 3 | 30 | **75.0** | Good |
| P4 | 4 | 2 | 3 | 1 | 4 | 2 | 3 | 2 | 3 | 3 | 27 | **67.5** | OK |
| P5 | 4 | 3 | 4 | 2 | 3 | 4 | 3 | 2 | 4 | 2 | 25 | **62.5** | OK |
| **Trung bình** | **4.2** | **2.2** | **3.6** | **2.0** | **3.4** | **2.6** | **3.2** | **2.6** | **2.8** | **2.8** | **25.0** | **62.5** | **OK** |

---

## 5. Phân tích Usability Findings & Điểm đau (Pain Points)

Các điểm đau phát hiện qua 5 phiên test được phân loại và xếp hạng theo mức độ nghiêm trọng (Severity từ 0 đến 4 theo Nielsen):

### Severity 3: Mức độ Nghiêm trọng Cao (Major Usability Issue)
1. **Thiếu nút "Yêu cầu hỗ trợ" trực tiếp trên trang chi tiết sự kiện (D1/B2)**
   - **Mô tả:** Cả 3/5 người dùng (P1, P3, P5) đều có xu hướng tìm kiếm nút báo lỗi/hỗ trợ ngay trên trang sự kiện bị lỗi đăng ký. Việc bắt người dùng phải quay ra menu chính để tìm "Support Request" gây ngắt quãng trải nghiệm.
   - **Tác động:** Tăng thời gian làm task (Time on task của P3 lên 6 phút), gây do dự và thắc mắc.

2. **Màu sắc hiệu ứng Focus trên các ô nhập liệu Form tạo Request quá mờ / khó nhìn (D1)**
   - **Mô tả:** Khi nhấp chuột vào ô Input Form D1 (Title, Content), viền focus không đổi màu rõ ràng và thiếu con trỏ nhấp nháy (`|`) khiến người dùng (P1, P2) phân vân không biết đã chọn ô nhập hay chưa.
   - **Tác động:** Tạo cảm giác ứng dụng bị đơ (unresponsive), người dùng nhấp lại nhiều lần.

### Severity 2: Mức độ Nghiêm trọng Trung bình (Medium Usability Issue)
3. **Rào cản ngôn ngữ mặc định (i18n) và Nút chuyển ngôn ngữ khó nhận biết (Global)**
   - **Mô tả:** Giao diện mặc định hiển thị bằng tiếng Anh, trong khi người dùng P3 cần giao diện tiếng Việt. Nút đổi ngôn ngữ được thiết kế dạng biểu tượng lá cờ nhỏ trên header khiến người dùng khó nhận ra.
   - **Tác động:** Người dùng tốn nhiều thời gian đọc hiểu và tìm kiếm tính năng.

4. **Sự nhầm lẫn giữa Menu Support Request dành cho Admin và User (D3/D4)**
   - **Mô tả:** Khi truy cập với tài khoản Admin (phiên P4), tên danh mục trên menu không phân biệt rõ ràng giữa trang theo dõi ticket cá nhân (User) và trang quản lý ticket toàn hệ thống (Admin).
   - **Tác động:** Admin phải bấm thử vào menu mới xác định đúng trang quản lý.

---

## 6. Khuyến nghị Cải tiến UX/UI (Actionable Recommendations)

| STT | Vấn đề Usability | Mức độ | Khuyến nghị cải tiến | Ưu tiên |
|---|---|---|---|---|
| 1 | Thiếu điểm truy cập Support ở sự kiện | Severity 3 | Thêm nút "Báo lỗi / Yêu cầu hỗ trợ" ngay trong trang chi tiết sự kiện kèm đính kèm ID sự kiện tự động. | Cao |
| 2 | Outline Focus mờ trên Form input | Severity 3 | Thêm đường viền outline tương phản cao (primary accent color) và hiển thị con trỏ con trỏ gõ rõ ràng khi focus. | Cao |
| 3 | Nút đổi ngôn ngữ khó thấy | Severity 2 | Thay nút lá cờ bằng Menu Dropdown chọn ngôn ngữ rõ ràng ("Tiếng Việt / English") tại Header. | Trung bình |
| 4 | Phân biệt menu Admin vs User | Severity 2 | Đổi tên menu Admin thành "Quản lý Support Ticket (Admin)" và đưa vào phân vùng Quản trị riêng. | Trung bình |

---

## 7. Nhật ký chuyển tiếp (Findings Transfer Log)

Toàn bộ các phát hiện usability trên đã được mã hóa và chuyển tiếp đầy đủ vào tệp **Bug & Usability Findings Log** (`05_findings_log/Bug_Usability_Findings_Log.md`) cũng như nộp lên hệ thống Google Form theo đúng quy định.