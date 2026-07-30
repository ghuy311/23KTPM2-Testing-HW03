# BUG-D1-08

| Trường | Nội dung |
|---|---|
| **Màn hình** | D1 — Form tạo Support Request |
| **Mã checklist liên quan** | IA04-16 |
| **Ngày giờ phát hiện** | 30/7/2026 |
| **Vai trò khi test** | User |
| **Mức độ nghiêm trọng (0–4)** | 2 |

## Bước tái hiện (Steps to Reproduce)
1. Đạt tới trạng thái bị giới hạn (limit) không thể gửi thêm support request (ví dụ đã đạt số lượng request tối đa cho phép).
2. Quan sát trạng thái nút Submit trên form.

## Kỳ vọng (Expected)
Nút Submit chuyển sang trạng thái disable để phản ánh đúng việc người dùng không thể thực hiện hành động, đồng bộ với trạng thái dữ liệu thực tế.

## Thực tế (Actual)
Nút Submit vẫn ở trạng thái enable (bấm được) mặc dù đang bị giới hạn không thể gửi yêu cầu hỗ trợ — control không đồng bộ với trạng thái dữ liệu ứng dụng.

## Ảnh chụp
![](../../01_report/screenshots/D1/D1_IA04-16.png)

## Ghi chú thêm
Gây hiểu lầm cho người dùng, có thể dẫn đến thao tác vô ích hoặc lỗi khi submit bị từ chối phía backend.
