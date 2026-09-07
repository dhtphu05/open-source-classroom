# Open Source Classroom

Open Source Classroom là một kho tài liệu và mẫu dự án dành cho giảng viên, trợ giảng và sinh viên muốn học và thực hành đóng góp mã nguồn mở (open-source). Mục tiêu của repo là cung cấp hướng dẫn rõ ràng, bài tập thực hành, mẫu quy trình đóng góp và tài nguyên học tập để đưa người mới tiếp cận được quy trình phát triển phần mềm thực tế.

## Mục tiêu
- Dạy các khái niệm cơ bản về Git và GitHub.
- Hướng dẫn quy trình đóng góp: fork → branch → PR → review → merge.
- Cung cấp bài tập, mẫu dự án và đề bài phù hợp cho lớp học.
- Khuyến khích sinh viên tham gia đóng góp mã nguồn mở thực tế.

## Nội dung chính
- README.md — Mô tả dự án và hướng dẫn nhanh.
- contributors.md — Hướng dẫn và danh sách đóng góp viên.
- resources.md — Tài nguyên học tập (tài liệu, video, bài viết).
- /exercises — Bài tập thực hành (mô tả bài và test/data nếu có).
- /templates — Mẫu issue, PR, và bài tập.

## Bắt đầu nhanh
1. Fork repo này về tài khoản của bạn.
2. Clone về máy:

   git clone https://github.com/<your-username>/open-source-classroom.git
3. Tạo branch mới cho thay đổi của bạn:

   git checkout -b feat/ten-cua-ban
4. Thực hiện thay đổi, commit và push:

   git add .
   git commit -m "Mô tả ngắn thay đổi"
   git push origin feat/ten-cua-ban
5. Mở Pull Request (PR) từ branch của bạn vào nhánh chính của repo gốc.

## Cách đóng góp
Trước khi đóng góp, đọc `contributors.md` để biết quy tắc đóng góp, tiêu chuẩn commit và cách thêm tên bạn vào danh sách đóng góp.

Nếu bạn là giảng viên và muốn dùng repo này cho lớp học, hãy mở một Issue với mô tả khóa học hoặc yêu cầu tính năng — chúng tôi sẽ hỗ trợ tạo template bài tập.

## Quy tắc hành xử
Mọi người tham gia phải tuân thủ Quy tắc ứng xử (Code of Conduct). Hãy lịch sự và tôn trọng khi review và trao đổi.

## Giấy phép
Mọi nội dung trong repo này được cấp phép theo MIT License — xem file LICENSE để biết chi tiết.

---

Nếu bạn muốn mình điều chỉnh nội dung README để phù hợp với chương trình giảng dạy cụ thể (ví dụ: môn Git cơ bản, PBL, hoặc workshop 2 giờ), hãy cho biết tên khóa học và mục tiêu học tập.