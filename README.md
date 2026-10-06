# Track1_Day18_2A202602942_LuuManhHung

**Day 18 — Design the Experiment · Human-Centered AI Design**
Track 1 · Repo nộp bài cá nhân trên sản phẩm nhóm

---

## 1. Thông tin cá nhân và nhóm

| Trường | Nội dung |
| --- | --- |
| **MHV** | 2A202602942 |
| **Họ tên** | Lưu Mạnh Hùng |
| **Nhóm** | **Double Hờ** |
| **Thành viên** | Lưu Mạnh Hùng — **Option B (Cùng tổ chức)** · Trần Vũ Gia Huy — **Option C (Nháp sẵn)** |
| **Case** | **Case B — AI Notes: Personal Learning Notes** *(giữ nguyên case Day 17)* |
| **Công cụ prototype** | HTML/CSS/JS tĩnh trong repo — `prototype/` |

### ⚠️ Ba điểm lệch chuẩn so với đề bài — khai báo trước khi đọc tiếp

| Đề bài yêu cầu | Thực tế nhóm | Cách xử lý |
| --- | --- | --- |
| 3 thành viên · 3 options **A/B/C** | **2 thành viên · 2 options B/C** | Khai báo rõ ở đây và trong mọi artifact. Không bịa một option thứ ba để cho đủ số |
| **3 Practice Notes** làm evidence Day 17 | **1** (P01 — Tài) | Hypothesis Problem đứng trên một nguồn duy nhất; **Barrier** và **Consequence** để nguyên 🔴 *giả thuyết, không evidence* |
| **3 Feedback Notes** | **2** chắc chắn, **3** nếu chạy thêm được 1 tester ngoài giờ | Ghi đúng số note thật trong `group-feedback-synthesis.md` §0. Không nhân bản một phiên thành hai |

👉 Hệ quả quan trọng nhất: cả B và C **đều có AI sinh nội dung**, nên nhóm **không có hướng user-led / no-inference** làm đối chứng cho `H_C`. Chấp nhận có chủ đích — chi tiết ở `three-option-design-sheet.md` §2.7.

---

## 2. Hypothesis Problem — một giả thuyết duy nhất cho cả B và C

> **Khi** vừa học hoặc research một chủ đề và muốn giữ lại một phần kiến thức để dùng sau, **learner** gặp khó khăn trong việc **tìm lại nội dung đó cùng ngữ cảnh khi thực sự cần dùng**, vì **cách lưu hiện tại không khớp với cách họ tìm**, dẫn đến **phải dò lại, khôi phục hoặc research lại, làm chậm việc đang cần hoàn thành**.

| Thành phần | Evidence | Mức |
| --- | --- | --- |
| **Situation** — vừa học/research xong, có nội dung muốn giữ | E01, E02, E03 | 🟡 Medium — tự thuật, chưa neo vào một lần cụ thể |
| **User** — learner tự học | E01–E05 | 🟡 Medium |
| **Job** — tìm lại được kiến thức cần dùng, **cùng ngữ cảnh** | E03, E04 | 🟡 Medium |
| **Barrier** — cách lưu không khớp cách tìm | — | 🔴 **Giả thuyết, không có evidence** |
| **Consequence** — dò lại / research lại, chậm việc đang làm | — | 🔴 **Giả thuyết, không có evidence** |

**Không có evidence nào ở mức 🟢 Strong.** Hai ô 🔴 để nguyên là có chủ đích — đúng tinh thần GATE 1: không điền bù chỗ thiếu bằng suy diễn của nhóm.

Đầy đủ: `three-option-design-sheet.md` §1 · Evidence gốc Day 17: `day17-input-pack.md`

---

## 3. Solution Options — hai hướng, cùng một Hypothesis Problem

Cả hai **bắt đầu từ cùng Màn 1, cùng task, cùng bộ dấu vết, cùng desired outcome**. Chỗ duy nhất khác nhau là **critical interaction** ở Màn 2.

