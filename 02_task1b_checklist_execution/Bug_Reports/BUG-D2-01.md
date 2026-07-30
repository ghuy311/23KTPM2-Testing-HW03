# BUG-D2-01

| Trường | Nội dung |
|---|---|
| **Màn hình** | D2 — My Requests (Yêu cầu hỗ trợ) |
| **Mã checklist liên quan** | IA03-01 |
| **Ngày giờ phát hiện** | 31/07/2026 |
| **Vai trò khi test** | User |
| **Mức độ nghiêm trọng (0–4)** | 1 |

## Bước tái hiện (Steps to Reproduce)
1. Đăng nhập, điều hướng tới trang "Yêu cầu hỗ trợ" (D2) bằng cách click avatar góc phải → chọn "Yêu cầu hỗ trợ" trong dropdown.
2. Trong lúc đang đứng ở trang này, click lại vào avatar để mở dropdown ra lần nữa.
3. Quan sát mục "Yêu cầu hỗ trợ" trong dropdown.

## Kỳ vọng (Expected)
Mục "Yêu cầu hỗ trợ" trong dropdown được highlight (đổi màu, có nền khác, hoặc dấu hiệu active) để người dùng biết đang đứng ở trang nào.

## Thực tế (Actual)
Cả 3 mục trong dropdown ("Yêu cầu hỗ trợ", "Xem hồ sơ", "Đăng xuất") có cùng kiểu hiển thị, không có mục nào được đánh dấu là đang active.

## Ảnh chụp
![](../../01_report/screenshots/D2/D2_IA03-01.png)

## Ghi chú thêm
Cùng vấn đề với BUG-D1-05 (D1) — điều hướng tới trang "Yêu cầu hỗ trợ" nằm trong dropdown avatar, không phải sidebar/navbar chính, nên cần đối chiếu cách xử lý active state riêng cho dropdown menu này.
