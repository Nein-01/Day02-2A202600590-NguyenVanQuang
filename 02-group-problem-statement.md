# 02 — Group Problem Statement

## Goal

This is the group deliverable. The team should work together on one final document covering:

- Team members
  - 2A202600590 - Nguyễn Văn Quang
  - 2A202600693 - Nguyễn Khánh Bằng
  - 2A202600857 - Phạm Trần Nguyên Phú
  - 2A202600975 - Mã Vĩnh Lộc

- Convergence log / meeting notes
- Validation and research
- Problem Statement
- Rule / Workflow / Agent discussion
- Final decision
- Before/after workflows

## 1. Group convergence log

- **Session 1 (May 29, 2026, 14:00-14:30):** Each member shared top 3 candidate problems. Bang presented weekly update synthesis, decision search, and rubric check. Two other members shared similar issues in status reporting and review follow-up.
- **Session 2 (May 29, 2026, 15:00-15:20):** Group clustered candidates into three themes: information synthesis, retrieval of past decisions, and submission accuracy. We scored each candidate and discussed feasibility in the 4-hour lab.
- **Session 3 (May 29, 2026, 15:50-16:10):** Final shortlist and validation plan. Group agreed đi sâu vào một problem có workflow rõ, evidence thật và phù hợp AI hỗ trợ.

### Candidates shared by each member

- Nguyễn Khánh Bằng: weekly status update, tìm decision cũ trong Discord, so khớp rubic nộp bài.
- Nguyễn Văn Quang: tổng hợp feedback review, viết meeting note, kiểm tra checklist nộp sản phẩm.
- Phạm Trần Nguyên Phú: search tài liệu cũ, xác nhận task, tổng hợp data từ CRM/Slack.
- Mã Vĩnh Lộc: kiểm tra completeness của file nộp, định nghĩa rõ requirement trước deadline.

### How the group clustered

| Cluster | Candidates | Common pattern |
|---|---|---|
| Information synthesis | Weekly update, meeting note, feedback summary | Gom nhiều nguồn rồi viết lại thành bản tóm tắt rõ ràng |
| Retrieval | Find decision in Discord, recall requirement, search old docs | Tìm lại evidence/requirement nhanh khi cần |
| Submission certainty | Rubric check, review checklist, file completeness | Giảm sai sót trước khi nộp hoặc gửi |

### Shortlist and scoring

| Candidate | Actor rõ | Workflow rõ | Evidence | Feasibility | AI fit | Total |
|---|---|---|---|---|---|---|
| Weekly update synthesis | 5 | 5 | 4 | 5 | 5 | 24 |
| Retrieval of past decision | 4 | 4 | 4 | 4 | 4 | 20 |
| Rubric / submission check | 4 | 4 | 3 | 5 | 3 | 19 |

Group chose: **Weekly update synthesis**.

## 2. Validation / research

### Validation

- Interviewed 4 peers in class and project group.
- 3/4 reported rằng họ thường mất 45-90 phút để tổng hợp nội dung từ nhiều nguồn mỗi tuần.
- Một bạn cho biết phần khó nhất là viết narrative ngắn gọn, không phải thu thập dữ liệu.
- Có một peer phản bác: team của họ dùng template cứng và đã giảm được một phần thời gian, nhưng vẫn mất effort ở bước viết cho nội dung mới.

### Research

| Source | What they solve | Insight | Gap |
|---|---|---|---|
| Notion AI / Google Docs AI | Summarize notes, rewrite text | Good for tóm tắt, nhưng cần input sạch | Không tự động gom nhiều nguồn khác nhau |
| Slack AI summary | Tóm tắt conversation | Giúp lấy ý chính từ chat | Không xử lý được số liệu từ Jira/Figma/Google Sheets |
| Weekly report template | Giảm format work | Hữu ích để chuẩn hóa | Vẫn phải tự viết phần insight và action |

### Research notes

- AI rất phù hợp khi dữ liệu đầu vào đã được cấu trúc sơ bộ.
- Xây hoàn toàn agent tự động có rủi ro hallucination nếu đầu vào quá lộn xộn.
- Workflow hợp lý là dùng rule để gom dữ liệu, sau đó AI hỗ trợ draft narrative, và con người review.

