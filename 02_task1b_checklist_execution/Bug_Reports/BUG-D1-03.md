# BUG-D1-04

| Trường | Nội dung |
|---|---|
| **Màn hình** | D1 — Form tạo Support Request |
| **Mã checklist liên quan** | IA02-12 |
| **Ngày giờ phát hiện** | (điền ngày giờ test thực tế) |
| **Vai trò khi test** | User |
| **Mức độ nghiêm trọng (0–4)** | 1 |

## Bước tái hiện (Steps to Reproduce)
1. Mở form tạo Support Request tại D1.
2. Dùng phím Tab để di chuyển focus qua các trường, tới ô upload ảnh.
3. Quan sát viền (outline) báo hiệu focus.

## Kỳ vọng (Expected)
Khi Tab vào ô upload ảnh, có viền outline rõ ràng bao quanh để người dùng biết đang focus vào đâu (accessibility).

## Thực tế (Actual)
Không thấy outline khi Tab vào ô upload ảnh. Tuy nhiên khi nhấn Space hoặc Enter tại đó, chức năng upload vẫn được kích hoạt bình thường — chứng tỏ ô vẫn nhận focus, chỉ là không có chỉ báo thị giác.

## Ảnh chụp
![](../../01_report/screenshots/D1/D1_IA02-12.png)

## Ghi chú thêm
Ảnh hưởng người dùng dùng bàn phím/screen reader — khó biết đang ở đâu trong form.