| | **Option B — Cùng tổ chức**<br>*Lưu Mạnh Hùng* | **Option C — Nháp sẵn**<br>*Trần Vũ Gia Huy* |
| --- | --- | --- |
| **Cơ chế** | Learner **chọn phạm vi** dấu vết → AI gom nhóm, đề xuất tiêu đề, **hỏi làm rõ** chỗ thiếu ngữ cảnh → learner duyệt **từng nhóm** | AI **tự soạn bản nháp** từ **toàn bộ** dấu vết, kèm trích nguồn và nhãn cảnh báo → learner đối chiếu rồi quyết định |
| **Trigger** | Learner chọn *"Cùng AI tổ chức"* | Hết bài học, hệ thống **đề nghị** — learner được **Bỏ qua** |
| **AI Act/Ask** | **Ask → Act** | **Act → Ask for confirmation** |
| **Lối thoát** | *"Tự viết, không cần AI"* | *"Huỷ bản nháp"* · *"Tạo lại, chỉ dùng chỗ tôi đã đánh dấu"* · *"Bỏ qua"* |
| **Trade-off** | Cân bằng công sức / agency · **thêm lượt tương tác** | Nhanh · **rủi ro duyệt qua loa, mất sắc thái** |

**Điểm chung bắt buộc:** không autosave · mọi nội dung AI tạo đều có **đường về nguồn** · AI **không sửa hoặc xoá** dấu vết gốc · nguồn mâu thuẫn thì **AI không tự chọn** · nội dung learner sửa **không** dùng để huấn luyện.

### Link prototype

| | Đường dẫn |
| --- | --- |
| **Option B** | [`prototype/index.html?opt=b`](prototype/index.html?opt=b) |
| **Option C** | [`prototype/index.html?opt=c`](prototype/index.html?opt=c) |
| Tester mới | thêm `&fresh=1` |

HTML tĩnh, chạy offline, không cần cài gì. Hướng dẫn mở và giới hạn đã biết: **`prototype-link.md`**
Human–AI decisions: `three-option-design-sheet.md` §3 · Spec build: `prototype-build-spec.md`
Ghi chú facilitator *(không cho tester xem)*: `prototype/ANNOTATION.md`

---

## 4. Đóng góp của tôi trong nhóm

### 4.1 Option tôi chịu trách nhiệm — **Option B · Cùng tổ chức**

- Chốt cơ chế **Ask → Act**: AI **chỉ xử lý dấu vết learner đã chọn**, không tự ý mở rộng phạm vi
- Thiết kế **luật gom nhóm** chạy động trên dấu vết thật của tester *(không phải ID cố định)*, và **cố ý để nhóm 1 "Điều bạn đã nắm được" gom rộng** — mọi highlight bị dồn chung bất kể thuộc mục nào. Đây là chỗ để quan sát learner có sửa lại hay không
- Chốt **tối đa 2 câu hỏi làm rõ**, cả hai đều bỏ qua được
- Chốt cơ chế **"Duyệt nhóm này"** từng nhóm — learner không lưu được cho tới khi duyệt hết
- Lối thoát **"Tự viết, không cần AI"** luôn hiện, không nằm sau menu

### 4.2 Shared context và content fixture

- Chốt fixture cụ thể khi bản phân tích của Gia Huy còn để trống: bài **"Prompt Engineering — 4 thành phần của một prompt hiệu quả"**
- **Cài sẵn một phép thử ở mục 3**: bài nói *"3–5 ví dụ **phủ được các nhóm khác nhau** tốt hơn 10 ví dụ cùng một nhóm — quyết định là **độ phủ**, không phải số lượng"*. Bản nháp của Option C **đánh rơi đúng mệnh đề đánh đổi này** → dùng để đo trực tiếp desired outcome *"đủ ngữ cảnh"*
- Chốt **learner tự đánh dấu** thay cho dấu vết có sẵn read-only — đảo lại quyết định cũ trong spec: việc tự chọn chỗ nào đáng giữ **chính là phần job đang điều tra**, không nên lấy mất
- Chốt **giữ dấu vết qua reset** để lượt option thứ hai ăn **đúng bộ input của lượt đầu** → giữ được Comparison Contract
- Chốt **3 đường vào Sổ ghi chú** *(pill trên nav · nút dưới bảng dấu vết · "Hoàn thành bài học")* để quan sát affordance nào thật sự được thấy
- Chốt quy ước **CSS tập trung một file** → nếu B và C trông khác nhau ngoài vùng Màn 2 thì chắc chắn có người viết CSS riêng, sai quy ước 70% dùng chung

### 4.3 Human–AI decisions

