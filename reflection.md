# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Lê Thanh Tùng
- Mã học viên: 2A202602499
- Nhóm: C2
- Candidate problem nhóm chọn: #1 – Nhập liệu thủ công từ báo cáo viết tay (phiếu nhập kho viết tay → Excel)

---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

> Cột giữa: mình đã gắn sẵn **mốc trong file 02** để bạn biết phải chỉ vào chỗ nào. Bạn thay phần in nghiêng bằng việc thật của mình, kèm con số (bao nhiêu phút, bao nhiêu người, dòng nào trong bảng).

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | *Tôi liệt kê ___ problems, nộp top 3 là #__, #__, #__ trong bảng 3.1* | *VD: 2/3 candidate của tôi vào cluster A* |
| Pitch Problem Card | *Tôi pitch candidate #__, nhấn vào actor và bottleneck nào* | *VD: nhóm sửa lại mô tả điểm nghẽn thành "bước đọc + gõ lại", không phải "có báo cáo viết tay"* |
| Challenge bài của bạn khác | *Tôi hỏi bạn ___ câu gì về candidate #__* | *VD: nhờ câu hỏi đó, #4 bị hạ khỏi lựa chọn vì không dựng được baseline nhất quán* |
| Gom trùng / cluster | *Tôi đề xuất gộp #__ và #__ vào cluster __ vì ___* | *VD: rút 15 candidate xuống 4 cluster* |
| Chọn candidate problem | *Tôi chấm điểm tiêu chí nào, bảo vệ/phản đối bài nào* | *VD: tôi là người đề xuất giữ #10 làm phương án dự phòng* |
| Validation / research | *Tôi phỏng vấn __ người / khảo sát __ người, hoặc tra tool nào* | *VD: insight "pain nằm ở số lượng phiếu nhiều, không phải mọi phiếu viết tay" là từ interview của tôi* |
| Workflow nhóm | *Tôi bấm giờ bước nào, vẽ phần nào của sơ đồ 7 bước* | *VD: tôi phát hiện bước 5 (hỏi lại NV kho) là handoff gây chờ, trước đó nhóm bỏ sót* |
| Problem Statement | *Tôi viết field nào trong v0/v1, sửa gì từ v0 sang v1* | *VD: tôi ép Success Metric phải có mốc ≤ 50' và cách đo, thay vì "nhanh hơn"* |
| Rule / Workflow / Agent | *Tôi trả lời câu hỏi chốt nào, lập luận gì* | *VD: tôi là người chỉ ra Rule không chạm được bottleneck vì đầu vào là ảnh* |
| Decision | *Tôi đề xuất ngưỡng/điều kiện nào cho pilot* | *VD: tôi đề xuất ép review 100% trường số lượng & đơn giá trong pilot* |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
(Chỉ đúng 1 chỗ trong file 02 mà nếu bỏ bạn ra thì chỗ đó không có. Nói rõ: mục nào, câu nào, vì sao nó tồn tại nhờ bạn.)
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

