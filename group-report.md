# 02 — Group Problem Statement (Bản nộp nhóm)

> Làm chung 1 bản, mỗi thành viên copy vào repo cá nhân. Đi theo Phase 3 → 6 trong `01-worksheet.md`. Nhóm chỉ chọn **candidate problem** ở Phase 3, viết Problem Statement sau khi validate + vẽ workflow.

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm (VD: facilitator, workflow, research, writer) |
|-----|-----------|-------------|---------------------------------------------------------------|
| 1   | Lê Thanh Tùng | 2A202602499 | Facilitator — chủ trì convergence, chốt candidate |
| 2   | Đinh Quốc Bảo | 2A202602933 | Research — khảo sát tool/pattern OCR, Document AI |
| 3   | Nguyễn Hồ Nam | 2A202602788 | Workflow — vẽ current/future workflow, đo thời gian từng bước |
| 4   | Nguyễn Thu Hằng | 2A202602463 | Writer — viết Problem Statement v0/v1, tổng hợp bản nộp |
| 5   | Đậu Văn Thạch | 2A202602592 | Validation — interview/survey, thu thập evidence |

**Candidate problem nhóm chọn (1 câu):**

```text
Nhân viên nhập liệu phải đọc và gõ lại thủ công dữ liệu từ báo cáo/biểu mẫu viết tay vào Excel, khiến bước nhập liệu chiếm phần lớn thời gian xử lý và dễ phát sinh sai sót khi số lượng phiếu nhiều hoặc chữ viết khó đọc.
```

---

## Phase 3 — Group Convergence: từ 9-12 candidates về 1

### 3.1. Trình bày top 3 mỗi người (mỗi candidate 1-2 phút)

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh của nhóm |
|---|---|---|---|---|---|
| 1 | Lê Thanh Tùng | Nhập liệu thủ công từ báo cáo viết tay | Nhân viên nhập liệu | Bước đọc và gõ lại số/chữ viết tay thủ công. | Workflow rõ, lặp lại, có thể ứng dụng OCR/AI; impact dễ đo bằng thời gian |
| 2 | Lê Thanh Tùng | Xử lý báo cáo số liệu lặp lại hằng ngày | Nhân viên báo cáo | Bước copy, tổng hợp và kiểm tra các số liệu lặp lại từ nhiều báo cáo. | Lặp lại hằng ngày, workflow rõ, có khả năng tự động hóa bằng Rule/Workflow |
| 3 | Lê Thanh Tùng | Đọc thông tin từ ảnh/PDF và nhập vào Excel | Nhân viên nhập liệu | Bước đọc tài liệu và chuyển thông tin từ ảnh/PDF sang dữ liệu có cấu trúc. | Bottleneck rõ, phù hợp OCR + AI, dễ đo thời gian và độ chính xác |
| 4 | Đinh Quốc Bảo | Mất nhiều thời gian đọc và phân tích task trước khi bắt đầu code. | Intern / Developer | Thông tin của task nằm ở nhiều nguồn; phải đọc yêu cầu, tìm API/source code liên quan và trao đổi lại với Mentor/BA trước khi xác định được hướng triển khai. | Pain rõ nhưng workflow phụ thuộc từng task; cần đo thời gian và xác định bước gây chậm nhất |
| 5 | Đinh Quốc Bảo | Debug lỗi tích hợp giữa Front-end, Back-end và API mất nhiều thời gian. | Intern / FE Developer / BE Developer / Tester | Phải kiểm tra thủ công qua nhiều tầng như Front-end, request/response API, log Back-end và Database mới có thể xác định root cause. | Impact lớn, workflow rõ nhưng cần kiểm chứng thời gian debug và khả năng tự động hóa |
| 6 | Đinh Quốc Bảo | Phải đọc nhiều tài liệu API và source code trước khi phát triển hoặc chỉnh sửa chức năng. | Intern / Developer | Mất nhiều thời gian tìm đúng endpoint, file, module và theo dõi luồng Controller → Service → Repository → Database để hiểu chức năng hiện tại. | Pain khá rõ, có thể dùng AI hỗ trợ tìm kiếm/giải thích code; cần đo tần suất |
| 7 | Nguyễn Hồ Nam | Đọc slide dài 20-50 trang môn AI/ML trước deadline mất ~150 phút/buổi, bottleneck ở bước tra khái niệm và tổng hợp ý chính | Sinh viên học môn AI/ML | Tra khái niệm khó (35') + tổng hợp ý chính (30') | Số liệu cụ thể, bottleneck rõ, workflow dễ vẽ và AI có thể hỗ trợ tốt |
| 8 | Nguyễn Hồ Nam | Tra khái niệm khó trong slide phải mở 5-10 tab rời rạc, mất 30-45 phút/khái niệm | Sinh viên học môn AI/ML | Bước thu thập + tự ghép ý từ nhiều nguồn | Pain cụ thể, có số đo rõ, phù hợp AI hỗ trợ research/tổng hợp |
| 9 | Nguyễn Hồ Nam | Câu hỏi bài tập lặp lại trên Discord lớp, người trả lời mất 10-15 phút/câu | Trợ giảng, trợ giảng | Dựng lại context (mở slide tìm đúng phần) mỗi lần trả lời | Tính lặp lại cao, có thể dùng AI/knowledge base; cần kiểm chứng số câu hỏi mỗi tuần |
| 10 | Nguyễn Thu Hằng | Toàn bộ quy trình tổng hợp Daily Operation Report phải thực hiện thủ công dù cấu trúc báo cáo gần như giống nhau mỗi ngày | Nhân viên IT phụ trách tổng hợp và gửi báo cáo vận hành | Đối chiếu và tổng hợp dữ liệu từ nhiều nguồn trước khi hoàn thiện báo cáo | Workflow rõ, lặp lại hằng ngày và impact dễ đo bằng thời gian; cần kiểm chứng bottleneck thực sự nằm ở đâu |
| 11 | Nguyễn Thu Hằng | Phải đối chiếu số liệu BE với file báo cáo trước khi tổng hợp để tránh sai lệch | Nhân viên IT phụ trách kiểm tra và tổng hợp dữ liệu | So sánh và xác minh các số liệu không khớp | Problem cụ thể, workflow ngắn, có khả năng dùng Rule; cần kiểm chứng số lượng sai lệch và mức độ ảnh hưởng thực tế |
| 12 | Nguyễn Thu Hằng | Khi phát hiện camera hoặc dữ liệu bất thường, phải kiểm tra lại thông tin trước khi ghi nhận sự cố | Nhân viên IT/vận hành phụ trách theo dõi camera | Kiểm tra và xác minh các trường hợp bất thường trước khi ghi nhận | Có workflow rõ và pain trong vận hành; có thể so sánh Rule với AI nhưng cần xác định loại bất thường và tỷ lệ false alarm |
| 13 | Đậu văn Thạch | Đọc và tìm kiếm thông tin trong tài liệu API | Bản thân | Tài liệu lớn tốn thời gian tìm kiếm | Pain rõ, phù hợp AI search/RAG; cần đo số lần và thời gian tìm kiếm |
| 14 | Đậu văn Thạch | So sánh kết quả tốc độ phản hồi giữa nhiều lần/chế độ test | Bản thân | Nhiều số liệu cần tổng hợp và so sánh | Có tính lặp lại và dễ tự động hóa; cần xác định số lần test và thời gian xử lý |
| 15 | Đậu Văn Thạch | Đối chiếu kết quả test chatbot với yêu cầu/kỳ vọng của mentor | Mentor, bản thân | Phải xem lại kết quả test và tài liệu liên quan | Pain thực tế, có thể hỗ trợ bằng AI nhưng cần xác định tiêu chí đánh giá và thời gian đối chiếu |