Sắp lại nội dung của Gia Huy theo khung Expectation · Role & Agency · Evidence & Uncertainty · Control & Recovery, hoàn thiện **Human–AI Decision Table** 5 dòng × 2 cột, và bổ sung điều khoản **nguồn mâu thuẫn → AI không tự chọn** — `three-option-design-sheet.md` §3.

### 4.4 Facilitation — phiên tôi chạy

Soạn **toàn bộ `test-script.md`**: Opening · 1 câu relevant context · Outcome task nói **kết quả** không nói **nút** · 5 observation focus nối thẳng về 4 giả định §3.4 · 6 luật facilitation · 3 câu cứu hộ · timeline 20 phút.
Chốt **thứ tự đảo chiều** B→C / C→B giữa các tester để tách *tác dụng của option* khỏi *tác dụng của việc gặp trước*.

### 4.5 Observation và tổng hợp

Soạn cấu trúc 4 lớp **OBSERVED → INTERPRETED → DECIDED → STILL UNPROVEN** cho `prototype-feedback-note.md`, và bảng synthesis + §0 khai báo lệch chuẩn cho `group-feedback-synthesis.md`.

### 4.6 Ba lỗi tự phát hiện trong lúc build và đã sửa

| # | Lỗi | Vì sao phải sửa |
| --- | --- | --- |
| 1 | Mục 3 của bài học có **viền trái**, nổi bật hơn các mục khác | Hút mắt tester vào **đúng chỗ Option C giấu lỗi** → **làm hỏng phép thử**. Đã bỏ, mọi mục giờ trông như nhau |
| 2 | `CH2` bị hỏi **trùng hai lần** ở Option B | Vừa báo *"chưa xếp được"* vừa có câu hỏi làm rõ → tester gặp cùng một thứ hai lần. Đã gộp |
| 3 | **Thiếu nút reset** ở các màn giữa, chỉ có ở Màn 3 | **Trượt GATE 4** — không có đường về common context. Đã thêm vào thanh dưới, có mặt ở **mọi màn** |
| 4 | Dấu vết *"Chưa hiểu"* **biến mất ở lượt option thứ hai** — `repaintAll()` so chuỗi thô, trong khi dấu vết lưu chuỗi đã gộp khoảng trắng | Lượt hai tester thấy bài **sạch hơn** lượt đầu → **phá Comparison Contract**. Tìm ra bằng dry-run, không thấy được bằng mắt. Đã sửa — `dry-run-report.md` §3 |

### 4.7 Dry-run trước phiên test

Chạy 41 điểm kiểm trên đúng đường tester sẽ đi — `dry-run-report.md`. Ngoài lỗi #4 ở trên, dry-run còn cho thấy **Option B có thể không hỏi câu làm rõ nào** tuỳ cách tester đánh dấu. **Tôi quyết định không sửa**: thêm một câu hỏi "cho có" sẽ phá nguyên tắc *AI chỉ hỏi khi thật sự thiếu ngữ cảnh* (§3.1) và làm hỏng chính giả định 1 đang đi kiểm. Thay vào đó ghi cảnh báo vào `prototype/ANNOTATION.md` và thêm nhánh *"B hỏi 0 câu"* vào Feedback Note.

---

## 5. Prototype Feedback

**Phiên tôi facilitate:** tester **Dương Quốc Khánh** (ngoài nhóm) · 05/10/2026 · thứ tự **B → C** · 10 phút
Đầy đủ: `prototype-feedback-note.md` · Tổng hợp nhóm: `group-feedback-synthesis.md`

> ⚠️ **Hai giới hạn phải đọc trước mọi kết luận bên dưới**
> 1. Tester **không có relevant context** — không kể được lần nào phải tìm lại kiến thức đã học. Phiên này **chỉ dùng cho interaction breakdown**, không đưa value claim.
> 2. **Facilitator đã giải thích màn hình** khi tester hỏi → vi phạm luật facilitation số 3. Mọi quan sát **sau** thời điểm đó không còn độc lập.

### Quan sát chính — OBSERVED

