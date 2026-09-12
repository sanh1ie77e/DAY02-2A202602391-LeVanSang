# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên: Lê Văn Sang
- Mã học viên: 2A202602391
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...): Sinh Viên Năm 3 Đại Học FPT
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem): 

- một ngày của tôi thường là đi học và họp đồ án
- thường thì khi làm đồ án sẽ bị rất nhiều vấn đề ở khâu tìm tài liệu
- và nhiều lúc nhóm cũng khó sắp xếp lịch họp với nhau
- còn lại khoảng thời gian tôi có thể chơi game hoặc là đi thể dục
- và ngủ là phần cuối cùng
---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 | tốn thời gian | tôi thường mất rất nhiều thời gian tìm tài liệu phù hợp | Bản thân | tôi thường dành 50-60p/1buoi để tìm nhiều nguồn khác nhau |
| 2 | tốn thời gian | nhóm tôi khó sắp xếp lịch họp chung | Nhóm tôi | Nhóm tôi thường hẹn giữa chừng có lúc người này bận người kia bận nên khó nhất quán |
| 3 | tốn thời gian | tôi thường hay tìm tài liệu trên web trường | Bản thân | sau những buổi học tôi thường không hay lưu tài liệu và thường phải lên lại web lục lại |
| 4 | lặp lại | check lịch học trên fap | Tôi và cả lớp | tôi bị một lần trường thay đổi lịch thi nhưng không vào kiểm tra |
| 5 | AI có thể tốt hơn | gặp lại lỗi từng fix nhưng không nhớ | tôi và nhóm | thường nếu không hỏi AI sẽ mất 20-30p để fix vấn đề |
| 6 | | | | |
| 7 | | | | |
| 8 | | | | |
| 9 | | | | |
| 10 | | | | |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi: tôi là sinh viên năm 3 fpt thì tôi đag trong giai đoạn chuẩn bị đồ án cho bản thân và nhóm của mình 
- Ý dùng được: AI đã gợi ý trúng các vấn đề thực tế khi làm dự án như việc tốn thời gian sinh mock data/viết test case cho hệ thống, và vấn đề trôi tin nhắn khi chia task thảo luận nhóm.
- Ý bỏ vì không phải pain thật: AI gợi ý "Xây dựng một chatbot AI tự động quản lý tiến độ thay nhóm trưởng". Ý này bị bỏ vì phạm vi quá rộng (không có workflow cụ thể), và thực tế nhóm chỉ cần dùng Trello hay Notion là đủ, không phải điểm nghẽn (pain) thật sự bắt buộc dùng AI.

**Self-check Phase 1:**
- [ ] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [ ] Dùng ít nhất 3/4 lăng kính
- [ ] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Gặp lại lỗi từng fix nhưng không nhớ (mất 20-30p để fix lại) | Workflow rõ (Gặp lỗi -> Tìm cách cũ -> Fix) | Làm sao hệ thống/AI phân biệt được lỗi cũ với lỗi mới nếu thông báo lỗi in ra giống hệt nhau nhưng nguyên nhân logic code lại khác nhau |
| 2 | 	Tìm lại tài liệu/slide cũ trên web trường khi ôn thi | Pain thật, nhiều bạn cùng lớp cũng gặp | Impact khó đo bằng con số ngoài thời gian tìm kiếm, phạm vi có thể quá rộng (nhiều môn) |
| 3 |  | Mức độ tác động (Impact) cực kỳ nghiêm trọng,Điểm nghẽn rõ ràng trong thói quen | Hệ thống FAP thường xuyên yêu cầu đăng nhập và có mã bảo mật (Captcha). Việc tự động hóa lấy dữ liệu (crawl data) sẽ gặp rào cản kỹ thuật |

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — [Tên problem]