## 3. Problem Statement

**Actor:** Junior product / lab member hoặc project member cần nộp weekly status update.

**Problem v0:** Người dùng tốn nhiều thời gian gom dữ liệu và viết narrative cho weekly update.

**Problem v1:** User mất 60-90 phút mỗi tuần để chuyển nội dung từ Slack, Google Docs, Figma và Google Sheets thành báo cáo ngắn gọn, dẫn đến thiếu thông tin và giảm hiệu suất.

**Metric:** Giảm thời gian tổng hợp weekly update xuống dưới 30 phút, giữ chính xác và rõ ràng. (Fallback: hoàn thành trong 45 phút nếu không dùng AI.)

**Boundary:** Bao gồm tổng hợp dữ liệu nội bộ, đề xuất cấu trúc báo cáo, và draft narrative. Không bao gồm tự động gửi email, truy cập hệ thống bảo mật, hoặc thay thế review con người.

**Problem:** Khi phải tổng hợp tiến độ và ghi nhận kết quả từ nhiều nguồn như Slack, Google Docs, Figma và Google Sheets, người làm mất nhiều thời gian viết narrative rõ ràng.

**Context:** Cuối mỗi tuần hoặc trước buổi review nội bộ, người chịu trách nhiệm phải gửi cập nhật ngắn gọn cho nhóm và giảng viên.

**Bottleneck:** Việc biến dữ liệu thô và note rời rạc thành nội dung tóm tắt đủ rõ cho người đọc.

**Impact:** Mất 60-90 phút mỗi tuần, dẫn đến giảm thời gian thực thi công việc, dễ bỏ sót thông tin quan trọng và giảm chất lượng báo cáo.

**Success metric:** Giảm tổng thời gian soạn status update xuống dưới 30 phút mà vẫn giữ được độ chính xác và rõ ràng. Fallback: không có AI support, người làm vẫn hoàn thành trong 45 phút.

**Boundary / scope:**
- Bao gồm: tổng hợp nội dung từ nguồn text và note nội bộ, đề xuất cấu trúc status update, draft narrative.
- Không bao gồm: tự động kéo dữ liệu từ hệ thống bảo mật chưa có quyền truy cập; gửi email thay người dùng; thay thế hoàn toàn người review.

## 4. Rule / Workflow / Agent

### No AI alternative

- Dùng template weekly update và checklist.
- Mất nhiều công sức hơn ở bước viết narrative.
- Ưu điểm: ít rủi ro hơn, dễ thực hiện.

### Rule / automation alternative

- Dùng script hoặc form để gom dữ liệu từ các nguồn sẵn có.
- Giảm thời gian thu thập nhưng vẫn cần người viết phần insight.
- Ưu điểm: đáng làm nếu dữ liệu có cấu trúc.

### Workflow alternative

 - Dùng workflow chuẩn: gom dữ liệu bằng checklist / template, rồi cho AI đề xuất draft narrative và human review.
 - Giảm bottleneck ở bước viết nội dung, vẫn giữ kiểm soát của con người.
 - Ưu điểm: có thể cân bằng hiệu quả và độ tin cậy khi input đã sơ bộ.

### Agent alternative

 - AI tự động tạo toàn bộ status update từ dữ liệu thô.
 - Rủi ro: hallucination, thiếu context, và không rõ trách nhiệm nếu output sai.
 - Chỉ phù hợp khi có pipeline dữ liệu rất sạch và người dùng vẫn review kỹ.

### AI / agent alternative

- AI dùng để tóm tắt nội dung và đề xuất câu văn, không thay thế quyết định người dùng.
- Hợp lý nếu input được gom, lọc và đặt trong bối cảnh cụ thể.
- Giảm bottleneck ở bước viết narrative.

### Why final choice

Group quyết định chọn **Workflow + AI assistance**.
- Rule / template không giải quyết đủ phần viết ý chính.
- Agent toàn phần quá rủi ro khi dữ liệu chưa ổn định.
- Workflow hợp lý nhất là: gom dữ liệu → AI draft → human review.