| | Đã xảy ra |
| --- | --- |
| **First action** | Bấm thẳng *"Hoàn thành bài học"* ở **cả hai lượt**; đọc lướt bài ~1 phút; tự đánh dấu, **có** đánh dấu ở mục 3 |
| **Breakdown nặng nhất** | **Dừng 3 phút ở B, 2 phút ở C** ngay khi vào màn Sổ ghi chú, rồi hỏi *"Bạn có thể giải thích tính năng của màn hình này không?"* |
| **Đọc evidence** | Có mở link nguồn, nhưng **3 giây** sau đã bấm Lưu — ở **cả B và C**. **Không** dừng ở khối gắn nhãn ⚠ |
| **Giữ ngữ cảnh** | Mệnh đề đánh đổi ở mục 3: **B còn · C mất** |
| **Lấy lại control** | Thấy và thử *"Tự viết, không cần AI"*; sửa nội dung AI tạo ra; **tìm nút "Bắt đầu lại" khá khó khăn** |
| **Option được chọn** | **B — Cùng tổ chức**: *"cách đánh dấu và note, duyệt qua từng note trực quan và dễ hiểu hơn với người sử dụng"* |
| **Trade-off tự nói ra** | *"Cách thoát khỏi màn hình ghi chú chưa có, tester chưa biết cách thoát như thế nào."* |
| **Riêng Option B** | AI **hỏi 0 câu làm rõ** với bộ dấu vết tester tạo — bước *Ask* không xuất hiện |

### Evidence đi ngược kỳ vọng của nhóm

| Nhóm kỳ vọng | Quan sát thật |
| --- | --- |
| Người dùng C **sẽ kiểm tra nguồn** | **Ngược lại** — mở nguồn rồi 3 giây sau bấm Lưu, bỏ qua khối ⚠ |
| Cả hai cách **giữ đủ ngữ cảnh** | **Ngược một nửa** — C **mất** mệnh đề mục 3 |
| Câu hỏi làm rõ của B **hỗ trợ** tổng hợp | **Không kiểm được** — B không hỏi câu nào |
| Prototype **không cần facilitator narrate** *(GATE 4)* | **Trượt** — tester phải hỏi để hiểu màn hình, ở cả hai option |

### Next Change — **đề xuất**, chưa chốt

Mới có **1/3 Feedback Note**, nên chưa chốt được Next Change của nhóm. Hướng từ FB1:

> Màn Sổ ghi chú của **cả 2B và 2C** phải có **một dòng nói rõ màn này làm gì** và **một nút thoát hiện rõ ở vị trí cố định.**

Dựa trên ba dòng OBSERVED độc lập: dừng 3′/2′ rồi phải hỏi · *"cách thoát chưa có"* · tìm nút *Bắt đầu lại* khó khăn.
**Đã cân nhắc rồi bỏ:** sửa cơ chế hỏi của B — vì phiên này không kiểm được giả định 1.

### Still Unproven

| | |
| --- | --- |
| **Có pattern hay không** | Một tester không tạo ra pattern. Cần FB2 chạy ngược chiều C → B |
| **Tester có *tự* bắt được dòng 3 không** | Facilitator đã giải thích giữa phiên → quan sát không độc lập |
| **B được chọn vì cơ chế hay vì gặp trước** | Chỉ một phiên, thứ tự B → C |
| **Có giúp tìm lại kiến thức về sau không** | Tester không có relevant context; 10 phút không đo được hành vi một tháng sau |
| **Barrier và Consequence** của Hypothesis Problem | Vẫn 🔴 giả thuyết — Chặng 6 không đo được chúng |
| **Chất lượng AI thật** | Output là canned, lỗi mục 3 cài sẵn → chỉ kết luận được *"learner có bắt được lỗi dạng này không"* |

**Không có chỗ nào trong bài này tuyên bố solution đã được validated.**

---

## 6. AI Support Log — bản tóm

Đầy đủ 10 entry: **`ai-support-log.md`**

### AI đã giúp gì

| Việc | Thuộc phạm vi được phép |
| --- | --- |
| Gợi ý cơ chế tương tác, kịch bản đối thoại mẫu | ✅ |
| Sinh **dữ liệu mẫu**: bài học, dấu vết, bản nháp canned của C, 2 câu hỏi làm rõ của B | ✅ synthetic data |
| Code **toàn bộ giao diện** prototype — 7 file trong `prototype/` | ✅ boilerplate prototype |
| **Dry-run** 41 điểm kiểm trên prototype trước phiên test | ✅ kiểm thử kỹ thuật |
| **Rà soát câu hỏi dẫn dắt** trong `test-script.md` | ✅ |
| Soạn cấu trúc 4 lớp của Feedback Note và bảng synthesis | ✅ khung trống, **không** nội dung |

