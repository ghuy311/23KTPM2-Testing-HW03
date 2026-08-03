# Task Scenario — Kịch bản D (Support Request Lifecycle)

**Phạm vi màn hình kiểm thử (Kịch bản D):**
- **D1 (User Form):** Form tạo Support Request có đính kèm ảnh (User).
- **D2 (User History):** Trang "Yêu cầu của tôi" (My Requests) và xem chi tiết phản hồi (User).
- **D3 (Admin Requests):** Danh sách Support Requests Admin, chuyển tab Pending/Resolved và Tìm kiếm (Admin).

---

## 1. Hướng dẫn phân công màn hình theo phiên (Session Assignment)

Để đảm bảo phủ đủ cả 3 màn hình trong Kịch bản D theo đúng nguyên tắc 1 phiên kiểm thử 1 màn hình:
- **Màn hình D1 (Form tạo yêu cầu hỗ trợ):** Dành cho các phiên test phía Người dùng tạo ticket mới (VD: Session 1, Session 2, Session 3).
- **Màn hình D2 (Yêu cầu của tôi & Chi tiết phản hồi):** Dành cho phiên test phía Người dùng theo dõi và xem kết quả xử lý (VD: Session 4).
- **Màn hình D3 (Quản lý Support Requests phía Admin):** Dành cho phiên test phía Quản trị viên/Chuyên viên hỗ trợ kiểm tra danh sách, bộ lọc và tìm kiếm (VD: Session 5).

---

## 2. Kịch bản tác vụ chi tiết theo từng màn hình (Task Scenarios)

### Kịch bản A — Màn hình D1: Form tạo Support Request (User)
- **Bối cảnh đọc cho người tham gia:** "Bạn vừa cố đăng ký tham gia một sự kiện trên EMS nhưng bị hệ thống báo lỗi. Hãy gửi một yêu cầu hỗ trợ báo cáo sự cố này kèm ảnh chụp màn hình minh họa lỗi."
- **Nhiệm vụ (Task Goal):** Hoàn thành biểu mẫu "Tạo yêu cầu hỗ trợ" với đầy đủ thông tin bắt buộc và tệp đính kèm ảnh lỗi, sau đó nhấn nút gửi.
- **Tiêu chí thành công (Success Criteria):**
  - **Complete:** Điền đủ các trường, đính kèm ảnh thành công và gửi biểu mẫu thành công.
  - **Partial:** Gửi được biểu mẫu nhưng thiếu ảnh đính kèm hoặc cần gợi ý nút Submit.
  - **Fail:** Không gửi được biểu mẫu hoặc hủy bỏ giữa chừng.

---

### Kịch bản B — Màn hình D2: Danh sách Yêu cầu của tôi & Phản hồi (User)
- **Bối cảnh đọc cho người tham gia:** "Bạn đã gửi một yêu cầu hỗ trợ trước đó và muốn kiểm tra xem ban tổ chức/admin đã tiếp nhận và phản hồi yêu cầu của bạn hay chưa."
- **Nhiệm vụ (Task Goal):** Truy cập vào trang "Yêu cầu của tôi" (My Requests), định vị yêu cầu hỗ trợ vừa gửi, kiểm tra trạng thái (Pending/Resolved) và mở xem chi tiết nội dung phản hồi chính thức.
- **Tiêu chí thành công (Success Criteria):**
  - **Complete:** Tìm đúng trang My Requests, chọn đúng ticket và đọc được nội dung phản hồi/trạng thái không do dự.
  - **Partial:** Tìm được danh sách nhưng lúng túng hoặc cần gợi ý để mở chi tiết phản hồi.
  - **Fail:** Không tìm thấy trang danh sách yêu cầu cá nhân hoặc không thể xem chi tiết.

---

### Kịch bản C — Màn hình D3: Danh sách Support Requests Admin (Admin)
- **Bối cảnh đọc cho người tham gia:** "Với vai trò Quản trị viên hệ thống, bạn cần kiểm tra toàn bộ danh sách các yêu cầu hỗ trợ gửi đến từ người dùng để xử lý."
- **Nhiệm vụ (Task Goal):** Truy cập trang Quản lý Yêu cầu Hỗ trợ Admin, thực hiện chuyển đổi giữa các tab "Pending" (Chờ xử lý) và "Resolved" (Đã xử lý), sau đó sử dụng thanh Tìm kiếm (Search) để tra cứu một yêu cầu hỗ trợ theo từ khóa hoặc mã người dùng.
- **Tiêu chí thành công (Success Criteria):**
  - **Complete:** Chuyển đổi linh hoạt giữa 2 tab Pending/Resolved và dùng thanh search lọc đúng kết quả.
  - **Partial:** Chuyển được tab nhưng thao tác tìm kiếm bị lúng túng hoặc cần chỉ vị trí thanh search.
  - **Fail:** Không tìm thấy trang quản lý support phía Admin hoặc không thao tác được bộ lọc/search.

---

## 3. Metrics đo lường trong từng phiên (Metrics)

- **Task Success Rate:** Complete / Partial / Fail (theo tiêu chí màn hình được phân công).
- **Time on Task:** Thời gian tính từ khi bắt đầu đọc kịch bản màn hình đến khi hoàn thành mục tiêu.
- **Số lỗi / Lần do dự:** Đếm số lần người dùng dừng lại, nhấp sai, hoặc bày tỏ phân vân trong phiên.
- **Phản hồi SUS / UEQ-S:** Cho người tham gia điền biểu mẫu khảo sát ngay khi kết thúc phiên.

---

## 4. Probe Questions (hỏi sau khi hoàn thành task, trước khi điền SUS)

1. Điều gì rõ ràng nhất trong lúc bạn tạo yêu cầu hỗ trợ?
2. Có bước nào khiến bạn phân vân hoặc không chắc mình đang làm đúng không?
3. Khi yêu cầu gặp lỗi (nếu có xảy ra), bạn có hiểu ngay cần làm gì tiếp theo không?
4. Bạn có tin tưởng là yêu cầu của mình đã được ghi nhận và sẽ được xử lý không? Vì sao?
5. Nếu phải mô tả tốc độ thao tác này cho bạn bè, bạn sẽ nói gì?