### 3.2. Gom trùng / cluster

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| A | #1, #3, #7, #8 | Đọc, tìm kiếm và trích xuất thông tin từ tài liệu | Đều mất thời gian khi phải đọc tài liệu dài, tìm thông tin, tra khái niệm hoặc chuyển thông tin từ tài liệu sang dữ liệu có cấu trúc; có tiềm năng dùng OCR, AI Search hoặc RAG |
| B | #2, #10, #11, #14 | Tổng hợp, đối chiếu và xử lý dữ liệu lặp lại | Có workflow lặp lại, nhiều số liệu hoặc nhiều nguồn dữ liệu; phù hợp với Rule, Excel automation hoặc Workflow automation |
| C | #4, #5, #6, #15 | Hiểu task, code và kiểm tra/debug hệ thống | Đều liên quan đến việc đọc context, source code, API, log hoặc kết quả test để xác định vấn đề; AI có thể hỗ trợ phân tích và tìm nguyên nhân |
| D | #9, #12 | Xử lý câu hỏi hoặc tình huống bất thường cần xác minh | Đều phát sinh khi cần tìm context, kiểm tra thông tin và đưa ra phản hồi/xác nhận; có thể dùng AI hỗ trợ nhưng cần kiểm chứng độ chính xác và false alarm |

### 3.3. Shortlist

| Candidate | Vì sao vào shortlist (2-3 ý) | Rủi ro / điều chưa rõ |
|---|---|---|
| #1 – Nhập liệu thủ công từ báo cáo viết tay | - Công việc lặp lại, quy trình rõ ràng và dễ mô tả.<br>- Có thể đo trực tiếp thời gian nhập liệu và tỷ lệ sai sót.<br>- AI/OCR có khả năng hỗ trợ rõ ràng, có thể kiểm chứng bằng prototype. | - Chưa rõ tần suất thực tế và số lượng báo cáo mỗi ngày.<br>- Độ chính xác phụ thuộc nhiều vào chất lượng chữ viết tay. |
| #4 – Mất nhiều thời gian đọc và phân tích task trước khi bắt đầu code | - Pain point thực tế đối với Intern/Developer.<br>- Quy trình gồm nhiều bước: đọc yêu cầu, tìm tài liệu/API/source, xác định hướng xử lý.<br>- Có tiềm năng ứng dụng AI để tóm tắt task, tìm source/API và gợi ý hướng triển khai. | - Thời gian xử lý phụ thuộc độ khó từng task.<br>- Cần xác định rõ phần nào thực sự gây mất thời gian nhất.<br>- Khó đo hiệu quả nếu task giữa các lần không tương đồng. |
| #10 – Toàn bộ quy trình tổng hợp Daily Operation Report thủ công dù cấu trúc gần như giống nhau mỗi ngày | - Xảy ra hằng ngày, tính lặp lại rất cao.<br>- Quy trình và đầu ra tương đối cố định nên dễ chuẩn hóa/đo lường.<br>- Có tiềm năng tự động hóa bằng Rule + Workflow, kết hợp AI khi cần xử lý dữ liệu không đồng nhất. | - Cần xác định chính xác các nguồn dữ liệu đầu vào.<br>- Chưa rõ bước nào chiếm nhiều thời gian nhất.<br>- Cần kiểm tra mức độ sai lệch và các trường hợp ngoại lệ trong báo cáo. |

### 3.4. Score để đồng thuận

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #1 – Nhập liệu thủ công từ báo cáo viết tay | 5 | 5 | 4 | 5 | 5 | 5 | 5 | 34 |
| #10 – Tổng hợp Daily Operation Report thủ công | 4 | 5 | 5 | 5 | 5 | 5 | 4 | 33 |
| #4 – Đọc và phân tích task trước khi code | 5 | 4 | 4 | 4 | 5 | 4 | 4 | 30 |

**Candidate nhóm chọn (1 bài duy nhất):**

```text
#1 – Nhập liệu thủ công từ báo cáo viết tay
```

**Vì sao chọn (4-5 câu):**

```text
Nhóm chọn Candidate #1 vì vấn đề có actor rõ ràng, workflow cụ thể và xảy ra trong một quy trình lặp lại. Điểm nghẽn tập trung ở việc đọc và nhập lại dữ liệu viết tay, nên có thể xác định rõ thời gian xử lý và tỷ lệ sai sót. Đây cũng là bài toán phù hợp để thử nghiệm OCR/AI và có thể xây dựng prototype trong phạm vi lab. Nhóm có thể dễ dàng so sánh Current Workflow với AI-assisted Workflow và đo được mức giảm thời gian, độ chính xác trước và sau khi áp dụng. Ngoài ra, fallback vẫn rõ ràng: các trường có độ tin cậy thấp sẽ được chuyển sang người kiểm tra thủ công.
```

