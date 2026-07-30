# BUG-D3-08

| Trường | Nội dung |
|---|---|
| **Màn hình** | D3 — Danh sách Support Requests (Admin) |
| **Mã checklist liên quan** | IA04-14 |
| **Ngày giờ phát hiện** | 31/07/2026 |
| **Vai trò khi test** | Admin |
| **Mức độ nghiêm trọng (0–4)** | 2 |

## Bước tái hiện (Steps to Reproduce)
1. Mở trang danh sách Support Requests (D3) trên 2 tab/thiết bị (VD: 1 admin, 1 user gửi request mới).
2. Từ phía user, gửi 1 support request mới.
3. Quan sát danh sách bên phía admin mà không F5 trang.

## Kỳ vọng (Expected)
Danh sách tự động cập nhật request mới theo thời gian thực (real-time), không cần reload trang.

## Thực tế (Actual)
Danh sách không tự cập nhật, admin phải F5 thủ công mới thấy request mới nhất.

## Ảnh chụp
Đang bị rate limit khi test, sẽ cập nhật clip minh chứng sau.

## Ghi chú thêm
Ảnh hưởng hiệu quả xử lý support request kịp thời của admin — nên cân nhắc polling định kỳ hoặc WebSocket.
