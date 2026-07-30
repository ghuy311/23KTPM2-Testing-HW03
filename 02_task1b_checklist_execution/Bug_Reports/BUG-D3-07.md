# BUG-D3-07

| Trường | Nội dung |
|---|---|
| **Màn hình** | D3 — Danh sách Support Requests (Admin) |
| **Mã checklist liên quan** | IA04-10 |
| **Ngày giờ phát hiện** | 31/07/2026 |
| **Vai trò khi test** | Admin |
| **Mức độ nghiêm trọng (0–4)** | 1 |

## Bước tái hiện (Steps to Reproduce)
1. Vào trang danh sách Support Requests (D3), áp dụng ít nhất 1 filter.
2. Di chuột (hover) vào icon xóa filter.

## Kỳ vọng (Expected)
Tooltip xuất hiện giải thích chức năng của icon (VD: "Xóa bộ lọc").

## Thực tế (Actual)
Không có tooltip nào xuất hiện khi hover vào icon xóa filter.

## Ảnh chụp
![](../../01_report/screenshots/D3/D3_IA04-10.png)

## Ghi chú thêm
Cùng vấn đề với BUG-D1-07/BUG-D2-05 — dấu hiệu thiếu tooltip là lỗi mang tính hệ thống (component dùng chung).