### Comparison: No AI / Rule / Workflow / Agent

| Option | How it works | Benefits | Risks | Fit for this problem |
|---|---|---|---|---|
| No AI | Dùng template và checklist manual | Ít rủi ro, dễ triển khai | Vẫn mất nhiều thời gian viết | Khi AI không khả dụng |
| Rule | Script/form gom dữ liệu, người viết nội dung | Giảm thu thập, giữ con người chủ đạo | Không giải quyết bottleneck viết | Nếu dữ liệu có cấu trúc tốt |
| Workflow | Gom dữ liệu + AI draft + review | Giảm thời gian viết, giữ kiểm soát | Cần input đủ rõ và review | Phù hợp nhất cho weekly update |
| Agent | AI tạo toàn bộ output tự động | Nhanh nhất nếu dữ liệu sạch | Hallucination, trách nhiệm mơ hồ | Chưa phù hợp hiện tại |

### Human boundary and review

- Người dùng vẫn kiểm tra lại nội dung; AI chỉ là gợi ý draft.
- Nếu AI output sai hoặc thiếu context, người dùng bỏ draft và tự viết.
- Con người chịu trách nhiệm quyết định phần nào nên gửi.

## 5. Final decision

- **Decision:** Go with AI-assisted workflow.
- **Why:** Problem có workflow rõ, pain thật, dữ liệu có thể gom được, và phần AI hỗ trợ là writing / summarization, không phải quyết định.
- **Risks:** AI hallucination, output thiếu chính xác, dữ liệu đầu vào không đủ rõ.
- **Fallback plan:** Nếu AI không cho kết quả tốt, dùng template manual và vẫn giữ workflow gom dữ liệu thô.

### Go / Not Yet / No-Go

| Decision | Reason |
|---|---|
| Go | Workflow + AI assistance cho weekly update có thể giảm đáng kể thời gian viết narrative và vẫn giữ con người review. |
| Not Yet | Agent toàn phần chưa đủ độ tin cậy do input rời rạc và risk hallucination. |
| No-Go | Không dùng AI chỉ khi nhóm không có dữ liệu gom được hoặc không muốn thêm bước review AI. |

## 6. Workflow before / after

### Before workflow
<img width="2008" height="1421" alt="02-group-problem-statement-workflow-before" src="https://github.com/user-attachments/assets/6eb32616-0806-4cc0-a26a-b3e6ed4d6f31" />

### After workflow
<img width="1784" height="1351" alt="02-group-problem-statement-workflow-after" src="https://github.com/user-attachments/assets/9b3cdf62-52e5-4244-9e01-1792367f454e" />

### Notes

- Bottleneck hiện tại: viết narrative từ dữ liệu thô.
- AI được đặt ở bước đề xuất nội dung, không phải quyết định cuối cùng.
- Human review là checkpoint bắt buộc trước khi gửi.

## 7. Supporting files

- Nếu có thể, nhóm sẽ thêm `02-group-problem-statement-workflow.pdf` để minh họa flowchart.
- Nếu cần, ghi lại note research vào `02-group-problem-statement-research-notes.md`.

## 8. Phase 3: Finalization

### Final deliverables

- Hoàn chỉnh Problem Statement với workflow before/after và boundary rõ ràng.
- Bổ sung note research và evidence validation trong file `02-group-problem-statement-research-notes.md`.
- Chuẩn bị sơ đồ flow cho workflow AI-assisted trong `02-group-problem-statement-workflow.pdf`.
- Kiểm tra lại thành viên nhóm và file nộp, đảm bảo tất cả nội dung đều phù hợp với rubic.

### What we completed in Phase 3

- Quyết định chọn giải pháp AI-assisted workflow để giảm thời gian viết narrative cho weekly update.
- Xác định rõ actor, bottleneck, impact và success metric.
- Đặt boundary rằng AI chỉ hỗ trợ đề xuất nội dung, con người vẫn review và quyết định cuối.
- Liệt kê tập hợp supporting files cho Phase 3 và chuẩn bị nộp nhóm.
