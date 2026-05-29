
1. Tổng hợp các vấn đề
			
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
<img width="831" height="169" alt="image" src="https://github.com/user-attachments/assets/3d8005a0-5901-4bfc-aa37-2018a2b05c5f" />


4. Lựa chọn vấn đề
Nhóm chọn: Information Aggregation.

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
