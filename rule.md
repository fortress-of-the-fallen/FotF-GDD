# QUY ĐỊNH VIẾT BÁO CÁO ĐỒ ÁN  
(Dành cho báo cáo Game Design & Phân tích hệ thống)

---

## 1. Mục tiêu và phạm vi báo cáo

### 1.1. Mục tiêu
Báo cáo nhằm:
- Trình bày cơ sở lý thuyết và kiến thức nền tảng liên quan đến Action RPG online.
- Phân tích yêu cầu và hệ thống ở mức logic.
- Đề xuất thiết kế hệ thống và định hướng hiện thực cho giai đoạn đầu của đồ án.

### 1.2. Mức độ đồ án
- Báo cáo ở **mức độ đồ án / đồ án chuyên ngành**, không phải sản phẩm thương mại.
- Giai đoạn 1:
  - Chưa hiện thực AI phức tạp.
  - Chưa triển khai PvP hoàn chỉnh.
  - Chưa có live-ops, monetization, balancing dài hạn.
- Trọng tâm là **phân tích – thiết kế – kiến trúc**, không phải coding chi tiết.

---

## 2. Nguyên tắc viết chung

- Văn phong học thuật, trung tính.
- Không dùng ngôi thứ nhất (“tôi”, “chúng tôi”).
- Không viết theo kiểu nhật ký hay mô tả cảm tính.
- Mọi quyết định thiết kế quan trọng phải:
  - Có lập luận logic, hoặc
  - Có nguồn tham khảo.
- Không đưa nội dung ngoài phạm vi đồ án.

---

## 3. Quy định cấu trúc chương

### Chương 1 – Giới thiệu
- Bối cảnh, động lực, mục tiêu, phạm vi, ý nghĩa.
- Không dùng hình, không bảng.
- Có thể có trích dẫn tổng quan.

---

### Chương 2 – Kiến thức nền tảng và Game Design
- Trình bày **lý thuyết chung**, không gắn trực tiếp vào game của đề tài.
- Nội dung chính:
  - Action RPG
  - Multiplayer real-time
  - Core loop, meta loop
  - Progression, combat, economy, UX/UI
- Có thể dùng **1–2 hình minh hoạ khái niệm** (ví dụ: core loop).
- Bắt buộc có tài liệu tham khảo.

---

### Chương 3 – Công nghệ sử dụng
- Trình bày:
  - Game engine
  - Backend
  - Networking
  - Database
  - Công cụ quản lý (GitHub Projects, v.v.)
- Giải thích **vì sao chọn**, không viết hướng dẫn cài đặt.
- Không cần hình UI hay screenshot.

---

### Chương 4 – Các công trình liên quan
- Phân tích **nguồn cảm hứng và tài liệu tham khảo**:
  - Game
  - Phim / anime
  - Tài liệu kỹ thuật
- Không review nội dung giải trí.
- Tập trung:
  - Cơ chế
  - Cấu trúc gameplay
  - Hệ thống vận hành
- Bắt buộc có **bảng đối chiếu tổng hợp** (mapping table).

---

### Chương 5 – Phân tích yêu cầu
- Mục tiêu hệ thống.
- Đối tượng sử dụng.
- Phạm vi hiện thực giai đoạn 1.
- Yêu cầu chức năng.
- Yêu cầu phi chức năng.
- Có bảng nếu cần (use case tổng hợp, phạm vi).

---

### Chương 6 – Phân tích hệ thống
- Actors.
- Danh sách use case.
- Đặc tả use case chi tiết.
- Luồng nghiệp vụ.
- Phân tích dữ liệu logic (CRUD).
- Có thể dùng bảng thay cho UML nếu rõ ràng.

---

### Các chương sau
- Thiết kế hệ thống.
- Mô tả hiện thực.
- Đánh giá.
- Kết luận.
- Phù hợp với mức đồ án, không phô trương kỹ thuật.

---

## 4. Quy định hình ảnh (Figure)

Chỉ dùng hình khi:
- Minh hoạ khái niệm trừu tượng.
- Sơ đồ logic hoặc kiến trúc.

Không dùng:
- Screenshot game tham khảo.
- Hình mang tính mỹ thuật.

Quy định:
- Mỗi hình phải có caption.
- Mỗi hình phải được nhắc trong nội dung.
- Không lạm dụng hình.

---

## 5. Quy định bảng (Table)

Dùng bảng cho:
- Danh sách.
- So sánh.
- Phân tích logic (Actors, Use Case, CRUD).

Quy định:
- Mỗi bảng có caption và label.
- Đánh số bảng liên tục trong nội dung chính.
- Reset counter bảng trước phần nội dung chính nếu cần.

---

## 6. Quy định danh mục thuật ngữ (Glossary)

- Đặt **trước Mục lục**.
- Dùng `longtable`.
- Không dùng caption.
- Không đánh số bảng.
- Không xuất hiện trong List of Tables.

Mục đích:
- Giải thích thuật ngữ viết tắt.
- Dùng xuyên suốt báo cáo.

Glossary **không được xem là bảng nội dung chính**.

---

## 7. Quy định tài liệu tham khảo

### Trích dẫn trong nội dung
- Dùng dạng số:
  - Ví dụ: `hệ thống leo tháp [1]`
- Không dùng tên tác giả trong câu.

### Danh mục tài liệu tham khảo
- Đặt cuối báo cáo.
- Định dạng:
  - `[1] Sword Art Online – Aincrad Arc`
  - `[2] Ernest Adams, Fundamentals of Game Design`
- Thứ tự thống nhất với trích dẫn.

---

## 8. Quy định LaTeX

- Mỗi chương nằm trong một file `.tex`.
- Không reset counter tuỳ tiện.
- Front-matter và nội dung chính tách rõ.
- Không để glossary ảnh hưởng tới:
  - List of Tables
  - Đánh số bảng/hình
- Không dùng `captionof` ngoài `table` nếu không cần.

---

## 9. Tiêu chí đánh giá báo cáo

Đánh giá dựa trên:
- Tính logic và mạch lạc.
- Chất lượng phân tích – thiết kế.
- Sự nhất quán giữa các chương.
- Khả năng mở rộng cho giai đoạn sau.

Không đánh giá dựa trên:
- Độ đẹp game.
- Số lượng tính năng hiện thực.
- Độ phức tạp không cần thiết.

---

## 10. Nguyên tắc tổng quát

> Báo cáo này là **bản thiết kế và phân tích học thuật**,  
> không phải tài liệu marketing hay tài liệu kỹ thuật triển khai sản phẩm thương mại.
