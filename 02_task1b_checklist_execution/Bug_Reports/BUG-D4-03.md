# BUG-D4-03

| Trường | Nội dung |
|---|---|
| **Màn hình** | D4 — Chi tiết Request (Admin) |
| **Mã checklist liên quan** | IA02-04 |
| **Ngày giờ phát hiện** | 31/07/2026 |
| **Vai trò khi test** | Admin |
| **Mức độ nghiêm trọng (0–4)** | 1 |

## Bước tái hiện (Steps to Reproduce)
1. Vào trang chi tiết 1 Support Request (D4).
2. Điền nội dung phản hồi vào ô input.
3. Nhấn phím Enter thay vì click nút Gửi.

## Kỳ vọng (Expected)
Nhấn Enter sẽ submit/gửi phản hồi, tương tự hành vi chuẩn của form input.

## Thực tế (Actual)
Nhấn Enter không có phản hồi gì, phản hồi không được gửi.

## Ảnh chụp
(chưa có ảnh — hành vi không hiển thị lỗi trên UI, cần quay video nếu muốn minh chứng)

## Ghi chú thêm
Cùng dạng lỗi với BUG-D1-01 (D1) — có thể là thiếu sót chung ở component form nhập liệu.
