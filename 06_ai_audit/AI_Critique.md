# Phản biện AI (AI Critique) — Bài tập HW03

## Đánh giá & Phản biện Quá trình Cộng tác với AI

Trong quá trình thực hiện bài tập HW03 về Kiểm thử GUI, Usability và Cross-Platform trên hệ thống EMS, các công cụ AI (Gemini 3.6 Flash và Claude Sonnet 5) đã thể hiện ưu điểm vượt trội trong việc cấu trúc bộ checklist GUI dùng chung (>40 mục), thiết kế kịch bản tác vụ hướng mục tiêu (goal-oriented task scenarios) tuân thủ tiêu chuẩn ISO 9241-11, và chuẩn hóa các biểu mẫu báo cáo.

Tuy nhiên, qua rà soát và kiểm chứng thực tế, AI bộc lộ những hạn chế cốt lõi sau:

First, AI hoàn toàn thiếu khả năng trải nghiệm thực tế trên hệ thống live. AI không thể tự nhận biết các lỗi vi phạm về tương tác trực quan động, chẳng hạn như viền Focus Outline bị mờ/chói màu khi người dùng Tab qua các ô nhập liệu, hay lỗi thiếu con trỏ nhấp nháy (`|`) khi nhấp vào Input Form D1.

Second, AI có xu hướng "bịa" hoặc tự suy đoán dữ liệu trải nghiệm người dùng (fake test data) nếu không được ràng buộc chặt chẽ. AI không thể thay thế việc quan sát cảm xúc thực tế, sự do dự hay các câu phát biểu "think-aloud" của 5 người dùng thật trong các phiên Usability Testing.

Third, đối với kiểm thử Cross-Platform, AI chỉ đưa ra các nhận định chung chung về tiêu chuẩn responsive mà không thể phát hiện các lỗi vỡ khung hình thực tế trên thiết bị di động hay lỗi cuộn trang trên trình duyệt Safari Mobile.

**Bài học rút ra:** AI là một trợ lý tuyệt vời để xây dựng khung lý thuyết, gợi ý Heuristics và chuẩn hóa tài liệu ở cấp độ G9.3/G9.4. Tuy nhiên, sinh viên phải giữ vai trò kiểm soát chất lượng (Human-in-the-loop), trực tiếp thực thi trên live app và thu thập dữ liệu kiểm thử thực tế để đảm bảo tính trung thực và chính xác của bài nộp.