```text
Problem 1 câu:Khi làm đồ án, tôi và nhóm thường gặp lại lỗi cũ nhưng không nhớ cách giải quyết, dẫn đến mất 20-30 phút lục lọi lịch sử chat hoặc search cách fix lại từ đầu.

Actor: Sinh viên IT (Tôi và các thành viên nhóm đồ án).

Thời điểm / bối cảnh: Trong quá trình code, chạy test và debug dự án chung.

Current workflow 3-7 bước:
1. Gặp lỗi (bug văng ra trên màn hình IDE/Terminal).
2. Cố gắng nhớ lại xem tuần trước ai fix lỗi này chưa.
3. Lục lọi lại lịch sử Zalo/Messenger của nhóm hoặc tra Google.
4. Đọc, thử áp dụng các cách fix.
5. Fix thành công và chạy tiếp.

Bottleneck: Bước 3. Việc lướt tìm lịch sử chat trôi tuột hoặc tra Google lại từ đầu làm đứt mạch suy nghĩ, tốn 20-30 phút.

Impact: Gây ức chế, giảm tốc độ hoàn thành đồ án, lãng phí thời gian lặp đi lặp lại.

Success metric: Giảm thời gian tìm lại cách fix từ 30 phút xuống dưới 3 phút; không ai trong nhóm phải hỏi lại "Lỗi này bữa trước ai fix ấy nhỉ?".

Non-AI alternative: Cả nhóm lập 1 file Notion chung, ai fix xong lỗi gì thì copy log lỗi và cách fix dán vào đó.

AI hypothesis: AI đọc trực tiếp log lỗi trên IDE, tự động quét trong "kho lỗi nội bộ" của nhóm và hiển thị ngay cách fix cũ mà không cần tra cứu thủ công.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #1** (ASCII / Mermaid / ảnh đính kèm):

```text
CURRENT STATE — 35 phút

[1 Gặp lỗi: 1'] → [2 Hỏi nhau/Cố nhớ: 4'] → [3 Lục tìm lịch sử chat/Google: 20'] <-- bottleneck → [4 Áp dụng & Debug: 10']

FUTURE STATE — 13 phút

[1 Gặp lỗi: 1'] → [2 AI khớp log lỗi với DB của nhóm: 2'] → [3 Dev đọc đề xuất review: 2'] <-- human boundary → [4 Áp dụng & Debug: 8']

Fallback: Nếu AI không tìm thấy lỗi cũ trong DB hoặc gợi ý sai, dev tự search Google thủ công như bình thường.
```

File đính kèm (nếu vẽ riêng): `01-individual-problem-scan-workflow-card-1.png`

---

#### Problem Card #2 — [Tên problem]

```text
Problem 1 câu: Sau các buổi học, tôi thường không lưu tài liệu nên mỗi khi cần ôn tập lại phải lên web trường (CMS/LMS) dò tìm lại từng thư mục/file, tốn tới 50-60 phút.

Actor: Sinh viên (Bản thân).

Thời điểm / bối cảnh: Bắt đầu buổi tự học, ôn thi tại nhà.

Current workflow 3-7 bước:
1. Xác định chương/topic cần học.
2. Đăng nhập hệ thống học tập của trường.
3. Mở từng môn học, lục tìm vào từng tuần/slot.
4. Tải nhiều file về và mở lướt xem có đúng file cần tìm không.
5. Sắp xếp lại file và bắt đầu học.

Bottleneck: Bước 3 và 4. Việc mở từng thư mục và đọc lướt để phân loại tài liệu vô cùng rườm rà, tiêu tốn gần 1 tiếng đồng hồ.

Impact: Làm tụt cảm hứng học tập, lãng phí thời gian lẽ ra dành cho việc thực sự tiếp thu kiến thức.

Success metric: Giảm thời gian gom và lọc đúng tài liệu từ 60 phút xuống 10 phút.

Non-AI alternative: Tạo thói quen phân loại và lưu tải tài liệu ngay trên lớp vào thư mục Google Drive rõ ràng để về nhà không phải tìm lại.

AI hypothesis: AI nhận từ khóa môn học/topic, tự động quét kho tài liệu đã được index và trả về link file tải chính xác kèm tóm tắt nội dung để sinh viên chọn đúng file.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — 60 phút

[1 Đăng nhập CMS: 2'] → [2 Dò từng thư mục môn: 20'] → [3 Tải & kiểm tra lướt từng file: 30'] <-- bottleneck → [4 Bắt đầu học: 8']

FUTURE STATE — 12 phút

[1 Nhập tên topic/từ khóa: 1'] → [2 AI quét kho lưu trữ & tóm tắt: 5'] → [3 SV đọc review & chọn file: 4'] <-- human boundary → [4 Tải & học: 2']

