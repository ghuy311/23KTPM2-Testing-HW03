# BUG-D4-04

| Trường | Nội dung |
|---|---|
| **Màn hình** | D4 — Chi tiết Request (Admin) |
| **Mã checklist liên quan** | IA02-06 |
| **Ngày giờ phát hiện** | 31/07/2026 |
| **Vai trò khi test** | Admin |
| **Mức độ nghiêm trọng (0–4)** | 1 |

## Bước tái hiện (Steps to Reproduce)
1. Vào trang chi tiết 1 Support Request (D4).
2. Để trống ô "Nội dung phản hồi" và bấm gửi để kích hoạt lỗi validation.
3. Quan sát vị trí thông báo lỗi xuất hiện.

## Kỳ vọng (Expected)
Thông báo lỗi hiển thị ngay dưới trường bị lỗi (inline error).

## Thực tế (Actual)
Thông báo lỗi của ô "Nội dung phản hồi" không nằm ngay dưới trường đó, gây khó xác định lỗi thuộc trường nào.

## Ảnh chụp
![](../../01_report/screenshots/D4/D4_IA02-06.png)

## Ghi chú thêm
Cần chụp lại ảnh đúng và đặt tên file theo quy ước D4_IA02-06.png (ảnh hiện tại đang để tên mặc định "image.png").
