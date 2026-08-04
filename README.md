# HW03 – GUI & Usability Testing trên EMS (Event Management System)

| **Thông tin bài nộp** | **Chi tiết** |
|---|---|
| **Họ và tên sinh viên** | HỒ GIA HUY |
| **Mã số sinh viên** | 23127376 |
| **Lớp / Khóa** | 23KTPM2 / 23CLC |
| **Kịch bản phụ trách** | Kịch bản D — Người dùng yêu cầu Support và Admin hỗ trợ |
| **Tự đánh giá điểm (Self-Assessed Grade)** | **090 / 100** |
| **Tên file nộp bài (.zip)** | `23127376_HW03_AI_GUIUsability_EMS_090.zip` |

---

## 1. Bảng tự đánh giá (Self-Evaluation Table)

*Tham chiếu theo Mục 16 của đề bài HW03:*

| STT | Tiêu chí đánh giá | Điểm tối đa | Tự đánh giá | Ghi chú hoàn thành |
|---|---|:---:|:---:|---|
| **1a** | **Task 1A — Shared GUI Checklist** (>40 mục, IA-01…IA-04 + References + Prompts) | 15 | **15** | Đã hoàn thành 45 mục phủ 4 Interface Aspects trong folder `00_group/` |
| **1b** | **Task 1B — Thực thi Checklist** (Chạy trên 4 màn hình D1-D4 + Bug Report) | 15 | **15** | Đã thực thi 180 lượt kiểm thử trên D1, D2, D3, D4 trong folder `02_task1b_checklist_execution/` |
| **2** | **Task 2 — User Testing** (5 người dùng thật + 5 phiên + Usability Report) | 25 | **25** | Đã chạy 5 phiên test thật, thu thập metrics, điểm SUS (62.5) và hoàn thành `03_task2_user_testing/Usability_Report.md` |
| **3** | **Task 3 — Cross-Platform** (3 OS × 5 Browsers × 3 Devices) | 25 | **25** | Đã hoàn thành ma trận tương thích và ảnh minh chứng có overlay MSSV trong `04_task3_cross_platform/` |
| **4** | **Log Findings & Google Form** (Gửi form + Log tổng hợp) | 10 | **10** | Đã tổng hợp đầy đủ 18 lỗi GUI và 4 Usability Findings trong `05_findings_log/Bug_Usability_Findings_Log.md` |
| **5** | **Agent Skills** (Skill tự động hóa + Video Demo) | 10 | **0** | Không thực hiện Agent Skill theo lựa chọn cá nhân |
| **TỔNG** | **Tổng điểm bài nộp** | **100** | **090 / 100** | **Đạt chuẩn 90/100 điểm** |

---

## 2. Tóm tắt kết quả kiểm thử (Test Summary)

### 2.1. Phạm vi & Kịch bản
- **Kịch bản phụ trách:** Kịch bản D (Support Request Lifecycle).
- **Các màn hình kiểm thử (4 màn hình):**
  1. `D1 (User Form)`: Form tạo Support Request có đính kèm ảnh phía người dùng.
  2. `D2 (User History)`: Trang "Yêu cầu của tôi" (My Requests) và xem phản hồi phía người dùng.
  3. `D3 (Admin Requests)`: Danh sách Support Requests, lọc Pending/Resolved phía Admin.
  4. `D4 (Admin Detail)`: Chi tiết Support Request kèm Lightbox ảnh và phản hồi phía Admin.

### 2.2. Kết quả Task 1 (GUI Checklist Execution)
- **Số mục Checklist thiết kế:** 45 mục (IA-01: 15 mục, IA-02: 15 mục, IA-03: 8 mục, IA-04: 16 mục).
- **Tổng số lượt kiểm thử thực thi:** 180 lượt (4 màn hình x 45 mục).
- **Kết quả:** **110 Passed** (85.9%), **18 Failed**, **52 N/A**.
- **Tổng số lỗi GUI phát hiện:** 18 lỗi.

### 2.3. Kết quả Task 2 (Usability Testing)
- **Số người tham gia kiểm thử:** 5 người dùng thật ngoài lớp học (P1 đến P5).
- **Tỉ lệ hoàn thành tác vụ (Task Success Rate):** **80% Complete**, **20% Partial**.
- **Thời gian hoàn thành trung bình (Time on Task):** **2.8 phút** / phiên.
- **Số lần do dự / lỗi thao tác trung bình:** **2.6 lần** / phiên.
- **Điểm SUS trung bình (System Usability Scale):** **62.5 / 100** (Xếp loại **OK** theo Bangor et al., 2008).
- **Phát hiện Usability:** 4 điểm đau chính (2 phát hiện Severity 3, 2 phát hiện Severity 2).

### 2.4. Kết quả Task 3 (Cross-Browser / Cross-Platform)
- **Độ phủ ma trận tương thích:** Phủ 100% theo yêu cầu (3 OS: Windows 11, macOS Sonoma, Android 14; 5 Browsers: Chrome, Firefox, Edge, Safari, Opera; 3 Thiết bị: Desktop, Tablet, Mobile Phone).
- **Lỗi giao diện Cross-Platform:** Phát hiện vỡ khung Form D1 trên Chrome Mobile Android và lỗi cuộn bộ lọc D3 trên Safari iPadOS.

---

## 3. Cấu trúc Thư mục Bài nộp

```
23127376_HW03_AI_GUIUsability_EMS_090/
├── 00_group/                       # Sản phẩm dùng chung cấp nhóm (Task 1A)
│   ├── Shared_GUI_Checklist.md     # Checklist GUI 45 mục (IA-01...IA-04)
│   └── References_and_Prompts.md   # Nguồn tham khảo & Prompt AI
├── 01_report/                      # Báo cáo chính
│   ├── Main_Report.md              # Báo cáo tổng hợp Task 1B, 2, 3
│   └── screenshots/                # Ảnh & Video bằng chứng kiểm thử
├── 02_task1b_checklist_execution/  # Thực thi Checklist (Task 1B)
│   └── Checklist_Results_D1-D4.md  # Kết quả chạy checklist 4 màn hình
├── 03_task2_user_testing/          # User Testing & Usability Report (Task 2)
│   ├── Task_Scenario.md            # Kịch bản tác vụ hướng mục tiêu
│   ├── Participants_Table.md       # Danh sách 5 người dùng thật (đã che)
│   ├── SUS_Questionnaire.md        # Bảng tính điểm SUS chi tiết (62.5)
│   ├── Usability_Report.md         # Báo cáo phân tích Usability
│   └── Session_Notes/              # Ghi chú chi tiết 5 phiên test (session_1..5)
├── 04_task3_cross_platform/        # Cross-Browser & Cross-Platform (Task 3)
│   ├── Compatibility_Matrix.md     # Ma trận tương thích 3 OS x 5 Browsers x 3 Devices
│   └── screenshots/                # Ảnh chụp minh chứng có overlay MSSV
├── 05_findings_log/                # Nhật ký lỗi tổng hợp
│   └── Bug_Usability_Findings_Log.md # Log gộp lỗi GUI & Usability
├── 06_ai_audit/                    # Phụ lục AI Audit & Critique
│   ├── AI_Audit_Report.md          # Log sử dụng AI đầy đủ
│   └── AI_Critique.md              # Đoạn phản biện AI (200-300 từ)
├── 08_git_log/                     # Nhật ký Commit Git
│   └── commit_log.txt              # Lịch sử commit Git
└── README.md                       # Trang tổng quan & Bảng tự đánh giá điểm
```