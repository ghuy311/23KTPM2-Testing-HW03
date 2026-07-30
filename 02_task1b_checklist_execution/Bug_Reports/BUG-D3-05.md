# BUG-D3-05

| Trường | Nội dung |
|---|---|
| **Màn hình** | D3 — Danh sách Support Requests (Admin) |
| **Mã checklist liên quan** | IA02-12 |
| **Ngày giờ phát hiện** | 31/07/2026 |
| **Vai trò khi test** | Admin |
| **Mức độ nghiêm trọng (0–4)** | 1 |

## Bước tái hiện (Steps to Reproduce)
1. Vào trang danh sách Support Requests (D3).
2. Dùng phím Tab để di chuyển focus xuống các dòng request trong danh sách.
3. Quan sát outline focus.

## Kỳ vọng (Expected)
Outline focus hiển thị rõ ràng, dễ nhìn khi Tab vào từng request.

## Thực tế (Actual)
Khi Tab vào các request trong danh sách, màu outline khó nhìn / gần như không thấy.

## Video minh chứng
[Video đính kèm](../01_report/screenshots/D3/D3_IA02-12.mp4)
## Ghi chú thêm
Ảnh hưởng người dùng thao tác bằng bàn phím — nên đổi màu outline sang tông tương phản cao hơn với nền.