**Vì sao KHÔNG chọn các candidate còn lại (mỗi bài 2-3 câu):**

```text
#10 – Tổng hợp Daily Operation Report thủ công:
Vấn đề có tính lặp lại và khả năng tự động hóa cao, nhưng quy trình phụ thuộc vào nhiều nguồn dữ liệu và cần hiểu rõ hơn về các trường hợp ngoại lệ. So với #1, việc dựng prototype và kiểm chứng trong lab khó kiểm soát hơn.

#4 – Mất nhiều thời gian đọc và phân tích task trước khi bắt đầu code:
Đây là pain point thực tế nhưng độ khó của từng task khác nhau nên khó xây dựng baseline và đo hiệu quả một cách nhất quán. Ngoài ra, cần xác định rõ bước nào trong quá trình đọc task thực sự gây mất nhiều thời gian nhất.
```

**Disagreement (nếu có — ai lo gì, chốt ra sao):**

```text
Một số thành viên có thể ưu tiên #10 vì đây là quy trình xảy ra hằng ngày và có tiềm năng tự động hóa lớn. Tuy nhiên, nhóm thống nhất chọn #1 vì workflow đơn giản, bottleneck rõ, dễ đo lường và dễ xây dựng prototype để kiểm chứng trong lab. #10 được giữ lại như phương án dự phòng nếu trong quá trình kiểm chứng #1 gặp vấn đề về chất lượng dữ liệu viết tay.
```

---

## Phase 4 — Quick Validation + Research

### 4.1. Quick validation (ít nhất 1 cách: interview 2-3 người hoặc survey 5-10 người)

| Nguồn | Số người / mẫu | Tín hiệu xác nhận (kèm quote nguyên văn) | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Interview | 3 | Người được hỏi đều xác nhận việc đọc và nhập dữ liệu viết tay tốn thời gian, đặc biệt khi số lượng biểu mẫu nhiều. Quote cần lấy nguyên văn từ người được phỏng vấn, ví dụ: "[Điền quote thực tế]" | Một người cho rằng nếu biểu mẫu ít hoặc chữ viết rõ thì thời gian xử lý không đáng kể. | Thu hẹp problem vào trường hợp có số lượng báo cáo nhiều hoặc chữ viết tay khó đọc, thay vì coi mọi báo cáo viết tay đều là pain point. |
| Survey / poll | 8 | Phần lớn người trả lời cho biết họ từng phải nhập lại dữ liệu từ báo cáo viết tay và cho rằng đây là công việc mất thời gian. | Một số người ít gặp báo cáo viết tay hoặc đã sử dụng biểu mẫu điện tử nên pain point thấp. | Tập trung vào nhóm thường xuyên tiếp nhận và số hóa báo cáo viết tay. |
| Log / ticket / review (nếu có) | Chưa có | Chưa có dữ liệu log/ticket thực tế để xác nhận. | Chưa có bằng chứng định lượng từ log. | Không sử dụng nguồn này để kết luận; ưu tiên interview/survey và đo thời gian thực tế trong prototype. |

> ⚠️ Còn thiếu: quote nguyên văn của 3 người interview. Nhóm phải điền trước khi nộp, không được để placeholder.

**Insight sau validation (1-2 câu — pain thật nằm ở đâu):**

```text
Pain không nằm đơn thuần ở việc có báo cáo viết tay, mà nằm ở bước đọc và nhập lại dữ liệu thủ công khi số lượng báo cáo nhiều hoặc chữ viết khó đọc. Vì vậy, problem được thu hẹp thành việc giảm thời gian và sai sót khi chuyển dữ liệu viết tay từ báo cáo sang dữ liệu có cấu trúc.
```

Bằng chứng đính kèm (nếu có): `02-group-problem-statement-survey.png`, `...-interview-notes.md`

### 4.2. Research giải pháp đã có (ít nhất 2-3 tools/patterns + 1-2 link kiểm được)

| Nguồn / tool / case | Link | Họ giải quyết bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Google Cloud Document AI – Enterprise Document OCR | https://docs.cloud.google.com/document-ai/docs/enterprise-document-ocr | Nhận diện chữ viết tay từ ảnh/PDF, phát hiện dòng/từ và cấu trúc tài liệu; có thể dùng kết quả OCR làm đầu vào cho bước trích xuất dữ liệu có cấu trúc. | Hỗ trợ OCR tài liệu, handwriting, layout và quality assessment; có thể xử lý tài liệu nhiều ngôn ngữ. | Chất lượng nhận diện phụ thuộc chất lượng ảnh và kiểu chữ; handwriting tiếng Việt hiện được Google ghi nhận ở mức experimental. | Không nên tự xây OCR từ đầu; nên tận dụng OCR có sẵn rồi tập trung vào xử lý hậu OCR, chuẩn hóa dữ liệu và human review. |
| Azure AI Document Intelligence – Read / Layout | https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/overview | Đọc chữ in và chữ viết tay, xác định dòng/từ, confidence; có thể kết hợp Layout để lấy bảng, cấu trúc và key-value. | Có confidence cho từng từ, hỗ trợ handwriting và trích xuất cấu trúc tài liệu; phù hợp xây pipeline document processing. | Khả năng hỗ trợ ngôn ngữ và handwriting thay đổi theo model; vẫn cần kiểm tra accuracy trên chính bộ dữ liệu của nhóm. | Nên sử dụng confidence score để quyết định trường nào AI tự động chấp nhận và trường nào chuyển cho người kiểm tra. |
| Amazon Textract | https://aws.amazon.com/textract/ | Nhận diện chữ in/chữ viết tay, trích xuất text, forms, tables và dữ liệu có cấu trúc từ ảnh/PDF. | Có sẵn OCR + document analysis, hỗ trợ handwriting và trả về confidence score; phù hợp với quy trình tự động hóa nhập liệu. | Một số chức năng handwriting và xử lý tài liệu có giới hạn ngôn ngữ; cần kiểm tra khả năng đáp ứng dữ liệu tiếng Việt thực tế. | Có thể dùng confidence threshold để xây cơ chế fallback: confidence thấp → người kiểm tra → sửa dữ liệu trước khi xuất Excel. |

**Research takeaway (2-3 câu — nên build gì / không build gì):**

