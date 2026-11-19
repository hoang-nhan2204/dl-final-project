# Deep Learning Final Project

Repo làm việc chung cho bài tập cuối kỳ Deep Learning. README này là điểm bắt đầu
cho thành viên và các agent tham gia dự án.

## Trạng thái repo

Hiện repo mới có README, chưa có mã nguồn, cấu trúc thư mục, dependency hoặc lệnh
cài đặt, chạy và kiểm thử. Khi các phần này được thêm vào, hãy cập nhật README
trong cùng thay đổi để người khác có thể làm theo từ một bản clone mới.

Các file chỉ có trên máy cá nhân nhưng chưa được Git theo dõi sẽ không xuất hiện
trong bản clone của thành viên khác. Không viết hướng dẫn phụ thuộc vào những file
đó trước khi nhóm thống nhất cách chia sẻ chúng.

## Cách làm việc cho thành viên và agent

1. Đọc README và kiểm tra trạng thái Git trước khi sửa. Giữ nguyên các thay đổi
   chưa commit của người khác.
2. Chỉ sửa những file liên quan trực tiếp đến nhiệm vụ. Mỗi thay đổi nên có mục
   đích rõ ràng và đủ nhỏ để review.
3. Khi thêm một thành phần, ghi lại cách cài đặt, chạy và kiểm thử tương ứng.
   Nêu rõ dữ liệu hoặc cấu hình cần thiết, nhưng không commit thông tin bí mật.
4. Trước khi bàn giao, kiểm tra định dạng và chạy các bước kiểm thử phù hợp nếu
   dự án đã có. Báo rõ phần nào chưa kiểm chứng được.

## Quy định về code

### Clean Code & Simplicity

- Viết hàm ngắn, chỉ làm một việc. Độ sâu lồng nhau tối đa 3 cấp; nếu sâu hơn,
  hãy tách hàm hoặc dùng điều kiện thoát sớm. Đặt tên rõ nghĩa, tránh tên mẹo.
- Viết code dễ đọc: mỗi dòng code tối đa 100 ký tự. Xuống dòng cho danh sách tham
  số, biểu thức hoặc lời gọi hàm dài; không dồn nhiều lệnh vào một dòng.
- Không để code chết: xóa export không dùng, import thừa, đoạn code bị comment
  và file không còn được tham chiếu trong chính thay đổi làm chúng trở nên thừa.
- Không sao chép logic. Khi cùng một logic xuất hiện ở từ 2 nơi trở lên, tách
  thành hàm dùng chung có tên và phạm vi phù hợp.
- Không thêm dependency nếu thư viện đã có trong stack có thể giải quyết việc
  đó, chẳng hạn ORM, thư viện validation hoặc HTTP client nhóm đã chọn.
- Tránh trừu tượng hóa để dùng "sau này" (YAGNI). Chỉ tạo lớp/hàm dùng chung khi
  đã có ít nhất 2 nơi gọi thực tế.
- Giữ cách trình bày nhất quán với code hiện có. Comment nên giải thích lý do
  hoặc ràng buộc khó thấy, không lặp lại điều mà code đã nói rõ.
