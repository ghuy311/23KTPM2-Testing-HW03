# BUG-D1-03

| Trường | Nội dung |
|---|---|
| **Màn hình** | D1 — Form tạo Support Request |
| **Mã checklist liên quan** | IA02-10 |
| **Ngày giờ phát hiện** | 30/7/2026 |
| **Vai trò khi test** | User |
| **Mức độ nghiêm trọng (0–4)** | 3 |

## Bước tái hiện (Steps to Reproduce)
1. Điền đầy đủ thông tin form tạo Support Request tại D1.
2. Nhấn nút Submit nhiều lần liên tiếp thật nhanh (double click hoặc click dồn dập).

## Kỳ vọng (Expected)
Nút Submit chuyển sang trạng thái disable/loading ngay sau lần click đầu tiên, ngăn gửi trùng request.

## Thực tế (Actual)
Nút Submit không bị disable trong lúc gửi, dẫn đến double-submit — có khả năng tạo nhiều support request trùng lặp từ 1 lần điền form.

## Ảnh chụp
![](../../01_report/screenshots/D1/D1_IA04-10.png)

## Ghi chú thêm
Ảnh hưởng tính toàn vẹn dữ liệu (data integrity) — có thể sinh dữ liệu rác trong hệ thống, cần ưu tiên fix.
