# AI Audit Report — Mẫu 5 mục cho mỗi Artifact

*Phụ lục bắt buộc đính kèm cho mọi bài tập có dùng AI (HW#01–HW#06, Seminar).*
*Tài liệu được biên soạn lại từ Med Kharbach, PhD (2026) — Mẫu Chính sách Sử dụng AI cho Giáo dục Đại học.*
*Giấy phép CC BY-NC-SA 4.0. Phiên bản này được FIT@HCMUS điều chỉnh cho môn CS423 / CSC15003 Kiểm chứng Phần mềm.*

---

## 1. Thông tin Sinh viên

| Mục | Giá trị |
| :--- | :--- |
| **Họ tên sinh viên (in hoa):** |HỒ GIA HUY |
| **MSSV:** | 23127376 |
| **Lớp / Khoá:** |23KTPM2 / 23CLC |
| **Mã bài tập (ví dụ HW#00, HW#02):** |HW03 |
| **Ngày làm bài:** |29/07/2026 |
| **Công cụ AI đã dùng:** | Gemini, Claude |
| **Công cụ AI đã dùng:** | `[X] Có`  `[] Không` |

---

## 2. Hướng dẫn (đọc trước khi điền)
* Thêm 1 hàng cho mỗi artifact AI sinh (test case, script, checklist, OpenAPI spec, JMeter plan…).
* Dán nguyên văn prompt — **KHÔNG** paraphrase.
* Dán nguyên văn output AI (hoặc kèm screenshot có chú thích trong báo cáo).
* Gắn nhãn: `VALID` / `INVALID` / `INCOMPLETE`.
* Lý do phải dẫn chiếu slide, mục ISTQB, hoặc RFC kỹ thuật.
* Hiển thị bản sửa với phần thay đổi được tô sáng.
* *Hàng mẫu in nghiêng — thay trước khi nộp.*

---

## 3. Bảng Audit — 1 hàng / artifact

| (1) Prompt + Công cụ | (2) Output AI | (3) Verdict | (4) Lý do (ISTQB) | (5) Bản SV sửa |
| :--- | :--- | :--- | :--- | :--- |
| **Artifact #1** <br> Công cụ : Gemini <br> Thời gian : 20:21 30/7/2026 <br> Prompt : " Độ tương phản màu sắc (Contrast Ratio) giữa chữ và nền đủ cao để dễ đọc (Cater to Universal Usability)"| Provided a structured list of tools to evaluate Color Contrast Ratio for Universal Usability, categorized by manual testing (WebAIM, Coolors), browser-based DOM testing (Chrome DevTools, WAVE, Lighthouse), and automated CI/CD integration (axe-core, pa11y).  |Valid | | |
| **Artifact #2** <br> Công cụ: Claude (Sonnet 5) <br> Thời gian: 01/08/2026 <br> Prompt: "để hình dựng cho tôi Task_Scenario.md, tôi gửi ảnh D1 (form tạo request) và D2 (danh sách + chi tiết request)" (kèm 2 ảnh chụp màn hình EMS thật) | Dựng `Task_Scenario.md` gồm: bối cảnh đọc cho người tham gia, 1 task scenario dạng mục tiêu (goal-oriented, không liệt kê bước bấm) dựa trên tình huống mẫu có sẵn trong placeholder UI ("Không thể đăng ký tham gia sự kiện"), bảng Success Criteria (Complete/Partial/Fail), danh sách metrics cần đo, 5 probe questions, và ghi chú riêng cho người quan sát liên kết với 2 bug đã tìm ở Task 1B (IA03-01). | Valid | Scenario bám sát nguyên tắc goal-oriented task design (không rò rỉ bước thao tác, tránh dẫn dắt hành vi người tham gia — theo khuyến nghị usability testing chuẩn ISO 9241-11 về đo lường effectiveness/efficiency/satisfaction một cách khách quan). Việc không gợi ý trước điểm vào "Yêu cầu hỗ trợ" là chủ đích để quan sát tự nhiên hành vi thật, không phải AI bỏ sót. | Chưa chỉnh sửa nội dung scenario; sẽ tinh chỉnh câu chữ sau khi chạy pilot (bước bắt buộc trước khi test 5 người chính thức) nếu phát hiện gây hiểu lầm. |
| **Artifact #3** <br> Công cụ: Claude (Sonnet 5) <br> Thời gian: 01/08/2026 <br> Prompt: "dựng cho tôi đi [Participants_Table.md và Session_Notes template]" | Dựng `Participants_Table.md` (bảng 5 người + 1 pilot, cột tên/vai trò/liên hệ đã che/ngày hẹn/trạng thái) và `session_template.md` (template ghi chú 1 phiên test: bảng quan sát theo mốc thời gian, bảng kết quả metrics, 5 probe questions, mục SUS, mục đối chiếu chéo với bug Task 1B). | Valid | Cấu trúc bảng tuân thủ yêu cầu đề bài về che thông tin liên hệ người tham gia (bảo vệ privacy của participant) và đủ trường dữ liệu tối thiểu để tái tạo được quy trình test khi TA kiểm tra chéo (traceability). Việc tách "Có phải Pilot không" giúp phân biệt rõ dữ liệu pilot (không tính vào kết quả chính thức) với 5 phiên thật, tránh làm sai lệch thống kê SUS/success rate. | Đang là file rỗng chờ điền dữ liệu thật trong quá trình test; SV sẽ điền thông tin người tham gia thật, quan sát thật, và kết quả thật vào các bảng khi chạy từng phiên — không có phần nào AI tự bịa dữ liệu test. |
| **Artifact #4** | | | | |
| **Artifact #5** | | | | |
| **Artifact #6** | | | | |
| **Artifact #7** | | | | |
| **Artifact #8** | | | | |
| **Artifact #9** | | | | |
| **Artifact #10** | | | | |

---

## 4. Tổng kết Độ chính xác AI
*Tổng hợp verdict từ Mục 3 và điền vào bảng dưới.*

| Chỉ số | Số lượng | Tỉ lệ |
| :--- | :---: | :---: |
| **Tổng artifact AI sinh đã audit** | | 100\% |
| **VALID** *(đúng, dùng nguyên)* | | % |
| **INVALID** *(sai; loại bỏ)* | | % |
| **INCOMPLETE** *(chấp nhận sau khi sửa)* | | % |

---

## 5. Kết luận — Khi nào nên / không nên dùng AI?
*Viết 80–150 chữ mô tả pattern quan sát được. AI mạnh ở đâu? AI sai ở đâu? Khuyến nghị của bạn cho việc dùng AI trong loại công việc này?*

................................................................................................................................................................................................
................................................................................................................................................................................................
................................................................................................................................................................................................

---

## 6. Mandatory Disclosure (dán nguyên văn)

> "[Test case / script / dataset / báo cáo] này được sinh phiên bản đầu bởi [tên công cụ AI]; tôi đã rà soát và chỉnh sửa [phần X], bổ sung [edge case Y, Z]; [phần W] do tôi tự viết. AI Audit Report chi tiết đính kèm ở Phụ lục A. Tôi cam đoan không dùng AI để sinh bất kỳ artifact nào thuộc danh mục bị cấm."

**Chữ ký:**

| | |
| :--- | :--- |
| **Họ tên sinh viên (in hoa):** |HỒ GIA HUY |
| **MSSV:** |23127376 |
| **Lớp / Khoá:** |23KTPM2 / 23CLC |
| **Môn học:** | CS423 / CSC13003 – Kiểm chứng Phần mềm |
| **Giảng viên:** |LÂM QUANG VŨ |
| **Ngày:** | |
| **Chữ ký:** | |

---

## Tham khảo
* Kharbach, M. (2026). AI Use Policy Templates for Higher Education. CC BY-NC-SA 4.0.
* ISTQB Foundation Level Syllabus (latest version).
* Hardman, P. (2025). A Post-AI Learning Taxonomy.
* Fuster Rabella, M. (2025). OECD Education Working Paper No. 338.
* Perkins, M., Roe, J., & Furze, L. (2025). AI Assessment Scale.
* Anthropic (2025). Building reliable AI test agents — engineering blog.
* DeepEval & Promptfoo documentation — testing frameworks for LLM systems.