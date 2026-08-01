# Bug & Usability Findings Log

> Tổng hợp toàn bộ lỗi phát hiện trong quá trình chạy checklist GUI (Task 1B) trên 4 màn hình D1–D4, kịch bản D (Support Request). Chi tiết đầy đủ từng bug (bước tái hiện, ảnh/video minh chứng) xem tại `../02_task1b_checklist_execution/Bug_Reports/`.

## Thống kê tổng quan

| Chỉ số | Giá trị |
|---|---|
| Tổng số bug phát hiện | 23 |
| Số màn hình đã kiểm tra | 4 (D1, D2, D3, D4) |
| Severity 0 (Cosmetic) | 1 |
| Severity 1 (Minor) | 17 |
| Severity 2 (Major) | 4 |
| Severity 3 (Critical) | 1 |
| Severity 4 (Blocker) | 0 |

## Phân bố theo màn hình

| Màn hình | Số bug |
|---|---|
| D1 | 5 |
| D2 | 5 |
| D3 | 8 |
| D4 | 5 |

## Danh sách chi tiết

| Bug ID | Màn hình | Mã checklist | Severity | Mô tả |
|---|---|---|---|---|
| BUG-D1-01 | D1 | IA02-04 | 1-Minor | Nhấn Enter không có phản hồi gì, form không được submit. Người dùng buộc phải dùng chuột để click nút Submit. |
| BUG-D1-02 | D1 | IA02-10 | 3-Critical | Nút Submit không bị disable trong lúc gửi, dẫn đến double-submit — có khả năng tạo nhiều support request trùng lặp từ 1 lần điền form. |
| BUG-D1-03 | D1 | IA02-12 | 1-Minor | Không thấy outline khi Tab vào ô upload ảnh. Tuy nhiên khi nhấn Space hoặc Enter tại đó, chức năng upload vẫn được kích hoạt bình thường — chứng tỏ ô vẫn nhận focus, chỉ là không có chỉ báo thị giác. |
| BUG-D1-04 | D1 | IA03-01 | 1-Minor | Sidebar không highlight mục nào khi đang ở trang Support Request, người dùng mất dấu vị trí hiện tại trong hệ thống điều hướng. |
| BUG-D1-05 | D1 | IA04-16 | 2-Major | Nút Submit vẫn ở trạng thái enable (bấm được) mặc dù đang bị giới hạn không thể gửi yêu cầu hỗ trợ — control không đồng bộ với trạng thái dữ liệu ứng dụng. |
| BUG-D2-01 | D2 | IA03-01 | 1-Minor | Cả 3 mục trong dropdown ("Yêu cầu hỗ trợ", "Xem hồ sơ", "Đăng xuất") có cùng kiểu hiển thị, không có mục nào được đánh dấu là đang active. |
| BUG-D2-02 | D2 | IA03-02 | 1-Minor | Chỉ có nút "← Quay lại" đơn thuần, không có breadcrumb thể hiện ngữ cảnh trang hiện tại. |
| BUG-D2-03 | D2 | IA01-03 | 1-Minor | Phần "Vấn đề cần hỗ trợ" và "Mô tả chi tiết" hiển thị ngoài danh sách có độ tương phản chữ/nền không tốt, khó đọc. |
| BUG-D2-04 | D2 | IA02-12 | 1-Minor | Request đầu tiên chỉ có outline ở cạnh dưới (thiếu outline-top), trong khi các request sau đó có đủ cả outline-top và outline-bottom — không nhất quán. |
| BUG-D2-05 | D2 | IA04-10 | 1-Minor | Không có tooltip nào xuất hiện khi hover vào các nút chỉ có icon. |
| BUG-D3-01 | D3 | IA01-03 | 0-Cosmetic | Màu sắc dấu `<` `>` chuyển trang có độ tương phản thấp so với nền, khó nhìn. |
| BUG-D3-02 | D3 | IA01-08 | 2-Major | Trên mobile, giao diện không responsive — bố cục bị vỡ/tràn, ảnh hưởng khả năng sử dụng của admin trên thiết bị di động. |
| BUG-D3-03 | D3 | IA01-15 | 1-Minor | File export ra có tên cột bằng tiếng Anh mặc dù giao diện web đang để tiếng Việt. |
| BUG-D3-04 | D3 | IA02-03 | 1-Minor | Ô "Mã thành viên" không có placeholder, admin phải tự suy đoán đây là mã số sinh viên mới nhập đúng. |
| BUG-D3-05 | D3 | IA02-12 | 1-Minor | Khi Tab vào các request trong danh sách, màu outline khó nhìn / gần như không thấy. |
| BUG-D3-06 | D3 | IA03-02 | 1-Minor | Không có breadcrumb nào trên trang. |
| BUG-D3-07 | D3 | IA04-10 | 1-Minor | Không có tooltip nào xuất hiện khi hover vào icon xóa filter. |
| BUG-D3-08 | D3 | IA04-14 | 2-Major | Danh sách không tự cập nhật, admin phải F5 thủ công mới thấy request mới nhất. |
| BUG-D4-01 | D4 | IA01-08 | 2-Major | Trên mobile, giao diện không responsive. |
| BUG-D4-02 | D4 | IA02-02 | 1-Minor | Trường "Nội dung phản hồi" là bắt buộc (không submit được nếu để trống) nhưng không có dấu `*` đánh dấu. |
| BUG-D4-03 | D4 | IA02-04 | 1-Minor | Nhấn Enter không có phản hồi gì, phản hồi không được gửi. |
| BUG-D4-04 | D4 | IA02-06 | 1-Minor | Thông báo lỗi của ô "Nội dung phản hồi" không nằm ngay dưới trường đó, gây khó xác định lỗi thuộc trường nào. |
| BUG-D4-05 | D4 | IA03-02 | 1-Minor | Không có breadcrumb nào trên trang. |

## Ghi chú

- Một số bug lặp lại pattern giống nhau trên nhiều màn hình, đây là lỗi ở cấp component dùng chung, không phải lỗi riêng lẻ từng màn hình:
  - Thiếu breadcrumb (IA03-02): BUG-D2-02, BUG-D3-06, BUG-D4-05
  - Không highlight active state điều hướng (IA03-01): BUG-D1-04, BUG-D2-01
  - Thiếu tooltip cho nút icon-only (IA04-10): BUG-D2-05, BUG-D3-07
  - Outline focus không rõ/không nhất quán (IA02-12): BUG-D1-03, BUG-D2-04, BUG-D3-05
  - Không responsive trên mobile (IA01-08): BUG-D3-02, BUG-D4-01