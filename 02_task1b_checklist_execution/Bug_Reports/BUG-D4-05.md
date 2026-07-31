# BUG-D4-05

| Trường | Nội dung |
|---|---|
| **Màn hình** | D4 — Chi tiết Request (Admin) |
| **Mã checklist liên quan** | IA03-02 |
| **Ngày giờ phát hiện** | 31/07/2026 |
| **Vai trò khi test** | Admin |
| **Mức độ nghiêm trọng (0–4)** | 1 |

## Bước tái hiện (Steps to Reproduce)
1. Từ danh sách Support Requests (D3), click vào 1 request để xem chi tiết (D4).
2. Quan sát phần đầu trang.

## Kỳ vọng (Expected)
Có breadcrumb thể hiện ngữ cảnh (VD: Admin > Support Requests > #24).

## Thực tế (Actual)
Không có breadcrumb nào trên trang.

## Ảnh chụp
![](../../01_report/screenshots/D4/D4_IA03-02.png)

## Ghi chú thêm
Cùng vấn đề với BUG-D1-05/BUG-D2-02/BUG-D3-06 — xác nhận đây là lỗi mang tính hệ thống, thiếu breadcrumb trên toàn bộ các trang con sâu.
