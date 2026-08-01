# Task Scenario — Kịch bản D (Support Request)

**Màn hình liên quan:** D1 (Tạo yêu cầu hỗ trợ), D2 (Yêu cầu hỗ trợ — danh sách & chi tiết)
**Vai trò người tham gia:** User (student/lecturer/guest) — không dùng vai Admin

---

## Bối cảnh trình bày cho người tham gia (đọc trước khi bắt đầu)

> "Bạn vừa cố đăng ký tham gia một sự kiện trên hệ thống EMS nhưng không thành công — hệ thống báo lỗi và không ghi nhận lượt đăng ký của bạn. Hãy dùng chức năng hỗ trợ trong EMS để báo cáo vấn đề này, sau đó kiểm tra xem yêu cầu của bạn đang ở trạng thái nào.
>
> Tôi đang test sản phẩm, không phải test bạn — cứ thoải mái, nếu có gì khó hiểu hoặc không chắc thì cứ nói ra suy nghĩ của bạn trong lúc làm (think aloud). Tôi sẽ không can thiệp trừ khi bạn hoàn toàn bế tắc."

## Task Scenario (mục tiêu, không phải bước bấm)

> **"Báo rằng một lượt đăng ký sự kiện của bạn bị lỗi, và theo dõi đến khi yêu cầu đó được xử lý."**

*(Không đọc gợi ý các bước cụ thể như "vào menu avatar", "bấm nút Tạo yêu cầu" — để tự người dùng khám phá luồng.)*

---

## Success Criteria

| Mức độ | Tiêu chí |
|---|---|
| **Complete** | Tạo được yêu cầu hỗ trợ với đủ 3 trường bắt buộc (Loại yêu cầu, Vấn đề cần hỗ trợ, Mô tả chi tiết), gửi thành công, sau đó tự tìm được và mở lại đúng yêu cầu đó trong danh sách "Yêu cầu hỗ trợ" để xem trạng thái |
| **Partial** | Tạo được yêu cầu nhưng cần gợi ý mới tìm ra cách xem lại trạng thái, hoặc bỏ sót/điền sai 1 trường không bắt buộc |
| **Fail** | Không gửi được yêu cầu, hoặc không tìm được nơi xem lại trạng thái yêu cầu đã gửi kể cả sau khi được gợi ý |

## Metrics đo lường (ghi trong lúc quan sát)

- **Task success**: Complete / Partial / Fail (theo bảng trên)
- **Time on task**: tính từ lúc bắt đầu đọc scenario đến khi xác nhận thấy trạng thái yêu cầu
- **Số lỗi / lần do dự**: đếm số lần người dùng dừng lại, quay lui, click nhầm, hoặc nói "ủa/không biết bấm đâu"
- **SUS hoặc UEQ-S**: phát sau khi kết thúc task (dùng Google Form khảo sát)

## Probe Questions (hỏi sau khi hoàn thành task, trước khi điền SUS)

1. Điều gì rõ ràng nhất trong lúc bạn tạo yêu cầu hỗ trợ?
2. Có bước nào khiến bạn phân vân hoặc không chắc mình đang làm đúng không?
3. Khi yêu cầu gặp lỗi (nếu có xảy ra), bạn có hiểu ngay cần làm gì tiếp theo không?
4. Bạn có tin tưởng là yêu cầu của mình đã được ghi nhận và sẽ được xử lý không? Vì sao?
5. Nếu phải mô tả tốc độ thao tác này cho bạn bè, bạn sẽ nói gì?

---

## Ghi chú cho người quan sát (bạn)

- Không gợi ý trước "vào avatar để tìm Yêu cầu hỗ trợ" — đây chính là điểm bạn đã tìm ra là **Failed** ở Task 1B (IA03-01), nên khả năng cao người tham gia cũng sẽ lúng túng tại đây — đúng là điều cần quan sát.
- Vấn đề cần hỗ trợ / Mô tả chi tiết: để người tham gia tự nghĩ nội dung, không đọc placeholder mẫu cho họ (placeholder trên UI là gợi ý sẵn, nhưng nên xem họ có tự viết được không hay copy y nguyên ví dụ — cũng là 1 tín hiệu về clarity của placeholder).
- Ghi lại rõ nếu người dùng bị vướng ở đúng những điểm đã phát hiện lỗi tại Task 1B (VD: không có preview ảnh, Enter không submit, double-submit...) — đây là bằng chứng chéo củng cố mức độ nghiêm trọng thực tế của các bug đó.
