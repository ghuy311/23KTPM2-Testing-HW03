# BUG-D3-03

| Trường | Nội dung |
|---|---|
| **Màn hình** | D3 — Danh sách Support Requests (Admin) |
| **Mã checklist liên quan** | IA01-15 |
| **Ngày giờ phát hiện** | 31/07/2026 |
| **Vai trò khi test** | Admin |
| **Mức độ nghiêm trọng (0–4)** | 1 |

## Bước tái hiện (Steps to Reproduce)
1. Vào trang danh sách Support Requests (D3), đảm bảo giao diện đang để tiếng Việt.
2. Bấm chức năng Export Excel/CSV.
3. Mở file vừa export, xem tên các cột.

## Kỳ vọng (Expected)
Tên cột trong file export phải đồng nhất ngôn ngữ với giao diện hiện tại (tiếng Việt).

## Thực tế (Actual)
File export ra có tên cột bằng tiếng Anh mặc dù giao diện web đang để tiếng Việt.

## Ảnh chụp
![](../../01_report/screenshots/D3/D3_IA01-15.png)

## Ghi chú thêm
Có thể do phần export chưa được nối với hệ thống i18n dùng cho giao diện, cần đồng bộ lại.