```text
Nhóm không nên build một OCR chữ viết tay tiếng Việt hoàn toàn từ đầu, mà nên xây một pipeline OCR chuyên biệt cho từng loại biểu mẫu/doanh nghiệp: thu thập dữ liệu chữ viết tay thực tế → fine-tune model OCR tiếng Việt → nhận diện từng trường → chuẩn hóa dữ liệu → kiểm tra confidence → human review → xuất Excel/API. Với chữ viết tay tiếng Việt, nhóm có thể bắt đầu từ PaddleOCR/SVTR hoặc các model/dataset tiếng Việt hiện có, sau đó fine-tune bằng dữ liệu thực tế của từng doanh nghiệp thay vì dùng một model chung cho mọi loại tài liệu.

Định hướng build nên chia theo từng use case doanh nghiệp: (1) doanh nghiệp sản xuất/kho vận: phiếu nhập kho, phiếu xuất kho, biên bản kiểm kê; (2) bán lẻ/F&B: phiếu nhập hàng, phiếu kiểm kê, phiếu giao nhận; (3) kế toán: phiếu thu, phiếu chi, chứng từ nội bộ; (4) logistics: phiếu giao hàng, biên bản bàn giao; (5) ngân hàng/bảo hiểm: biểu mẫu nghiệp vụ có trường viết tay. Với mỗi case, nhóm chỉ train và tối ưu những trường thực sự có giá trị như mã hàng, số lượng, ngày, số tiền, tên khách hàng hoặc ghi chú, thay vì cố nhận diện toàn bộ trang tài liệu.

Không nên cạnh tranh với các nền tảng OCR doanh nghiệp ở việc "đọc mọi loại tài liệu". Giá trị của nhóm nên nằm ở khả năng fine-tune theo handwriting/domain cụ thể, mapping chữ viết tay thành schema dữ liệu của từng doanh nghiệp và cơ chế confidence-based human-in-the-loop để các trường khó đọc được chuyển sang nhân viên xác nhận.
```

> Lưu ý: không dùng số liệu AI đưa nếu không verify được link chính thức. Ghi rõ giả định chưa chắc.

---

## Phase 5 — Workflow + Problem Statement

**Phạm vi cụ thể hóa để vẽ workflow:** 1 loại biểu mẫu duy nhất — *Phiếu nhập kho viết tay* của bộ phận kho, xử lý theo lô cuối ngày (~20 phiếu/ngày, 8 trường/phiếu: ngày, số phiếu, mã hàng, tên hàng, đơn vị tính, số lượng, đơn giá, người giao).

### 5.1. Current workflow bản nhóm

Dán workflow hoặc link file: `02-group-problem-statement-workflow.png`

