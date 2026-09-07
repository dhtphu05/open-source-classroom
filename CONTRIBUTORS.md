CONTRIBUTORS — HƯỚNG DẪN VÀ DANH SÁCH (CHO MỤC ĐÍCH HỌC TẬP)

Mục đích
---------
File này quy định cách ghi nhận đóng góp trong khuôn khổ bài lab: cách thêm tên sinh viên, yêu cầu tối thiểu để được ghi nhận và hướng dẫn tạo PR để bổ sung thông tin cá nhân.

Nguyên tắc ghi nhận
-------------------
- Mỗi sinh viên (hoặc nhóm) được ghi nhận khi PR của họ được merged vào repository chính theo đúng quy trình nộp bài.
- Ghi nhận bao gồm: Họ và tên, MSSV, GitHub handle và vai trò (ví dụ: author, reviewer).

Cách thêm tên (quy trình bắt buộc)
----------------------------------
1. Sau khi PR của bài lab được merged, tạo một Pull Request mới vào `main` để cập nhật `CONTRIBUTORS.md`.
2. Thêm một dòng mới vào bảng contributors theo mẫu dưới.
3. Mở PR với tiêu đề: `chore(contributors): add <MSSV> - <Ho Ten>`

Mẫu bảng contributors (Markdown)
---------------------------------
| Tên | MSSV | GitHub | Vai trò | Ghi chú |
|-----|------|--------|---------|--------|
| Nguyễn Văn A | 20123456 | @nguyenvana | Student (author) | Bài lab 01 — Exercise-01 |

Lưu ý quan trọng
----------------
- Không được thêm tên người khác mà không có sự đồng ý của họ.
- Nếu là nhóm, ghi rõ phần việc của từng thành viên.

Quy trình khi có tranh chấp
---------------------------
- Nếu có tranh chấp về quyền tác giả, liên hệ giảng viên/ban xử lý của khóa học. Mọi khiếu nại phải kèm bằng chứng (PR, commits, timestamp).

PR review và bổ sung
--------------------
- PR cập nhật CONTRIBUTORS.md sẽ được review bởi Maintainer/Trợ giảng để đảm bảo thông tin chính xác.

Ghi chú cho giảng viên
----------------------
- Maintainers có quyền chỉnh sửa danh sách để hợp thức hóa tên theo yêu cầu kiểm tra điểm.