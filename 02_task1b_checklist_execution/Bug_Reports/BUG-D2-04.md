# BUG-D2-04

| Trường | Nội dung |
|---|---|
| **Màn hình** | D2 — My Requests (Yêu cầu hỗ trợ) |
| **Mã checklist liên quan** | IA02-12 |
| **Ngày giờ phát hiện** | 31/07/2026 |
| **Vai trò khi test** | User |
| **Mức độ nghiêm trọng (0–4)** | 1 |

## Bước tái hiện (Steps to Reproduce)
1. Vào trang "Yêu cầu hỗ trợ" (D2), danh sách có nhiều request.
2. Dùng phím Tab để di chuyển focus lần lượt qua các item trong danh sách.
3. So sánh outline hiển thị ở request đầu tiên với các request tiếp theo.

## Kỳ vọng (Expected)
Outline focus hiển thị nhất quán (đầy đủ viền bao quanh) cho mọi item trong danh sách khi Tab tới.

## Thực tế (Actual)
Request đầu tiên chỉ có outline ở cạnh dưới (thiếu outline-top), trong khi các request sau đó có đủ cả outline-top và outline-bottom — không nhất quán.

## Ảnh chụp
![](../../01_report/screenshots/D2/D2_IA02-12(1).png)
![](../../01_report/screenshots/D2/D2_IA02-12(2).png)

## Ghi chú thêm
Có thể do phần tử đầu danh sách bị che 1 phần bởi thanh tiêu đề/toolbar phía trên, cần kiểm tra CSS overflow hoặc z-index tại vị trí item đầu tiên.