### AI sai hoặc hời hợt ở đâu — ghi nhận trong lúc làm

| # | Chỗ sai | Hệ quả nếu không bắt |
| --- | --- | --- |
| 1 | Thiết kế **reset xoá sạch dấu vết** → lượt option thứ hai tester phải đánh dấu lại → **B và C ăn input khác nhau** | **Hỏng Comparison Contract** — hai option không còn so sánh được. Đã đổi sang giữ dấu vết qua reset, thêm `?fresh=1` để xoá khi đổi tester |
| 2 | Để mục 3 có **viền trái**, nổi hơn các mục khác | Hút mắt tester vào đúng chỗ C giấu lỗi → **làm hỏng phép thử** |
| 3 | Thiếu **nút reset** ở các màn giữa | **Trượt GATE 4** |
| 4 | Đề xuất câu hỏi test **"Bạn có tin vào bản nháp AI tạo ra không?"** | Chữ *"tin"* **báo trước** rằng có gì đáng nghi, ngay trước phép thử dòng 3 của C. **Tôi bỏ câu này**, đo hành vi thay vì hỏi niềm tin |
| 5 | Bản nháp đầu của Outcome task viết *"hãy dùng AI để tổng hợp lại ghi chú"* | Nói **cơ chế** thay vì **kết quả** → ép tester vào đúng đường nhóm muốn thấy |

> ⬜ **Phần phản ánh cá nhân — tôi tự viết, không nhờ AI** *(mục *"AI sai ở đâu / tôi tự sửa gì"* ở cuối `ai-support-log.md`)*. Bảng trên là **ghi nhận sự việc đã xảy ra trong lúc làm**, không thay cho phần phản ánh đó.

### ❌ Không dùng AI cho

- Tạo **quote, observation hoặc feedback giả** từ tester
- Làm sạch evidence tới mức mất ranh giới giữa **lời user thật** và **diễn giải của nhóm**
- Viết hộ **phần đóng góp cá nhân** và **reflection**

**Cam kết:** mọi quote, observation và feedback trong `prototype-feedback-note.md` và `group-feedback-synthesis.md` sẽ do tôi tự ghi trong phiên test thật. Hiện tại hai file đó **đang trống** đúng vì lý do này.

---

## Cấu trúc repo

| File | Nội dung | Trạng thái |
| --- | --- | --- |
| `README.md` | Bản này — 6 phần | ✅ |
| `three-option-design-sheet.md` | Chặng 1–4 đầy đủ, GATE 1–3 đã đạt | ✅ |
| `prototype/` | Prototype B/C + annotation facilitator | ✅ |
| `prototype-link.md` | Cách mở, ba màn hình, giới hạn đã biết | ✅ |
| `prototype-build-spec.md` | Spec build, 15 điểm trống đã chốt | ✅ |
| `test-script.md` | Chặng 5 — script facilitation | ✅ |
| `session-kit.md` | Tin nhắn mời tester · cue card · bản ghi tay thô | ✅ |
| `dry-run-report.md` | Diễn tập prototype — 41 điểm kiểm *(**không phải** evidence từ tester)* | ✅ |
| `prototype-feedback-note.md` | Phiên tôi facilitate | 🔴 **chờ phiên test thật** |
| `group-feedback-synthesis.md` | Tổng hợp feedback nhóm | 🔴 **chờ đủ Feedback Note** |
| `ai-support-log.md` | 10 entry | ✅ *(trừ phần reflection cá nhân)* |
| `day17-input-pack.md` | 4 artifact Day 17 làm input | ✅ |
| `two-option-design-sheet_v2.md` | Bản phân tích của Gia Huy | ✅ |
| `CHECKLIST.md` | Checklist lab 180 phút | ✅ |
| `docs/` | Đề bài gốc + ảnh giao diện VLearn | ✅ |

---

## Kết luận được phép

✅ "Với Hypothesis Problem này, chúng tôi đã thử **hai** cách giải. Tester đã làm…, vì vậy iteration tiếp theo chúng tôi sẽ…"
❌ "User đã xác nhận solution này đúng." — **không chỗ nào trong repo này tuyên bố solution đã được validated.**
