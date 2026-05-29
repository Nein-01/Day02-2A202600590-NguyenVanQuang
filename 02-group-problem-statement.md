
1. Tổng hợp các vấn đề
#	Người đưa ra	Candidate problem	Người gặp vấn đề	Điểm nghẽn	Cảm nhận nhanh
1	2A202600590 - Nguyễn Văn Quang	Lượng kiến thức nhiều được nén lại trong thời gian ngắn gây khó tiếp cận	Học viên, giảng viên	Kiến thức dài nhưng thời gian ngắn	
2	2A202600590 - Nguyễn Văn Quang	Số TA hỗ trợ lớp quá ít so với số học viên trong 1 lớp	TA, học viên	Số lượng người ít nhưng vấn đề nhiều	
3	2A202600590 - Nguyễn Văn Quang	Một số lỗi kỹ thuật trong ứng dụng chung khiến cả TA và học viên đều khó khăn	TA, học viên	Phần mềm không hỗ trợ được workflow	
4	2A202600857 - Phạm Trần Nguyên Phú	Quên deadline giữa nhiều môn	Học viên		
5	2A202600857 - Phạm Trần Nguyên Phú	Tìm lại tài liệu/file cũ	Học viên, nghiên cứ sinh, người đi làm		
6	2A202600857 - Phạm Trần Nguyên Phú	Đọc tài liệu dài để tìm ý chính	Học viên, nghiên cứ sinh, người đi làm		
7	2A202600693 - Nguyễn Khánh Bằng	Viết status update tuần cho nhóm dự án bằng cách lấy số liệu và note từ Google Docs, Slack, Figma rồi tổng hợp vào Google Slides	Người đi làm		
8	2A202600693 - Nguyễn Khánh Bằng	Tìm lại quyết định / thông tin cũ trong Discord và Google Drive khi chuẩn bị nộp báo cáo nhóm	Người đi làm		
9	2A202600693 - Nguyễn Khánh Bằng	Chuẩn bị nộp bài lab khi không rõ các mục cần ghi, so khớp với rubic	Người đi làm, học viên		
10	2A202600975 - Mã Vĩnh Lộc	QA/QC Chất Lượng OCR Tài Liệu Cũ/Nát			
11	2A202600975 - Mã Vĩnh Lộc	Đánh Giá Hiệu Suất Và Tính Lương CTV Theo Giờ			
12	2A202600975 - Mã Vĩnh Lộc	Tự Động Phát Hiện Lỗi Chất Lượng Ảnh Scan Tại Chỗ			
<img width="1236" height="809" alt="image" src="https://github.com/user-attachments/assets/f88df827-60cd-43b2-b4f7-c340fbef2f46" />


2. Clustering các vấn đề
Nhóm nhận thấy nhiều vấn đề thực chất có pattern workflow giống nhau nên gom lại thành các cluster:

| Cluster | Candidate examples | Pattern chung |
|---|---|---|
| Information Aggregation | Weekly report, meeting recap, lab progress summary | Gom dữ liệu từ nhiều nguồn rồi viết lại |
| Knowledge Retrieval | Slack/Discord search, tìm file cũ, LMS FAQ | Tìm đúng thông tin trong nhiều nguồn rời rạc |
| Review & Validation | Review PRD, check lab submission, OCR QA/QC | Kiểm tra thiếu sót hoặc lỗi chất lượng |
| Planning & Follow-up | Deadline reminder, action item tracking | Công việc dễ bị quên sau meeting/lab |

3. Shortlist & Scoring
Candidate	Actor rõ	Workflow rõ	Pain có evidence	Impact đo được	Làm được trong lab	So sánh R/W/A được	Nhóm hiểu domain	Tổng
Weekly Report Generator	5	5	4	5	5	5	5	34
Multi-source Search	4	4	4	4	3	4	4	27
PRD / Assignment Reviewer	4	5	3	3	5	4	4	28

4. Lựa chọn vấn đề
Nhóm chọn: Project Progress summary.

Vì sao chọn:

- Workflow xảy ra thường xuyên trong môi trường học tập và làm project
- Việc tổng hợp report hiện tại đang thủ công và lặp lại
- Người dùng phải đọc lại nhiều nguồn khác nhau:
    + Google Docs
    + Slack/Discord
    + Meeting notes
    + Figma comments
- Quá trình này tốn khoảng 60–90 phút mỗi tuần
- Dễ thiếu thông tin hoặc quên update quan trọng
- Có thể đo hiệu quả rõ ràng:
    + Thời gian viết report
    + Số thông tin bị thiếu
    + Mức độ hài lòng của team

Vì sao không chọn các bài khác:

- Knowledge Retrieval: impact rộng nhưng data access phức tạp, dễ trượt sang hệ thống search/agent quá lớn.
- Review & Validation: workflow rõ nhưng quality metric khó thống nhất trong thời gian lab.
- Planning & Follow-up: Không phải AI giải quyết tốt nhất — reminder và tracking đã có công cụ chuyên biệt (Notion, Asana, Google Calendar) làm tốt hơn AI. Tần suất thấp, impact thấp — deadline reminder là việc xảy ra định kỳ, không phải pain point cốt lõi hàng ngày. Vấn đề thực chất là discipline/habit của người dùng, không phải thiếu thông tin hay thiếu xử lý.