Fallback: AI tổng hợp sai chủ đề, sinh viên quay lại hệ thống tự dò tìm từng tuần bằng tay.
```

File đính kèm: `01-individual-problem-scan-workflow-card-2.png`

---

#### Problem Card #3 — [Tên problem]

```text
Problem 1 câu: Việc kiểm tra lịch học/thi trên FAP lặp lại mỗi ngày rườm rà (phải đăng nhập, nhập Captcha), dẫn đến lười check và đôi khi bỏ lỡ thông báo đổi lịch thi.

Actor: Sinh viên FPT (Tôi và các bạn cùng lớp).

Thời điểm / bối cảnh: Mỗi sáng ngủ dậy hoặc đầu tuần.

Current workflow 3-7 bước:
1. Mở trình duyệt vào FAP.
2. Đăng nhập tài khoản.
3. Nhập mã Captcha (thường hay nhập sai phải làm lại).
4. Xem lịch tuần và dò mắt xem có thông báo đổi ngày/giờ không.
5. Ghi nhớ vào đầu.

Bottleneck: Bước 2 & 3 cồng kềnh làm sinh viên lười check. Bước 4 dò bằng mắt thủ công rất dễ bỏ sót lịch đổi đột xuất.

Impact: Đi học nhầm giờ, hoặc nghiêm trọng nhất là lỡ lịch thi (bị đánh trượt môn).

Success metric: Số lần quên lịch/nhầm lịch = 0. Giảm thời gian kiểm tra FAP chủ động mỗi sáng từ 5 phút xuống 0 phút.

Non-AI alternative: Viết một đoạn code tự động (Rule) để cào data lịch học mỗi 6h sáng và gửi tin nhắn tự động qua nhóm Zalo.

AI hypothesis: AI đọc file thông báo từ hệ thống, phân tích ngữ cảnh (ví dụ: đổi phòng học bình thường hay đổi lịch thi khẩn cấp) để bắn cảnh báo có còi báo động/ưu tiên cao cho sinh viên.

Quick gut:
[ ] No AI / process fix
[x] Rule
[ ] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE — 5 phút (Kèm rủi ro cực cao)

[1 Nhớ ra & Mở FAP: 1'] → [2 Đăng nhập & Captcha: 2'] <-- bottleneck → [3 Dò lịch bằng mắt: 2'] 

FUTURE STATE — 1 phút (Tự động hóa)

[1 Script tự cào data lịch từ FAP: 0'] → [2 Bắn thông báo Zalo/Tele: 0'] → [3 SV check tin nhắn điện thoại: 1'] <-- human boundary

Fallback: Tool cào data bị chặn/chết, sinh viên tự log in FAP bằng tay.
```

File đính kèm: `01-individual-problem-scan-workflow-card-3.png`

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**
```Card #1: Gặp lại lỗi (bug) từng fix nhưng không nhớ.

```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```Tôi chọn vấn đề này vì quy trình xử lý (Workflow) của nó rất rõ ràng: Gặp lỗi -> Tìm cách cũ -> Fix. Điểm nghẽn đo lường được bằng số liệu cụ thể (lãng phí 20-30 phút/lần cho cả nhóm). Về mặt tác động (Impact), đây là "nỗi đau" chung rất lớn đối với dân IT và các nhóm sinh viên chạy đồ án sát deadline.

```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```1. Việc dùng AI ở đây có bị "đao to búa lớn" quá không? Nếu cả nhóm chỉ cần kỷ luật lập 1 file Notion để ghi chú thủ công (Non-AI) thì có hiệu quả tương đương không?
2. Nếu màn hình terminal in ra thông báo log lỗi giống hệt nhau, nhưng nguyên nhân logic code bên trong lại khác nhau, làm sao AI phân biệt được để không gợi ý sai cách fix?

```

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra: AI sẽ gặp rủi ro lớn trong việc khớp mã lỗi (error matching) vì mỗi file code có dòng (line number) hoặc tên biến khác nhau. Metric hy vọng giảm xuống dưới 3 phút là hơi lạc quan.
- Tôi sửa gì: Tôi bổ sung rõ ranh giới con người (human boundary). Cụ thể, AI chỉ đóng vai trò "gợi ý" các cách fix cũ, dev vẫn phải tự đọc review và quyết định áp dụng chứ không để hệ thống tự động sửa code

### Self-check nộp phần 01
- [ ] Có 5+ problems + top 3 Cards đủ field
- [ ] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [ ] Đã chọn 1 card pitch + câu hỏi challenge
