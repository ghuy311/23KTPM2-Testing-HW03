# BUG-D1-05

| Trường | Nội dung |
|---|---|
| **Màn hình** | D1 — Form tạo Support Request |
| **Mã checklist liên quan** | IA03-01 |
| **Ngày giờ phát hiện** | 30/7/2026 |
| **Vai trò khi test** | User |
| **Mức độ nghiêm trọng (0–4)** | 1 |

## Bước tái hiện (Steps to Reproduce)
1. Đăng nhập, điều hướng tới trang Support Request (D1) từ sidebar.
2. Quan sát mục tương ứng trên thanh sidebar.

## Kỳ vọng (Expected)
Mục 'Support Request' trên sidebar được highlight (active state) để người dùng biết đang ở trang nào.

## Thực tế (Actual)
Sidebar không highlight mục nào khi đang ở trang Support Request, người dùng mất dấu vị trí hiện tại trong hệ thống điều hướng.

## Ảnh chụp
![](../../01_report/screenshots/D1/D1_IA03_01.png)

## Ghi chú thêm
Ảnh hưởng khả năng định hướng (navigability), không chặn thao tác chính.