> Dòng nào bạn thật sự dùng AI thì giữ, còn lại ghi `Không dùng` + lý do. Mình để sẵn vài gợi ý đúng với những gì đã xảy ra trong phiên làm việc với AI của nhóm — bạn chỉ giữ lại nếu chính bạn là người chạy phiên đó.

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | | | | |
| Problem Card | | | | |
| Workflow | *Nhờ AI dựng sơ đồ current workflow từ mô tả của nhóm* | *Tách được bước và gắn thời gian cho từng bước, nhìn ra bottleneck chiếm % bao nhiêu* | **AI tự bịa số liệu**: baseline 125'/lô, 70' cho bước gõ tay, 3,5'/phiếu đều là con số AI suy ra, không phải đo thật | *Đánh dấu toàn bộ là giả định và lên lịch bấm giờ 5 ngày để thay bằng số thật* |
| Research | *Nhờ AI tìm tool OCR/Document AI đã có* | *Gợi được 3 hướng: Google Document AI, Azure Document Intelligence, Amazon Textract + ý tưởng dùng confidence score* | *Mô tả năng lực tool nghe rất chắc chắn nhưng không kèm số đo cho chữ viết tay tiếng Việt* | *Mở từng link chính thức để kiểm, ghi rõ handwriting tiếng Việt còn ở mức experimental thay vì coi là đã chạy được* |
| Problem Statement | *Nhờ AI soi field nào còn mơ hồ trong v0* | *Chỉ ra Impact và Success Metric đang viết chung chung, không đo được* | *Bản AI viết ra vẫn nói "giảm đáng kể thời gian" — vẫn là chữ, chưa phải metric* | *Tự đặt mốc cụ thể (≤ 50'/lô, accuracy ≥ 98%) và ghi kèm cách đo, ai đo, đo trên bao nhiêu mẫu* |
| Rule / Workflow / Agent | *Nhờ AI so sánh 3 mức trên cùng bài* | *Khung so sánh rõ, tách được đâu là Rule đâu là AI trong cùng pipeline* | *Ban đầu AI nghiêng về phương án phức tạp, chưa tự hỏi "Rule có đủ không"* | *Tự trả lời 5 câu hỏi chốt, hạ xuống Workflow và giữ Rule ở bước kiểm ảnh + validate* |
| Decision | *Nhờ AI phác pilot và điều kiện dừng* | *Gợi ý cấu trúc pilot chạy tay không cần code* | *AI nghiêng về "Go" mà chưa nói rõ cái gì còn thiếu* | *Đổi thành Go có điều kiện, ghi rõ baseline chưa đủ và dữ liệu ảnh chưa đủ* |

---

## 3. Reflection câu hỏi mở

Chọn 3-4 câu trong 6 câu dưới để viết thành đoạn 8-12 câu (không trả lời bullet 1 dòng):
- Tôi học được gì khi nghe top 3 problems của các bạn khác?
- Nhóm có lúc nào bị solution-first, đòi làm Agent cho ngầu không?
- Tôi có thay đổi ý kiến sau khi bị challenge không, vì sao đổi?
- Tôi đóng góp gì thật sự vào artifact cuối, phần nào có dấu tay của tôi?
- Điều khó nhất khi viết Problem Statement là gì, metric hay boundary?
- Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?

### Câu hỏi tự soi để bạn có chất liệu (trả lời nhanh ra nháp trước khi viết đoạn)

1. Lúc nghe 15 candidate, có bài nào làm bạn nghĩ "ơ, cái này giống bài mình nhưng bạn ấy mô tả sắc hơn"? Sắc hơn ở chỗ nào — actor, bottleneck, hay số đo?
2. Có lúc nào trong nhóm ai đó (kể cả bạn) nói kiểu "cho AI đọc rồi tự điền luôn" trước khi biết bottleneck nằm ở đâu không? Ai kéo lại, bằng câu gì?
3. Bạn đã bảo vệ ý nào rồi bỏ? Câu hỏi nào của người khác làm bạn bỏ — nhắc lại đúng câu đó.
4. Khi viết metric, bạn viết bản đầu là gì và bản sau là gì? Cái gì làm bạn biết bản đầu chưa đo được?
5. Boundary: có thứ gì bạn muốn đưa vào phạm vi mà nhóm cắt đi không (VD phần ghi chú tự do, nhiều loại biểu mẫu)? Bạn thấy cắt đúng hay tiếc?
6. Con số baseline 125'/lô hiện vẫn là giả định. Bạn có thấy khó chịu với việc nhóm đang xây cả quyết định trên một con số chưa đo không? Lần sau bạn sẽ chặn chỗ đó thế nào?

**Reflection:**

```text
(8-12 câu, viết liền mạch, bằng lời của bạn. Mỗi ý phải neo vào một chuyện cụ thể:
tên bài, số bước, câu ai đó đã nói, con số bạn đo hoặc không đo được.
Tránh "em học được nhiều điều" — thay bằng "trước buổi này em nghĩ X, sau khi Y thì em thấy Z".)
```

---

## 4. Tự kiểm cuối bài (check trước khi nộp repo)

- [ ] [12đ] Cá nhân có 5+ problems + top 3 Problem Cards
- [ ] [12đ] Tôi đã pitch rõ + challenge nhóm đúng trọng tâm (ghi ở bảng mục 1)
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài — *file 02, mục 3.1 → 3.4*
- [x] [15đ] Nhóm có workflow trước/sau — *file 02, mục 5.1 và 5.2*
- [x] [20đ] Nhóm có PS v0/v1 với metric + boundary rõ — *file 02, mục 5.3 và 6.2*
- [x] [15đ] Nhóm có so sánh No AI / Rule / Workflow / Agent — *file 02, mục 6.1*
- [x] [10đ] Nhóm có Go / Not Yet / No-Go + lý do rõ — *file 02, mục 6.3*
- [ ] [10đ] Reflection này có vai trò thật + AI giúp/sai ở đâu + điều học được + nếu làm lại đổi gì
- [ ] [6đ] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp AI

### Còn thiếu trước khi nộp (chung với file 02)
- Quote nguyên văn của 3 người interview (mục 4.1 file 02) — hiện vẫn là placeholder.
- Baseline bấm giờ 5 ngày thật để thay các con số đang đánh dấu giả định.

---

### Tự test mục 4 dòng cuối (6đ) — nói thành tiếng trong 60 giây, không nhìn giấy

> Actor là ___ , mỗi ngày xử lý ___ . Workflow gồm ___ bước, bottleneck ở bước ___ vì chiếm ___% thời gian.
> Metric là ___ , đo bằng ___ . Boundary: làm ___ , không làm ___ .
> Mức chọn là ___ vì ___ , và không hạ xuống Rule được vì ___ .

Nếu có chỗ nào bạn phải mở file ra đọc mới nói được, đó là chỗ bạn chưa thật sự hiểu — quay lại đọc đúng mục đó trong file 02.