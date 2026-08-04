---
name: ems-gui-usability-testing-agent
description: Skill tự động hóa quy trình kiểm thử GUI Checklist 45 mục đầy đủ (IA01-01 đến IA04-16), đánh giá Heuristic Usability theo Nielsen và thực thi kiểm thử Cross-Platform trên hệ thống EMS (Event Management System).
---

# Agent Skill — EMS GUI & Usability Testing Assistant

Skill này cung cấp kịch bản tự động hóa cho AI Agent để thực hiện chuỗi hoạt động kiểm thử giao diện (GUI), tính tiện dụng (Usability) và độ tương thích đa nền tảng (Cross-Platform) trên hệ thống EMS.

---

## 1. Mục tiêu & Phạm vi (Scope)

- **Ứng dụng kiểm thử (SUT):** EMS — Event Management System.
- **Phạm vi kiểm thử:** Tự động hóa kiểm thử trên các gói chức năng Admin (A, C) và User (B, D).
- **Interface Aspects (IA):** Phủ đầy đủ 45 mục kiểm thử từ IA01-01 đến IA04-16.

---

## 2. Danh sách 45 Mục GUI Checklist Chi tiết (Complete 45-Item Checklist)

### Nhóm IA-01: Chuẩn UI Chung (Typography, Layout, Color, State)
- **IA01-01:** Font chữ (Typography) rõ ràng, kích thước chữ phân cấp đúng (H1 cho tiêu đề trang, H2-H6 cho các vùng phụ). (Nielsen #8 / Shneiderman #1)
- **IA01-02:** Màu sắc nhất quán theo SUT (Primary: Xanh dương cho action chính, Danger: Đỏ cho Xóa/Block). (Nielsen #4 / Shneiderman #1)
- **IA01-03:** Độ tương phản màu sắc (Contrast Ratio) giữa chữ và nền đủ cao để dễ đọc (Universal Usability). (Shneiderman #2)
- **IA01-04:** Tính năng chuyển đổi ngôn ngữ EN/VI hoạt động mượt mà, dịch thuật đồng nhất trên toàn hệ thống. (Nielsen #2)
- **IA01-05:** Text không bị tràn, vỡ layout hoặc bị che khuất khi chuyển sang tiếng Việt. (Nielsen #8 / Shneiderman #1)
- **IA01-06:** Trạng thái rỗng (Empty State) hiển thị thông báo thân thiện và có hình minh họa. (Nielsen #1 / Norman)
- **IA01-07:** Trạng thái tải (Loading/Skeleton) hiển thị rõ ràng khi đang gọi API fetch dữ liệu. (Nielsen #1 / Norman)
- **IA01-08:** Giao diện hiển thị tốt (Responsive) trên Desktop, Tablet, Mobile; không bị cuộn ngang vô lý. (Norman / Shneiderman #2)
- **IA01-09:** Hình ảnh (Thumbnail, Banner sự kiện) hiển thị đúng tỷ lệ chuẩn (4:3, 24:9) không bị kéo giãn. (Nielsen #8)
- **IA01-10:** Icon sử dụng nhất quán, hình ảnh khớp với thế giới thực (Icon thùng rác = xóa). (Nielsen #2 / Norman)
- **IA01-11:** Không có thẻ HTML rác hoặc code bị render trực tiếp trên UI. (Nielsen #8)
- **IA01-12:** Footer và Contact hiển thị đúng cấu hình từ Admin Settings trên toàn hệ thống. (Nielsen #4)
- **IA01-13:** Lượng thông tin hiển thị trên màn hình là vừa đủ (adequate), không nhồi nhét gây rối. (Usability Slide)
- **IA01-14:** Giao diện tổ chức bám sát theo tác vụ người dùng, gom nhóm thông tin liên quan hợp lý. (Usability Slide)
- **IA01-15:** Dữ liệu khi xuất file (Export Excel/CSV) đồng nhất về ngôn ngữ, định dạng và hiển thị đầy đủ các cột. (Nielsen #4)

### Nhóm IA-02: Forms & Controls (Input, Validation, Focus, Upload)
- **IA02-01:** Mọi input field đều có Label rõ ràng, ngắn gọn và dễ hiểu. (Shneiderman #8)
- **IA02-02:** Các trường bắt buộc phải có dấu `*` màu đỏ hoặc nhãn rõ ràng để phân biệt với trường Tùy chọn (Optional). (Nielsen #4 / Shneiderman #5)
- **IA02-03:** Placeholder text cung cấp ví dụ định dạng hữu ích (VD: "Nhập email của bạn..."). (Nielsen #6 / Norman)
- **IA02-04:** Hỗ trợ thao tác nhanh: Có thể nhấn phím "Enter" để Submit form thay vì phải click chuột vào nút. (Nielsen #7 / Shneiderman #2)
- **IA02-05:** Validation lỗi định dạng ngay khi nhập (Real-time) hoặc khi blur (VD: sai định dạng email). (Nielsen #5 / Shneiderman #5)
- **IA02-06:** Thông báo lỗi (Error message) hiển thị ngay dưới trường bị lỗi (Inline error), không dùng alert chung chung. (Nielsen #9 / Shneiderman #3)
- **IA02-07:** Nội dung thông báo lỗi có tính xây dựng, chỉ rõ nguyên nhân và cách khắc phục. (Nielsen #9 / Shneiderman #3)
- **IA02-08:** Vùng Upload File/Ảnh ghi rõ ràng quy định về định dạng và dung lượng tối đa. (Nielsen #5 / Norman)
- **IA02-09:** Sau khi upload ảnh thành công, có hiển thị ảnh Preview trước khi submit form. (Nielsen #1 / Shneiderman #3)
- **IA02-10:** Nút Submit bị disable hoặc chuyển sang trạng thái loading khi form đang gửi đi để tránh double-submit. (Nielsen #5 / Norman)
- **IA02-11:** Focus order (bấm phím Tab) di chuyển hợp lý từ trên xuống dưới, trái sang phải trong form. (Shneiderman #7)
- **IA02-12:** Outline Focus: Có viền bao quanh rõ ràng khi dùng phím Tab di chuyển vào input/button (Accessibility). (Shneiderman #2)
- **IA02-13:** Form có nhiều bước (VD: Reset Password) hiển thị thanh chỉ báo tiến trình (Step Indicator). (Nielsen #1 / Shneiderman #3)
- **IA02-14:** Rich-text editor hoạt động đúng các chức năng format cơ bản (In đậm, In nghiêng, Bullet). (Nielsen #4 / Shneiderman #1)
- **IA02-15:** Các trường dữ liệu (input fields) hiển thị giá trị mặc định (field default) chính xác và hợp lý. (GUI bugs Slide)

### Nhóm IA-03: Navigation (Menu, Breadcrumb, Pagination, Deep Link)
- **IA03-01:** Thanh điều hướng (Navbar/Sidebar) highlight rõ ràng trang hoặc menu đang đứng (Active state). (Nielsen #1 / Norman)
- **IA03-02:** Có Breadcrumb rõ ràng ở các trang con sâu để người dùng dễ dàng hiểu ngữ cảnh và quay lại. (Nielsen #3 / Nielsen #6)
- **IA03-03:** Phân trang (Pagination) hoạt động đúng và tuân theo ánh xạ tự nhiên: Nút lùi bên trái, Nút tiến bên phải. (Norman / Shneiderman #7)
- **IA03-04:** Các nút "Back", "Hủy bỏ" luôn sẵn sàng để thoát khỏi luồng hiện tại một cách an toàn. (Nielsen #3 / Shneiderman #6)
- **IA03-05:** Bộ lọc (Filter) áp dụng chính xác lên danh sách và UI hiển thị rõ là filter nào đang được bật. (Nielsen #6)
- **IA03-06:** Khung tìm kiếm trả về kết quả đúng; từ khóa tìm kiếm vẫn được giữ lại trong ô input sau khi search. (Nielsen #6 / Shneiderman #8)
- **IA03-07:** Hỗ trợ Deep Linking: Khi copy URL đã filter/search mở ở tab mới, kết quả được giữ nguyên. (Shneiderman #7)
- **IA03-08:** Trạng thái không có kết quả tìm kiếm hiển thị thân thiện, có gợi ý hoặc nút "Xóa bộ lọc". (Nielsen #9 / Shneiderman #3)
- **IA03-09:** Tính năng kéo thả (Reorder) có chỉ báo thị giác (Signifiers) như icon "6 chấm" cho biết có thể kéo. (Norman)
- **IA03-10:** Khi đang kéo thả, item được chọn có phản hồi thị giác (mờ đi, hoặc có viền đổ bóng). (Nielsen #1 / Norman)
- **IA03-11:** Sau khi thả, thứ tự mới được cập nhật ngay lập tức trên UI và thông báo lưu thành công. (Nielsen #1 / Shneiderman #3)

### Nhóm IA-04: Feedback & State (Toast, Modal, Hover, Cursor)
- **IA04-01:** Hành động thành công trả về Toast Notification màu xanh lá. (Nielsen #1 / Shneiderman #3)
- **IA04-02:** Hành động thất bại trả về Toast Notification màu đỏ với nội dung lỗi cụ thể. (Nielsen #9 / Shneiderman #3)
- **IA04-03:** Toast notification tự động biến mất sau một khoảng thời gian hợp lý (3-5 giây). (Shneiderman #7)
- **IA04-04:** Hành động phá hủy (Xóa User, Block User) BẮT BUỘC có Dialog xác nhận (Confirmation). (Nielsen #5 / Shneiderman #5)
- **IA04-05:** Nút hành động chính trong Dialog nguy hiểm có màu đỏ (Cảnh báo); nút Hủy nằm ở vị trí an toàn. (Norman)
- **IA04-06:** Tương tác chuột (Hover) lên nút bấm, link, hoặc hàng trong table có hiệu ứng chuyển màu hoặc đổ bóng. (Norman)
- **IA04-07:** Tương tác nhấn (Active/Pressed) lên nút bấm có phản hồi lún xuống hoặc đổi màu nền. (Norman)
- **IA04-08:** Con trỏ chuột đổi thành hình bàn tay (Pointer) khi trỏ vào các vùng có thể tương tác (Clickable). (Norman)
- **IA04-09:** Các nút bị vô hiệu hóa (Disabled) bị làm mờ, không thể click và đổi con trỏ thành `not-allowed`. (Norman)
- **IA04-10:** Tooltip xuất hiện giải thích ý nghĩa khi hover vào các nút bấm chỉ có icon (VD: Icon con mắt). (Shneiderman #8)
- **IA04-11:** Tích hợp liên kết tới User Guide hoặc Support rõ ràng cho Admin/User khi cần hỗ trợ. (Nielsen #10)
- **IA04-12:** Nút ẩn/hiện mật khẩu (Toggle Password Visibility) hoạt động chính xác trong các form bảo mật. (Nielsen #3 / Shneiderman #7)
- **IA04-13:** Progress bar hiển thị đúng tỷ lệ % (VD: Tỷ lệ đăng ký, tiến độ duyệt) và đổi màu theo trạng thái. (Nielsen #1)
- **IA04-14:** Dữ liệu Real-time (VD: số lượng Check-in nhảy số) thay đổi trên UI mà không cần reload trang. (Nielsen #1)
- **IA04-15:** Cửa sổ pop-up/dialog phải đảm bảo tính Modality (Correct window modality) – khóa các tương tác với màn hình nền bên dưới khi đang mở. (GUI bugs Slide)
- **IA04-16:** Trạng thái của các controls và menu đồng bộ và khớp chính xác với trạng thái dữ liệu trong ứng dụng (Synchronization of window object content). (GUI bugs Slide)

---

## 3. Quy trình Thực thi của Agent (Execution Workflow)

```
[Nhận URL Màn hình EMS] 
       ↓
[Bước 1: Chạy từng mục trong 45 GUI Checklist Items (IA01-01 -> IA04-16)]
       ↓
[Bước 2: Đánh giá 10 Nielsen Heuristic Usability & Điểm đau Severity 0-4]
       ↓
[Bước 3: Thực thi Ma trận Cross-Platform (3 OS x 5 Browsers x 3 Devices)]
       ↓
[Bước 4: Xuất nhật ký Bug & Usability Findings Log chuẩn hóa]
```

---

## 4. Hướng dẫn chi tiết từng bước (Step-by-step Instructions)

### Bước 1: Kiểm thử 45 Mục GUI Checklist
1. Truy cập màn hình chỉ định trên EMS (VD: Form tạo Support Request D1).
2. Lần lượt quét và kiểm tra từng mã ID từ **IA01-01 đến IA04-16** theo danh sách ở Mục 2.
3. Đánh giá kết quả: **Passed**, **Failed**, hoặc **N/A**.
4. Với mục **Failed**: Ghi chú (Note) lại chi tiết lý do thất bại (Kỳ vọng vs Thực tế), chụp ảnh/video bằng chứng, sau đó **BẮT BUỘC TIẾP TỤC** kiểm thử các mục tiếp theo mà KHÔNG ĐƯỢC dừng quy trình.

### Bước 2: Đánh giá Tính tiện dụng (Nielsen Heuristic Evaluation)
1. Quan sát luồng thao tác người dùng trên màn hình.
2. Đánh giá theo 10 nguyên lý Heuristics (H1 đến H10).
3. Xếp hạng mức độ nghiêm trọng (Severity từ 0 đến 4).

### Bước 3: Kiểm thử Cross-Platform & Xuất Báo cáo
1. Đánh giá tính tương thích trên 3 OS x 5 Browsers x 3 Devices.
2. Tự động xuất dữ liệu vào **Bug & Usability Findings Log**.

---

## 5. Nguyên tắc Xử lý Lỗi & Tiếp tục Công việc (Fault-Tolerance & Non-Blocking Rule)

- **Nguyên tắc không chặn (Non-blocking Execution):** Trong suốt quá trình Agent kiểm thử từng mục từ IA01-01 đến IA04-16, nếu phát hiện mục bất kỳ bị Lỗi (Failed) hoặc gặp exception trên giao diện:
  - Agent thực hiện ghi vết (Logging): Đánh dấu trạng thái `Failed`, chụp ảnh minh chứng và ghi rõ nội dung lỗi vào ô Notes.
  - Agent **tuyệt đối KHÔNG ngắt luồng hoặc dừng kiểm thử**.
  - Agent lập tức chuyển sang kiểm thử mục tiếp theo trong danh sách cho đến khi phủ đủ 100% 45 mục checklist của màn hình.