```text
[1 Nhận & gom phiếu viết tay: 5' - NV kho] → [2 Phân loại, đánh số lô: 5' - NV nhập liệu]
→ [3 Chụp/scan phiếu: 10' - NV nhập liệu] → [4 Đọc từng phiếu & gõ tay vào Excel: 70' ⛔ BOTTLENECK - NV nhập liệu]
→ [5 Hỏi lại người viết khi chữ khó đọc/thiếu trường: 15' - NV nhập liệu ↔ NV kho (handoff)]
→ [6 Soát lại số liệu (đối chiếu phiếu ↔ Excel): 15' - NV nhập liệu]
→ [7 Lưu file & gửi báo cáo/đẩy vào hệ thống: 5' - NV nhập liệu]

Tổng: ~125 phút / lô 20 phiếu / ngày  (số đo pilot nội bộ — CẦN đo lại trên 1 tuần thực tế)
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú (handoff? bottleneck?) |
|---|---|---|---|---|---|
| 1 | NV kho | Phiếu viết tay rời | Tập phiếu theo ngày | 5' / ngày | Handoff kho → nhập liệu; phiếu có thể thiếu/nhàu |
| 2 | NV nhập liệu | Tập phiếu | Lô phiếu đã đánh số | 5' / ngày | Thủ công nhưng nhanh, không phải bottleneck |
| 3 | NV nhập liệu | Phiếu giấy | Ảnh/PDF phiếu | 10' / ngày | Chất lượng ảnh không đồng đều → ảnh hưởng bước sau |
| 4 | NV nhập liệu | Phiếu giấy / ảnh | 20 dòng Excel (160 trường) | ~3,5'/phiếu → **70' / ngày** | ⛔ **Bottleneck chính**: đọc chữ tay + gõ lại; mỏi mắt, dễ nhầm số |
| 5 | NV nhập liệu ↔ NV kho | Trường không đọc được | Trường đã xác nhận | 15' / ngày (≈3-5 phiếu) | **Handoff**: phải chờ người viết rảnh, có khi sang hôm sau |
| 6 | NV nhập liệu | Excel + phiếu gốc | Excel đã soát | 15' / ngày | Soát 100% thủ công, vẫn sót lỗi |
| 7 | NV nhập liệu | Excel đã soát | File/bản ghi trong hệ thống | 5' / ngày | Cuối luồng, ít rủi ro |

**Bottleneck chính (2-3 câu):**

```text
Bottleneck nằm ở bước 4 — đọc từng trường viết tay và gõ lại vào Excel — chiếm khoảng 70/125 phút (~56%) toàn bộ thời gian của lô. Đây là bước duy nhất mà thời gian tăng tuyến tính theo số phiếu và là nơi phát sinh hầu hết lỗi số liệu (nhầm chữ số, nhầm mã hàng), kéo theo chi phí ở bước 6 (soát lại) và bước 5 (hỏi lại người viết). Bước 5 tuy ngắn hơn nhưng là handoff gây chờ đợi, nên nhóm coi bước 4 là điểm can thiệp chính và bước 5 là điểm can thiệp phụ.
```

### 5.2. Future workflow bản nhóm

Phải nhìn ra 5 thứ: bước nào máy (Rule), bước nào AI, bước nào người, boundary ở đâu, fallback khi AI sai.

```text
[1 Chụp/scan hàng loạt theo lô: 10' - NGƯỜI]
→ [2 RULE: kiểm tra chất lượng ảnh (độ phân giải/mờ/nghiêng), auto-rotate, đặt tên & phân loại theo mã biểu mẫu: 2' - MÁY]
→ [3 AI: OCR chữ viết tay + trích xuất 8 trường theo schema, trả confidence từng trường: 3' - AI]
→ [4 RULE: validate dữ liệu (định dạng ngày, mã hàng phải có trong danh mục, số lượng > 0, thành tiền = SL × đơn giá), gắn cờ trường nghi ngờ: 1' - MÁY]
→ [5 NGƯỜI review các trường confidence < 0,90 hoặc bị Rule gắn cờ, sửa trực tiếp trên màn hình ảnh–dữ liệu song song: 20' ⬅ BOUNDARY]
→ [6 Xuất Excel / đẩy API + lưu ảnh gốc kèm bản ghi: 2' - MÁY]

Tổng kỳ vọng: ~38 phút / lô 20 phiếu (giả định, cần đo lại bằng pilot)

BOUNDARY:
- AI chỉ được làm: đọc chữ và đề xuất giá trị cho từng trường.
- AI KHÔNG được làm: tự chốt dữ liệu cuối, tự ghi vào hệ thống kho, tự suy đoán trường bị bỏ trống trên phiếu.
- Mọi bản ghi chỉ được xuất sau khi có người bấm xác nhận.

FALLBACK khi AI sai:
- Trường có confidence < 0,90 hoặc vi phạm Rule → đưa vào hàng đợi review, hiển thị cạnh ảnh gốc để người sửa nhanh.
- Ảnh mờ/nghiêng/thiếu góc → Rule chặn ngay ở bước 2, yêu cầu chụp lại, không đưa vào OCR.
- Trường trên phiếu thực sự không đọc được → giữ nguyên quy trình cũ: hỏi lại NV kho (giữ bước handoff cũ làm đường lui).
- Nếu OCR lỗi/hết quota/hệ thống down → chuyển toàn lô về nhập tay bằng template Excel cũ, không chặn nghiệp vụ.
```

**Before/after impact:**

| Metric | Trước | Sau kỳ vọng | Cách đo |
|---|---:|---:|---|
| Tổng thời gian / lô 20 phiếu | ~125' | ~38' (−70%) | Bấm giờ 5 ngày liên tiếp trước và sau, cùng 1 nhân viên, cùng loại phiếu |
| Số bước | 7 | 6 | Đếm trên sơ đồ workflow |
| Số bước thủ công | 6/7 | 2/6 (bước 1 và bước 5) | Đếm bước có người thao tác trực tiếp |
| Bottleneck chính | Bước 4 — gõ tay 160 trường (70') | Bước 5 — review trường nghi ngờ (20') | Bấm giờ riêng từng bước |
| Độ chính xác trường | Chưa đo (giả định ~97% sau soát tay) | ≥ 98% sau review | Đối chiếu 200 trường mẫu với phiếu gốc do người thứ hai chấm |
| Risk mới | — | AI đọc sai nhưng confidence cao → lỗi lọt qua review ("silent error") | Audit ngẫu nhiên 10% bản ghi đã auto-accept mỗi tuần |

### 5.3. Problem Statement v0 (mỗi field 2-3 câu)

| Field | Nội dung |
|---|---|
| **Actor** | Nhân viên nhập liệu của bộ phận kho, người nhận phiếu nhập kho viết tay từ NV kho và chịu trách nhiệm số hóa vào Excel/hệ thống. Mỗi ngày xử lý khoảng 20 phiếu, mỗi phiếu 8 trường. |
| **Workflow** | Nhận phiếu → phân loại → chụp/scan → đọc và gõ tay vào Excel → hỏi lại người viết khi chữ khó đọc → soát lại → lưu/gửi. Toàn bộ 7 bước hiện làm thủ công, chỉ có bước lưu file là thao tác máy. |
| **Bottleneck** | Bước 4: đọc từng trường viết tay và gõ lại, chiếm ~70/125 phút (~56%) mỗi lô. Thời gian tăng tuyến tính theo số phiếu và đây là nơi phát sinh phần lớn lỗi số liệu. |
| **Impact** | Mất ~125 phút/ngày cho một việc không tạo giá trị mới, tương đương hơn 10 giờ/tháng của một nhân viên. Lỗi nhập sai mã hàng hoặc số lượng phải truy ngược lại phiếu gốc và làm lệch tồn kho. |
| **Success Metric** | Giảm tổng thời gian xử lý lô 20 phiếu từ ~125' xuống ≤ 50', và giữ độ chính xác ở mức trường ≥ 98% sau bước review. Đo bằng bấm giờ 5 ngày trước/sau và chấm chéo 200 trường mẫu. |
| **Boundary** | Chỉ xử lý 1 loại biểu mẫu (phiếu nhập kho) và 8 trường đã định nghĩa; không xử lý phiếu khác loại, không đọc phần ghi chú tự do. AI chỉ đề xuất giá trị, người vẫn là bên xác nhận cuối trước khi dữ liệu vào hệ thống. |

**Câu hỏi AI phản biện v0 (nếu có):**
- Field nào mơ hồ: "Impact" ban đầu chỉ nói "mất nhiều thời gian" mà không quy ra con số/tháng; "Success Metric" ban đầu chỉ nói "nhanh hơn" mà không có mốc và cách đo; "Boundary" chưa nói rõ loại biểu mẫu nào.
- Tôi sửa gì: quy Impact ra phút/ngày và giờ/tháng kèm hệ quả nghiệp vụ (lệch tồn kho); đặt mốc cụ thể cho Success Metric (≤ 50', accuracy ≥ 98%) và ghi rõ cách đo; khóa Boundary về đúng 1 biểu mẫu và 8 trường, loại phần ghi chú tự do ra khỏi phạm vi.

---

## Phase 6 — Rule / Workflow / Agent + Decision

### 6.0. Ma trận độ phù hợp (suy nghĩ nhanh, không thay quyết định cuối)

- Độ mơ hồ: [x] Thấp (có đúng/sai rõ) / [ ] Cao (nhiều cách trả lời vẫn OK) — Vì sao: mỗi trường trên phiếu chỉ có đúng một giá trị đúng, đối chiếu được với phiếu gốc; không có chuyện "nhiều đáp án cùng chấp nhận được".
- Độ phức tạp: [ ] Thấp (1-2 bước) / [x] Cao (3+ bước/nguồn, phụ thuộc nhau) — Vì sao: phải qua kiểm tra ảnh → OCR → trích xuất theo schema → validate theo danh mục hàng hóa → review → xuất dữ liệu, các bước phụ thuộc kết quả của nhau.

**Bài toán nhóm nằm ở ô nào:**

```text
Ô "Độ mơ hồ THẤP + Độ phức tạp CAO" → Workflow (pipeline nhiều bước cố định, có AI ở đúng một mắt xích).
```

**Vì sao (2-3 câu):**

```text
Đầu ra có đúng/sai rõ ràng nên không cần một hệ thống tự quyết định linh hoạt, nhưng chuỗi xử lý lại gồm nhiều bước phụ thuộc nhau nên một Rule đơn lẻ không gánh nổi. Mắt xích duy nhất thực sự cần AI là đọc chữ viết tay; các bước còn lại đều có thể mô tả bằng logic cố định. Vì vậy bài toán rơi đúng vào dạng Workflow: đường đi cố định, AI đóng vai một node trong chuỗi.
```

### 6.1. So sánh Rule / Workflow / Agent (so trên cùng 1 bài)

| Mức | Phương án cho bài toán nhóm | Khi nào đủ | Rủi ro | Chọn? (Dùng cho bước nào?) |
|---|---|---|---|---|
| **Rule** | Template Excel có data validation, dropdown mã hàng, công thức tự tính thành tiền, cảnh báo khi ngày/số lượng sai định dạng. Người vẫn gõ tay. | Đủ nếu phiếu đã là dữ liệu điện tử, hoặc nếu mục tiêu chỉ là giảm lỗi chứ không giảm thời gian gõ. | Không chạm vào bottleneck (bước 4 vẫn 70'); chỉ giảm lỗi định dạng, không giảm công đọc–gõ. | ✅ Có — dùng cho **bước 2** (kiểm tra chất lượng ảnh) và **bước 4** (validate sau OCR). Không dùng làm giải pháp chính. |
| **Workflow** | Pipeline cố định: kiểm tra ảnh (Rule) → OCR + trích xuất trường (AI) → validate + gắn cờ (Rule) → người review trường nghi ngờ → xuất Excel/API. | Đủ khi loại biểu mẫu cố định, schema trường biết trước, thứ tự bước không đổi giữa các lô. | Phụ thuộc chất lượng OCR tiếng Việt viết tay; phải tự chỉnh ngưỡng confidence; mỗi biểu mẫu mới phải cấu hình lại schema. | ✅ **CHỌN LÀM MỨC CHÍNH** — dùng cho toàn bộ luồng bước 2 → 6. |
| **Agent** | Agent tự quyết định gọi tool nào (OCR, tra danh mục hàng, hỏi lại người viết, tra hệ thống kho), tự lập kế hoạch xử lý cho từng phiếu lạ. | Chỉ đủ lý do khi đầu vào là nhiều loại chứng từ không biết trước, cần tự tra cứu chéo nhiều hệ thống. | Không xác định, khó debug khi sai, chi phí cao, khó đo baseline; rủi ro tự ghi dữ liệu sai vào hệ thống kho. | ❌ Không chọn — không có bước nào trong bài này cần tự lập kế hoạch. |

**5 câu hỏi chốt (trả lời câu đầy đủ):**

1. **Rule có giải được 70-80% case không?** Không. Rule chỉ xử lý được phần kiểm tra định dạng và tính toán sau khi dữ liệu đã ở dạng số, trong khi 70% thời gian của bài toán nằm ở việc chuyển ảnh chữ viết tay thành văn bản — việc mà không có logic if/else nào làm được.
2. **Các bước có đi thẳng một đường không hay phải rẽ nhánh?** Các bước đi thẳng một đường cố định (ảnh → OCR → validate → review → xuất), chỉ có đúng một nhánh điều kiện đơn giản là "confidence thấp hoặc vi phạm Rule thì đưa vào hàng đợi review", nên hoàn toàn mô tả được bằng một workflow tĩnh.
3. **Có thật sự cần Agent tự lập kế hoạch + gọi tool không?** Không cần, vì với mỗi phiếu, danh sách tool và thứ tự gọi luôn giống hệt nhau và đã biết trước; không có tình huống nào buộc hệ thống phải tự nghĩ ra bước tiếp theo.
4. **Nếu AI sai, ai phát hiện đầu tiên và sửa trong bao lâu?** Nhân viên nhập liệu phát hiện ngay tại bước 5 vì màn hình review hiển thị ảnh gốc cạnh giá trị AI đề xuất, sửa một trường mất khoảng 5-10 giây; nếu lỗi lọt qua (confidence cao nhưng sai), kế toán kho sẽ phát hiện khi đối chiếu tồn kho cuối tuần và nhóm có audit ngẫu nhiên 10% bản ghi để bắt sớm.
5. **Có hạ được từ Agent → Workflow → Rule không?** Hạ được từ Agent xuống Workflow và nhóm đã hạ, nhưng không hạ tiếp xuống Rule được vì Rule không đọc được chữ viết tay — đó là ranh giới cứng của bài toán này.

**Mức chọn:**

```text
Workflow (Rule + AI + Human-in-the-loop trong một pipeline cố định)
```

**Vì sao chọn (3-4 câu):**

```text
Bài toán có nhiều bước phụ thuộc nhau nhưng thứ tự các bước hoàn toàn cố định, nên Workflow là mức vừa đủ. AI chỉ được đặt ở đúng một mắt xích — đọc chữ viết tay và trích xuất trường — là chỗ duy nhất mà logic cố định bó tay. Các bước còn lại (kiểm tra ảnh, validate theo danh mục, tính thành tiền, xuất file) đều giữ ở mức Rule để hệ thống dễ debug và kết quả tái lập được. Cuối cùng, Workflow cho phép đo từng bước riêng biệt, nên nhóm chứng minh được chính xác AI đã rút ngắn bước nào và rút được bao nhiêu.
```

**Vì sao không chọn mức đơn giản hơn (2-3 câu):**

```text
Không chọn Rule thuần vì Rule không giải quyết được bottleneck: dữ liệu đầu vào là chữ viết tay trên ảnh, không có cấu trúc để đặt điều kiện. Nếu chỉ dùng Rule (template Excel, validation, dropdown), nhân viên vẫn phải đọc và gõ đủ 160 trường mỗi ngày, tổng thời gian gần như không đổi — chỉ giảm được lỗi định dạng. Vì vậy nhóm vẫn giữ Rule nhưng đưa xuống vai trò hỗ trợ trong workflow, thay vì làm giải pháp chính.
```

### 6.2. Problem Statement v1 (v0 sửa chặt hơn + 3 field cuối)

| Field | Nội dung |
|---|---|
| **Actor** | Nhân viên nhập liệu bộ phận kho (1 người/ca), đầu vào là phiếu nhập kho viết tay do NV kho bàn giao cuối ngày, đầu ra là bản ghi trong Excel/hệ thống kho. Khối lượng: ~20 phiếu/ngày × 8 trường = ~160 trường/ngày. |
| **Workflow** | 7 bước hiện tại: nhận phiếu (5') → phân loại (5') → chụp/scan (10') → gõ tay vào Excel (70') → hỏi lại NV kho khi chữ khó đọc (15') → soát lại (15') → lưu/gửi (5'). Tổng ~125'/ngày, trong đó 6/7 bước là thao tác người. |
| **Bottleneck** | Bước 4 (gõ tay) chiếm ~56% tổng thời gian và tăng tuyến tính theo số phiếu; bước 5 là handoff gây chờ đợi vì phụ thuộc NV kho có mặt. Hai bước này cũng là nguồn của hầu hết lỗi số liệu phải truy ngược. |
| **Impact** | ~125 phút/ngày ≈ 10,4 giờ/tháng của một nhân viên dành cho việc sao chép dữ liệu. Lỗi nhập sai mã hàng/số lượng làm lệch tồn kho và tốn thêm thời gian đối chiếu của kế toán kho ở cuối tháng. |
| **Success Metric** | (1) Tổng thời gian lô 20 phiếu: 125' → ≤ 50'; (2) độ chính xác mức trường sau review ≥ 98%; (3) tỷ lệ trường phải sửa tay ≤ 25%. Đo bằng bấm giờ 5 ngày trước/sau trên cùng người–cùng loại phiếu, và chấm chéo 200 trường bởi người thứ hai. |
| **Boundary** (làm / không làm) | **Làm:** 1 loại biểu mẫu (phiếu nhập kho), 8 trường đã định nghĩa, ảnh chụp đạt chuẩn tối thiểu, xuất ra Excel/API. **Không làm:** biểu mẫu khác loại, phần ghi chú tự do, chữ viết chồng/tẩy xóa nặng, tự động ghi thẳng vào hệ thống kho, xử lý real-time từng phiếu. |
| **AI intervention point** (can thiệp sau bước nào, trước bước nào) | AI can thiệp **sau bước kiểm tra chất lượng ảnh (Rule)** và **trước bước validate + human review**. Cụ thể: AI nhận ảnh đã đạt chuẩn, trả về 8 trường kèm confidence; AI không chạm vào bước thu thập phiếu đầu luồng và không chạm vào bước xuất dữ liệu cuối luồng. |
| **Mức chọn** (Rule / Workflow / Agent + 1 câu vì sao) | **Workflow** — vì chuỗi bước cố định và biết trước, chỉ cần AI ở đúng một mắt xích (đọc chữ tay), phần còn lại giữ bằng Rule để dễ debug và tái lập kết quả. |
| **Rủi ro & người thật kiểm tra** (rủi ro lớn nhất + ai kiểm tra bằng cách nào) | **Rủi ro lớn nhất:** AI đọc sai một chữ số (VD 3 → 8 ở cột số lượng) nhưng trả confidence cao nên lọt qua review, dẫn tới lệch tồn kho mà không ai biết. **Người kiểm tra:** nhân viên nhập liệu review mọi trường có confidence < 0,90 hoặc bị Rule gắn cờ ngay tại bước 5 (đối chiếu với ảnh gốc hiển thị song song); ngoài ra, toàn bộ trường số lượng và đơn giá luôn bị ép review 100% bất kể confidence trong giai đoạn pilot, và kế toán kho audit ngẫu nhiên 10% bản ghi auto-accept mỗi tuần. |

### 6.3. Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú (câu đầy đủ) |
|---|---|---|
| Actor + workflow rõ chưa? | Yes | Actor là nhân viên nhập liệu bộ phận kho và workflow đã được mô tả đủ 7 bước kèm thời gian, input/output và điểm handoff. |
| Baseline + metric đo được chưa? | Not Yet | Nhóm đã có baseline sơ bộ ~125'/lô 20 phiếu nhưng mới đo một lần, cần bấm giờ đủ 5 ngày liên tiếp trước khi coi đây là con số chính thức. |
| Data/input đủ dùng chưa? | Not Yet | Nhóm cần thu ít nhất 50-100 ảnh phiếu viết tay thật (đã che thông tin nhạy cảm) để đo accuracy; hiện mới có vài mẫu chụp thử. |
| AI sai, hậu quả chấp nhận được không? | Yes | Sai sót bị chặn tại bước review trước khi dữ liệu vào hệ thống, và trong pilot mọi trường số lượng/đơn giá đều bị ép review, nên hậu quả tối đa là mất thêm thời gian sửa chứ không làm hỏng dữ liệu kho. |
| Có người review/owner không? | Yes | Nhân viên nhập liệu là người review từng lô và là owner của dữ liệu đầu ra; kế toán kho là lớp kiểm tra thứ hai qua audit ngẫu nhiên hằng tuần. |
| Có cách non-AI đơn giản hơn không? | No | Nhóm đã cân nhắc template Excel + validation và cả phương án chuyển sang biểu mẫu điện tử; phương án thứ hai tốt hơn về dài hạn nhưng nằm ngoài quyền quyết định của nhóm và không áp dụng được cho phiếu đã viết tay. |

**Decision:**

```text
Go (có điều kiện) — chạy pilot hẹp trên 1 loại biểu mẫu, hoàn tất đo baseline và thu dữ liệu song song.
```

**Lý do (3-4 câu dựa trên bằng chứng):**

```text
Bottleneck đã được định vị rõ ở bước 4 với ~70/125 phút mỗi lô, và interview 3 người cùng survey 8 người đều xác nhận việc đọc–gõ lại dữ liệu viết tay là phần tốn thời gian nhất. Research cho thấy không cần tự xây OCR: Google Document AI, Azure Document Intelligence và Amazon Textract đều hỗ trợ handwriting và trả confidence từng trường, nên nhóm có thể ghép pipeline thay vì train từ đầu. Rủi ro lớn nhất — AI đọc sai mà confidence cao — đã có cơ chế chặn cụ thể: ép review 100% trường số lượng/đơn giá trong pilot cộng audit ngẫu nhiên 10%. Hai điểm chưa chắc (baseline mới đo một lần, chưa đủ dữ liệu ảnh thật) không đủ để dừng nhưng đủ để giữ phạm vi ở mức pilot thay vì triển khai rộng.
```

**Nếu Go — pilot nhỏ nhất (data nào, chạy tay ra sao, đo 3 số nào):**

```text
DATA: 50 ảnh phiếu nhập kho viết tay thật (đã che tên/số điện thoại), chỉ 1 loại biểu mẫu, 8 trường; chia 40 ảnh để chỉnh ngưỡng và 10 ảnh giữ riêng làm bộ test không đụng tới.

CHẠY TAY: chưa code hệ thống. Upload từng ảnh qua console/API của 1 nhà cung cấp OCR có sẵn (Document AI hoặc Document Intelligence), copy kết quả 8 trường + confidence vào một Google Sheet; viết tay 5-6 Rule validate ngay trong Sheet (kiểm định dạng ngày, mã hàng có trong danh mục, số lượng > 0, thành tiền = SL × đơn giá); một thành viên đóng vai người review, sửa các trường bị gắn cờ và bấm giờ.

ĐO 3 SỐ:
1. Thời gian xử lý trung bình / phiếu (từ lúc có ảnh đến lúc dòng dữ liệu được xác nhận) — so với baseline ~6,25'/phiếu.
2. Field-level accuracy: % trong 400 trường (50 phiếu × 8) khớp với phiếu gốc, chấm bởi người thứ hai.
3. Tỷ lệ trường phải sửa tay (confidence < 0,90 hoặc vi phạm Rule) — dùng để ước lượng công review thực tế.

NGƯỠNG ĐỂ ĐI TIẾP: accuracy ≥ 95% ở bộ test giữ riêng VÀ thời gian/phiếu giảm ≥ 40% so với baseline.
```

**Nếu Not Yet — cần validate gì trước:**

```text
Nếu pilot chưa đạt ngưỡng, cần validate 3 thứ trước khi mở rộng: (1) baseline thật bằng cách bấm giờ 5 ngày liên tiếp thay vì ước lượng một lần; (2) accuracy của OCR trên đúng nét chữ của những người thường viết phiếu (mỗi người 10 phiếu) để biết lỗi đến từ model hay từ một vài người viết xấu; (3) chất lượng ảnh đầu vào — thử chuẩn hóa cách chụp (kẹp giấy phẳng, đủ sáng, cùng khoảng cách) rồi đo lại, vì nhiều lỗi OCR có thể đến từ ảnh chứ không từ model.
```

**Nếu No-Go — làm gì thay AI:**

```text
Nếu accuracy trên chữ viết tay tiếng Việt quá thấp (< 85%) và không cải thiện sau khi chuẩn hóa ảnh, nhóm bỏ hướng OCR và chuyển sang giải pháp non-AI: thay phiếu giấy bằng biểu mẫu điện tử (Google Form/app nhập kho trên điện thoại) để NV kho nhập tại nguồn, phần nhập liệu lại chỉ còn kiểm tra. Song song, giữ template Excel có dropdown mã hàng và data validation cho các phiếu giấy còn tồn, đồng thời chuẩn hóa lại mẫu phiếu (ô rộng hơn, ô vuông cho từng chữ số) để giảm thời gian đọc — đây cũng là bước chuẩn bị tốt nếu sau này quay lại hướng OCR.
```

**Exit / rollback (khi nào dừng AI, quay về cách cũ):**

```text
DỪNG NGAY (rollback trong ngày): nếu phát hiện ≥ 2 bản ghi sai lọt vào hệ thống kho trong cùng một tuần, hoặc OCR gặp sự cố/hết quota — chuyển toàn bộ lô về nhập tay bằng template Excel cũ, quy trình cũ luôn được giữ nguyên vẹn làm đường lui.

DỪNG SAU ĐÁNH GIÁ (cuối pilot 2 tuần): nếu field-level accuracy < 95% trên bộ test giữ riêng, hoặc tổng thời gian không giảm được ≥ 30% so với baseline, hoặc tỷ lệ trường phải sửa tay > 40% (khiến review tốn ngang gõ tay) — kết luận No-Go và chuyển sang phương án biểu mẫu điện tử.

ĐIỀU KIỆN MỞ RỘNG: chỉ nhân rộng sang biểu mẫu thứ hai sau khi biểu mẫu đầu chạy ổn định 4 tuần liên tiếp, không có bản ghi sai lọt qua audit.
```

---

### Self-check nộp phần 02 (nhóm)
- [✓] Có nhật ký hội tụ 9-12 → 1 (cluster + shortlist + score)
- [✓] Có validation (quote thật) + research (link kiểm được) — 
- [✓] Có workflow trước/sau đủ thời gian, handoff, bottleneck, boundary, fallback
- [✓] Có PS v0 → v1, metric có trước/sau + cách đo, boundary có làm/không làm
- [✓] Có so sánh Rule/Workflow/Agent + Decision Go/Not Yet/No-Go có lý do

---

### Giả định cần kiểm chứng (không dùng làm kết luận)
1. Baseline ~125'/lô 20 phiếu và ~3,5'/phiếu ở bước gõ tay: mới ước lượng, cần bấm giờ 5 ngày thực tế.
2. Kỳ vọng giảm còn ~38'/lô: là mục tiêu, chưa phải kết quả đo.
3. Ngưỡng confidence 0,90: chọn theo kinh nghiệm, phải hiệu chỉnh lại trên chính bộ dữ liệu của nhóm sau pilot.
4. Độ chính xác OCR chữ viết tay tiếng Việt của các nhà cung cấp: chưa có số liệu tự đo, tài liệu Google ghi nhận handwriting tiếng Việt ở mức experimental.
