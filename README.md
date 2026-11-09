# Bài 3 : Sử dụng AI an toàn khi xử lý lỗi phần mềm
## 3. Ràng buộc & Bẫy dữ liệu**

**AI có thể bị hiện tượng **AI Hallucination** (đưa ra lệnh không có thật hoặc sai phiên bản hệ điều hành).**

## 4. Yêu cầu đầu ra

**Báo cáo phân tích (IPO): Xác định **Input** (Câu trả lời của AI), **Process** (Quy trình kiểm chứng bằng toán tử **site:[stackoverflow.com](http://stackoverflow.com)** hoặc trang chủ phần mềm), **Output** (Xác nhận lệnh an toàn/không an toàn).**
|INPUT|PROCESS|OUTPUT|
|---|---|---|
|Lệnh và bối cảnh do AI cung cấp,kèm bói cảnh phiên bản và phần mểm|dùng toán tử **site:[stackoverflow.com](http://stackoverflow.com)**để tìm câu trả lời được cộng đồng xác nhận, dùng site: với trang chủ phần mềm để đối chiếu tài liệu chính thức, sau đó so sánh chéo và đánh giá rủi ro. |Kết luận lệnh an toàn, cần thận trọng hoặc không an toàn; chỉ chạy khi đã được xác nhận bởi nguồn đáng tin cậy.|

**Thiết kế một câu lệnh (Prompt) "hỏi ngược lại" AI để yêu cầu nó giải thích độ an toàn của câu lệnh trước khi bạn thực thi.**
- Lệnh này thực sự đang làm gì ?
- Nó có xóa hay ghi đè vào phần nào hay không?
- Trường hợp code này lỗi thì như thế nào/
- Kết luận mức độ an toàn ?(an toàn/cẩn thận trọng /không an toàn)?Vì sao?
- Đưa mong đợi của mình vào.
