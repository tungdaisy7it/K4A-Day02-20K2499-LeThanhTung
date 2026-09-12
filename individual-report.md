# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên: Lê Thanh Tùng
- Mã học viên: 2A202602499
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...): Sinh viên năm cuối
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem): Code, Học tập, Nghe nhạc

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 | Lặp lại | Nhập liệu thủ công số và chữ từ báo cáo viết tay vào Excel | Nhân viên nhập liệu | 1 báo cáo mất trung bình 12 phút; thực hiện 25 báo cáo/ngày; bấm giờ 10 báo cáo |
| 2 | Tốn thời gian | Tổng hợp các báo cáo số liệu lặp lại hằng ngày vào file tổng | Nhân viên báo cáo | 15 báo cáo/ngày, trung bình 8 phút/báo cáo; tổng khoảng 2 giờ/ngày |
| 3 | Lặp lại | Sao chép số liệu từ nhiều file Excel vào một file tổng hợp | Nhân viên data | 8 file nguồn/ngày; mỗi lần tổng hợp mất 35 phút; thực hiện 5 ngày/tuần |
| 4 | AI có thể tốt hơn | Đọc ảnh/PDF rồi nhập thông tin thủ công vào Excel | Nhân viên nhập liệu | 30 tài liệu/ngày; trung bình 5 phút/tài liệu; khoảng 2,5 giờ/ngày |
| 5 | Lặp lại | Đối chiếu số liệu giữa báo cáo chi tiết và báo cáo tổng | Nhân viên kế toán | Kiểm tra 20 báo cáo/ngày; khoảng 4 phút/báo cáo; thực hiện hằng ngày |
| 6 | Tốn thời gian | Nhập cùng một thông tin vào nhiều biểu mẫu | Nhân viên hành chính | Một thông tin được nhập lại trung bình 3 lần; khoảng 40 trường hợp/ngày |
| 7 | AI có thể tốt hơn | Trích xuất số liệu từ các biểu mẫu có bố cục khác nhau | Nhân viên data | 4 loại biểu mẫu; khoảng 50 biểu mẫu/ngày; trung bình 4 phút/biểu mẫu |
| 8 | Lặp lại | Tạo báo cáo ngày bằng cách copy/paste dữ liệu và định dạng | Nhân viên vận hành | 1 báo cáo/ngày; mất khoảng 45 phút; thực hiện 5 ngày/tuần |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi:
- Ý dùng được:
- Ý bỏ vì không phải pain thật:

**Self-check Phase 1:**
- [✓] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [✓] Dùng ít nhất 3/4 lăng kính
- [✓] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

#### Problem Card #1 — Nhập liệu thủ công từ báo cáo viết tay

Problem 1 câu:
Nhân viên phải đọc và gõ lại số, chữ từ các báo cáo viết tay vào Excel hoặc hệ thống, gây tốn thời gian và dễ xảy ra sai sót.

Actor:
Nhân viên nhập liệu / nhân viên hành chính / kế toán.

Thời điểm / bối cảnh:
Khi nhận các báo cáo giấy hoặc ảnh chụp báo cáo viết tay cần chuyển thành dữ liệu số.

Current workflow 3-7 bước:

1. Nhận báo cáo giấy hoặc ảnh chụp.
2. Mở báo cáo và đọc từng dòng thông tin.
3. Đọc và nhận diện số/chữ viết tay.
4. Gõ lại dữ liệu vào Excel hoặc hệ thống.
5. Kiểm tra lại dữ liệu đã nhập.
6. Sửa các lỗi phát hiện được.
7. Lưu và gửi dữ liệu.

Bottleneck:
Bước đọc và gõ lại số/chữ viết tay thủ công.

Impact:
Mỗi báo cáo mất khoảng 12 phút; xử lý 25 báo cáo/ngày, tương đương khoảng 5 giờ/ngày. Dữ liệu nhập thủ công cũng có nguy cơ sai sót khi số lượng báo cáo tăng.

Success metric:
Giảm ít nhất 70% thời gian nhập liệu và đạt độ chính xác dữ liệu từ 95% trở lên.

Non-AI alternative:
Chuẩn hóa biểu mẫu, sử dụng form điện tử hoặc thuê thêm nhân viên nhập liệu.

