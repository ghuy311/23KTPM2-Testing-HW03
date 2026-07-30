# BUG-D1-01

| Trường | Nội dung |
|---|---|
| **Màn hình** | D1 — Form tạo Support Request |
| **Mã checklist liên quan** | IA02-04 |
| **Ngày giờ phát hiện** | 30/7/2026|
| **Vai trò khi test** | User |
| **Mức độ nghiêm trọng (0–4)** | 1 |

## Bước tái hiện (Steps to Reproduce)
1. Mở form tạo Support Request tại D1.
2. Điền đầy đủ các trường bắt buộc bằng bàn phím.
3. Nhấn phím Enter thay vì click chuột vào nút Submit.

## Kỳ vọng (Expected)
Form được submit ngay khi nhấn Enter, tương tự như hành vi chuẩn của các form input trên web.

## Thực tế (Actual)
Nhấn Enter không có phản hồi gì, form không được submit. Người dùng buộc phải dùng chuột để click nút Submit.

## Ảnh chụp
![](../../01_report/screenshots/D1/D1_IA02-04.png)

## Ghi chú thêm
Ảnh hưởng nhẹ đến tốc độ thao tác, không chặn hoàn toàn tác vụ vì vẫn submit được bằng chuột.
