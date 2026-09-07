# Open Source Classroom — LAB GUIDE

Phiên bản: 1.0
Ngày phát hành: 2026-09-07

Mục đích
----------
Open Source Classroom là kho tài liệu phục vụ cho bài lab của môn học về quy trình phát triển phần mềm và đóng góp mã nguồn mở. Tài liệu này được viết với mục tiêu hướng dẫn rõ ràng, chính xác và có thể áp dụng trong môi trường lớp học (điều kiện kiểm tra và chấm điểm).

Mục tiêu học tập (Learning Outcomes)
------------------------------------
Sau khi hoàn thành bài lab, sinh viên sẽ có thể:
1. Sử dụng Git và GitHub cho quy trình làm việc nhóm: fork, branch, commit, push, pull request (PR), review, merge.
2. Viết mô tả PR và issue rõ ràng, kèm testcase hoặc hướng dẫn tái tạo lỗi.
3. Thực hành làm việc theo chuẩn commit (ví dụ Conventional Commits) và đặt tên branch chuẩn.
4. Thực hiện review code bản chất xây dựng, phản hồi có tính xây dựng và theo dõi feedback.
5. Chuẩn bị sản phẩm (code, tài liệu, hướng dẫn) đáp ứng yêu cầu kiểm thử đơn vị hoặc mô phỏng.

Yêu cầu trước khi làm bài
-------------------------
- Có tài khoản GitHub cá nhân.
- Cài Git trên máy tính và cấu hình username/email: `git config --global user.name "Tên bạn"` và `git config --global user.email "email@domain"`.
- Kiến thức cơ bản về command line.

Thiết lập môi trường
---------------------
1. Fork repository gốc: https://github.com/dhtphu05/open-source-classroom
2. Clone fork về máy:
   git clone https://github.com/<your-username>/open-source-classroom.git
   cd open-source-classroom
3. Tạo branch cho bài làm (theo chuẩn):
   git checkout -b lab/<mssv>-<ho-ten-slug>
   Ví dụ: `git checkout -b lab/20123456-nguyen-van-a`

Cấu trúc bài lab
-----------------
Trong repository, bài lab được tổ chức như sau:
- exercises/ : thư mục chứa đề bài theo từng bài (exercise-01, exercise-02, ...). Mỗi exercise có file README.md mô tả nhiệm vụ và tiêu chí chấm.
- templates/ : mẫu Issue, PR, và mẫu báo cáo kết quả.
- resources/ : tài liệu hỗ trợ (link, slides, script cài đặt).
- tests/ (nếu có) : bộ kiểm thử tự động dùng để đánh giá.

Nội dung bài tập (ví dụ mẫu)
-----------------------------
Exercise 1 — Git fundamentals (nhóm 1-2 người)
- Yêu cầu: Thực hiện một thay đổi tài liệu/website tĩnh theo yêu cầu trong `exercises/exercise-01/README.md`.
- Kết quả cần nộp: Một Pull Request từ branch `lab/<mssv>-<ten>` trong fork của bạn vào nhánh `main` của repository gốc.
- Tiêu chí chấm: PR đúng format, commit rõ ràng, mô tả PR (mục tiêu, cách kiểm thử), passing tests (nếu có).

Deliverables — những mục phải nộp
--------------------------------
- Pull Request hợp lệ, kèm mô tả chi tiết.
- Nếu yêu cầu: file báo cáo ngắn (report.md) trong thư mục bài làm mô tả cách thực hiện và các quyết định kỹ thuật.
- Nếu có test tự động: PR phải vượt qua test CI (nếu CI được cấu hình).

Quy trình nộp bài (bắt buộc)
---------------------------
1. Fork -> tạo branch `lab/<mssv>-<ten>`.
2. Thực hiện thay đổi trên branch đó.
3. Đảm bảo commit có thông điệp rõ ràng theo chuẩn:
   - `feat(exercise-01): implement X`
   - `fix(exercise-01): correct Y`
4. Push branch lên fork và mở Pull Request vào `dhtphu05/open-source-classroom:main`.
5. Trong mô tả PR, nêu rõ:
   - Tên, mã số sinh viên (MSSV), lớp
   - Mục tiêu bài làm
   - Các bước để kiểm thử
   - Nếu cần: ảnh chụp màn hình hoặc log
6. Gắn nhãn PR theo hướng dẫn của khóa học (vd: `lab`, `exercise-01`, `ready-for-review`).

Quy tắc chấm điểm (Rubric)
---------------------------
- Tính hoàn thiện của yêu cầu (0-50%) — 50 điểm
- Chất lượng code/tài liệu (0-20%) — 20 điểm
- Tuân thủ quy trình Git/GitHub và định dạng PR (0-15%) — 15 điểm
- Kiểm thử / passing CI (0-10%) — 10 điểm
- Thái độ hợp tác (code review, phản hồi) (0-5%) — 5 điểm

Academic Integrity (Trung thực học thuật)
-----------------------------------------
- Mọi hành vi sao chép không ghi nguồn sẽ bị xử lý theo quy định của khóa học.
- Hợp tác được cho phép trong phạm vi được nêu trong đề bài; nếu hợp tác, PR phải nêu rõ tên thành viên và phần việc.

Hỗ trợ và liên hệ
------------------
- Mọi thắc mắc về đề bài hoặc lỗi kỹ thuật, mở Issue trong repository và gắn nhãn `question`.
- Liên hệ Giảng viên/Trợ giảng trong mô tả Issue: tên và email.

Checklist để đánh dấu hoàn thành trước khi mở PR
-------------------------------------------------
- [ ] Đã đọc kỹ đề bài trong `exercises/*/README.md`.
- [ ] Branch theo chuẩn `lab/<mssv>-<ten>`.
- [ ] Commit message rõ ràng và có ý nghĩa.
- [ ] Có mô tả PR đầy đủ: mục tiêu, bước kiểm thử, dữ liệu đầu vào (nếu cần).
- [ ] Đã chạy test cục bộ (nếu có) và document cách chạy test.

Tham khảo
---------
Xem `RESOURCES.md` để biết tài liệu và hướng dẫn chi tiết.

---

Nếu nội dung này ổn cho bài lab của bạn, tôi sẽ commit các file bổ sung (`CONTRIBUTORS.md`, `RESOURCES.md`) vào repository và gửi thông báo nơi các sinh viên có thể bắt đầu làm bài.