AI hypothesis:
Sử dụng OCR/AI để nhận diện chữ viết tay, trích xuất số liệu và tự động đưa dữ liệu vào Excel; con người chỉ kiểm tra và sửa các trường AI không chắc chắn.

Quick gut:

[ ] No AI / process fix

[ ] Rule

[x] Workflow

[ ] Agent

[ ] Chưa biết


Draft workflow Card #1

CURRENT STATE — 12 phút

[1 Nhận báo cáo: 1'] → [2 Đọc báo cáo: 2'] → [3 Đọc chữ/số viết tay: 3'] → [4 Gõ dữ liệu: 4'] → [5 Kiểm tra: 2']  <-- bottleneck

FUTURE STATE — 4 phút

[1 Upload ảnh/PDF: 0.5'] → [2 OCR + AI trích xuất: 1'] → [3 Human review: 2.5']  <-- human boundary

Fallback: Nếu AI nhận diện sai hoặc độ tin cậy thấp thì đánh dấu trường dữ liệu cần kiểm tra để nhân viên sửa thủ công.


File đính kèm:
01-individual-problem-scan-workflow-card-1.png


---

#### Problem Card #2 — Xử lý báo cáo số liệu lặp lại hằng ngày

Problem 1 câu:
Nhân viên phải xử lý và tổng hợp các báo cáo số liệu có nội dung lặp lại hằng ngày bằng cách thực hiện nhiều thao tác thủ công.

Actor:
Nhân viên báo cáo / nhân viên vận hành / nhân viên data.

Thời điểm / bối cảnh:
Hằng ngày khi nhận các báo cáo số liệu từ nhiều nguồn và cần tổng hợp thành báo cáo chung.

Current workflow 3-7 bước:

1. Nhận các báo cáo số liệu trong ngày.
2. Mở từng file hoặc nguồn dữ liệu.
3. Kiểm tra và đọc số liệu.
4. Copy dữ liệu sang file tổng hợp.
5. Kiểm tra và đối chiếu số liệu.
6. Tính toán hoặc tổng hợp các chỉ số.
7. Hoàn thiện và gửi báo cáo.

Bottleneck:
Bước copy, tổng hợp và kiểm tra các số liệu lặp lại từ nhiều báo cáo.

Impact:
Xử lý khoảng 15 báo cáo/ngày; mỗi báo cáo mất 8 phút, tổng thời gian khoảng 2 giờ/ngày. Công việc phải lặp lại 5 ngày/tuần.

Success metric:
Giảm ít nhất 70% thời gian tổng hợp báo cáo và giảm số lỗi nhập/tổng hợp xuống dưới 2%.

Non-AI alternative:
Chuẩn hóa file Excel, dùng công thức, Power Query hoặc tạo template báo cáo cố định.

AI hypothesis:
Xây dựng workflow tự động nhận dữ liệu từ các báo cáo, chuẩn hóa dữ liệu, tổng hợp và tạo báo cáo định kỳ; con người chỉ kiểm tra kết quả trước khi gửi.

Quick gut:

[ ] No AI / process fix

[x] Rule

[x] Workflow

[ ] Agent

[ ] Chưa biết


Draft workflow Card #2

CURRENT STATE — 120 phút

[1 Nhận báo cáo: 10'] → [2 Mở/kiểm tra dữ liệu: 25'] → [3 Copy dữ liệu: 35'] → [4 Tổng hợp + tính toán: 30'] → [5 Kiểm tra: 20']  <-- bottleneck

FUTURE STATE — 35 phút

[1 Nhận dữ liệu: 5'] → [2 Workflow tự động tổng hợp: 10'] → [3 Human review: 20']  <-- human boundary

Fallback: Nếu dữ liệu thiếu, sai định dạng hoặc workflow không xử lý được thì đưa báo cáo vào danh sách cần xử lý thủ công.


File đính kèm:
01-individual-problem-scan-workflow-card-2.png


---

#### Problem Card #3 — Đọc thông tin từ ảnh/PDF và nhập vào Excel

Problem 1 câu:
Nhân viên phải đọc thông tin từ ảnh hoặc PDF rồi nhập thủ công vào Excel hoặc hệ thống quản lý dữ liệu.

Actor:
Nhân viên nhập liệu / nhân viên hành chính / nhân viên data.

Thời điểm / bối cảnh:
Khi nhận nhiều ảnh hoặc PDF chứa thông tin cần chuyển thành dữ liệu có cấu trúc.

Current workflow 3-7 bước:

1. Nhận ảnh/PDF từ email, Zalo, Drive hoặc hệ thống.
2. Mở từng tài liệu.
3. Đọc và xác định các trường thông tin cần lấy.
4. Gõ dữ liệu vào Excel hoặc hệ thống.
5. Kiểm tra dữ liệu.
6. Sửa lỗi nhập liệu.
7. Lưu dữ liệu và chuyển sang tài liệu tiếp theo.

Bottleneck:
Bước đọc tài liệu và chuyển thông tin từ ảnh/PDF sang dữ liệu có cấu trúc.

Impact:
Xử lý khoảng 30 tài liệu/ngày; trung bình 5 phút/tài liệu; tổng thời gian khoảng 2,5 giờ/ngày.

Success metric:
Giảm ít nhất 70% thời gian nhập liệu và đạt độ chính xác trích xuất từ 95% trở lên.

Non-AI alternative:
Sử dụng biểu mẫu điện tử, yêu cầu dữ liệu đầu vào theo một template cố định hoặc dùng công cụ nhập liệu có cấu trúc.

AI hypothesis:
Sử dụng OCR kết hợp AI để đọc ảnh/PDF, xác định các trường thông tin, chuẩn hóa dữ liệu và tự động ghi vào Excel/hệ thống.

Quick gut:

[ ] No AI / process fix

[ ] Rule

[x] Workflow

[ ] Agent

[ ] Chưa biết


Draft workflow Card #3

CURRENT STATE — 5 phút

[1 Nhận ảnh/PDF: 0.5'] → [2 Mở và đọc tài liệu: 1.5'] → [3 Xác định thông tin: 1'] → [4 Nhập Excel: 1.5'] → [5 Kiểm tra: 0.5']  <-- bottleneck

FUTURE STATE — 1.5 phút

[1 Upload ảnh/PDF: 0.2'] → [2 OCR + AI trích xuất: 0.3'] → [3 Human review: 1']  <-- human boundary

Fallback: Nếu ảnh/PDF không rõ, thiếu thông tin hoặc AI có độ tin cậy thấp thì chuyển tài liệu sang xử lý thủ công.


File đính kèm:
01-individual-problem-scan-workflow-card-3.png

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

Card #1 — Nhập liệu thủ công từ báo cáo viết tay

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

Tôi chọn bài toán nhập liệu từ báo cáo viết tay vì workflow khá rõ: nhận báo cáo → đọc chữ/số → nhập dữ liệu → kiểm tra → lưu dữ liệu. Bottleneck nằm chủ yếu ở bước đọc và gõ lại dữ liệu thủ công, có thể đo bằng thời gian xử lý mỗi báo cáo, số báo cáo mỗi ngày và tỷ lệ lỗi. Nếu ứng dụng OCR + AI để trích xuất dữ liệu, nhân viên có thể chuyển từ nhập liệu thủ công sang kiểm tra kết quả, qua đó giảm thời gian xử lý và hạn chế lỗi.

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

Chữ viết tay có đủ rõ và đủ đồng nhất để OCR/AI đạt độ chính xác chấp nhận được không?

Nếu AI nhận diện sai một số trường dữ liệu quan trọng thì cơ chế kiểm tra và chuyển sang xử lý thủ công nên được thiết kế như thế nào?

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra: Chưa có số liệu thực tế chứng minh vấn đề đủ lớn và chưa biết độ chính xác OCR đối với chữ viết tay trong thực tế.
- Tôi sửa gì: Bấm giờ nhiều báo cáo để đo thời gian trung bình, thống kê số lượng báo cáo/ngày và ghi nhận lỗi nhập liệu; sau đó thử nghiệm OCR trên một tập báo cáo thực tế để đo độ chính xác trước khi xây dựng workflow.

### Self-check nộp phần 01
- [✓] Có 5+ problems + top 3 Cards đủ field
- [✓] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [✓] Đã chọn 1 card pitch + câu hỏi challenge
