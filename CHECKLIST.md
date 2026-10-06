# Checklist — Day 18: Design the Experiment (Human-Centered AI Design)

**Repo:** `Track1_Day18_2A202602942_LuuManhHung` · **Thời lượng lab:** 180 phút
**Mô hình:** sản phẩm nhóm 3 người → nộp bài cá nhân. Mỗi người chịu trách nhiệm 1 option, nhưng **phải test cả A/B/C** với 1 tester ngoài nhóm.
> ⚠️ Đây là **nguyên văn đề bài**. Nhóm thực tế **2 người · 2 option B/C** — xem bảng lệch chuẩn ở §0. Mọi chỗ bên dưới nói "ba" đều phải đọc là **hai**.

---

## 📍 Trạng thái hiện tại

| Chặng | Trạng thái | Kết quả |
| --- | --- | --- |
| 0 · Chuẩn bị | ✅ | `day17-input-pack.md` |
| 1 · Evidence | ✅ GATE 1 | `three-option-design-sheet.md` §1 |
| 2 · Chọn option | ✅ GATE 2 | §2 |
| 3 · Human–AI pass | ✅ GATE 3 | §3 |
| 4 · Build prototype | ✅ GATE 4 *(tự kiểm)* | `prototype/` · `prototype-link.md` |
| 5 · Chuẩn bị test | ✅ | **`test-script.md`** · `session-kit.md` |
| 6 · Test 3 người | 🟡 **1/3 phiên đã chạy** | FB1 xong (Dương Quốc Khánh) · chờ FB2 của Gia Huy |
| 7 · AI Support Log | ✅ *(trừ reflection cá nhân)* | 12 entry |
| 8 · Nộp bài | ✅ *(trừ phần phụ thuộc Chặng 6)* | `README.md` 6 phần |

**Việc còn lại:**

1. ⬜ **Gia Huy chạy phiên của mình** (thứ tự C → B) → điền cột FB2 trong `group-feedback-synthesis.md` → điền cột *Pattern hoặc khác biệt* → **chốt** Next Change
2. ⬜ *(nếu kịp)* Tester thứ 3 ngoài giờ → FB3

✅ Đã xong: FB1 · README §5 · synthesis cột FB1 · phản ánh cá nhân ở `ai-support-log.md`

> Mọi thứ không cần tester đã xong: script, bộ đồ nghề phiên test, dry-run 41/41 điểm kiểm, và 1 lỗi prototype đã sửa trước khi tester gặp.

> ⚠️ Không điền bù, không nhờ AI sinh quote/observation/feedback của tester — `docs/10.md` cấm tuyệt đối.

---

## 0. Chuẩn bị trước khi bắt đầu — ✅ **HOÀN TẤT** → `day17-input-pack.md`

- [x] Đặt cạnh nhau 4 artifact từ Day 17 → `day17-input-pack.md`
- [x] Xác nhận giữ đúng case Day 17 → **Case B — AI Notes: Personal Learning Notes**
- [x] Chốt nhóm và phân công → **Double Hờ, 2 người:** Lưu Mạnh Hùng = **Option B — Cùng tổ chức**, Trần Vũ Gia Huy = **Option C — Nháp sẵn**
- [x] Chốt công cụ prototype → **HTML/CSS/JS trong repo**
- [ ] Chuẩn bị thiết bị chạy prototype + đồng hồ bấm giờ *(việc tay, làm trước Chặng 6)*
- [x] Mở sẵn `ai-support-log.md`, đã có Entry 01–03

### ⚠️ Ba điểm lệch chuẩn đã khai báo (phải ghi vào README)

| Đề bài yêu cầu | Thực tế nhóm | Cách xử lý |
| --- | --- | --- |
| 3 thành viên · 3 options A/B/C | **2 thành viên · 2 options B/C** | Khai báo rõ trong README; nên xác nhận với giảng viên/TA |
| 3 Practice Notes | **1 Practice Note** (P01 – Tài) | Khai báo + nêu giới hạn; không bịa evidence |
| 3 Feedback Notes | **2** (có thể lên 3 nếu chạy thêm 1 tester ngoài giờ) | Ưu tiên chạy thêm tester thứ 3 nếu kịp |

---

## 1. Chặng 1 — Tổng hợp evidence · 15 phút → ✅ **GATE 1 ĐẠT**

Kết quả: `three-option-design-sheet.md` §1.1–§1.5

- [x] Evidence huddle — 1 nguồn thật (P01 Tài), 2 dòng còn lại khai báo **không có**, không điền bù
- [x] Bảng tách *User thực sự làm/nói gì* vs *Điều nhóm đang diễn giải*
- [x] Trả lời 4 câu thảo luận
- [x] Hypothesis Problem đủ 5 thành phần — **`H_B`: giữ / tìm lại kiến thức**
- [x] Evidence Snapshot: 4 evidence hỗ trợ (🟡 Medium, **không có Strong**) + 3 evidence **chống lại** + 7 điều chưa chứng minh

**Chốt lại:** Barrier và Consequence đánh dấu 🔴 **giả thuyết, không có evidence** — cố ý để nguyên, đúng tinh thần GATE 1.

---

## 2. Chặng 2 — Chọn hai Solution Options · 20 phút → ✅ **GATE 2 ĐẠT**

Kết quả: `three-option-design-sheet.md` §2.0–§2.6

- [x] Soát lại Solution Parking Lot — 7 hướng đủ dùng, không cần thêm
- [x] Comparison Contract (phần giữ nguyên) — user · situation · task · desired outcome · fixture
- [x] Bảng khác biệt A/B — mechanism · user · AI · trigger · trade-off · điều gì hỏng khi AI sai
- [x] Distance check — viết không dùng một từ nào về màu/layout/wording
- [x] Tự soát 5 nguy cơ thiên vị
- [x] Ghi lý do **không** làm option co-create

**Hai option đã chốt** *(theo bản phân tích của Gia Huy — `two-option-design-sheet_v2.md`)*:

| | **Option B — Cùng tổ chức**<br>Lưu Mạnh Hùng | **Option C — Nháp sẵn**<br>Trần Vũ Gia Huy |
|---|---|---|
| Cơ chế | Learner **chọn phạm vi** → AI gom nhóm, đề xuất heading, **hỏi làm rõ** chỗ thiếu ngữ cảnh | AI **tự tạo bản nháp** từ toàn bộ dấu vết, kèm trích dẫn nguồn và cảnh báo phần không chắc |
| Trigger | Learner chọn *"Cùng AI tổ chức"* | Hoàn thành bài học; hệ thống đề nghị, learner được bỏ qua |
| AI Act/Ask | **Ask → Act** | **Act → Ask for confirmation** (không tự lưu) |
| Trade-off | Cân bằng công sức/agency · thêm lượt tương tác | Nhanh · rủi ro duyệt qua loa, mất sắc thái |

> ⚠️ **Giới hạn đã khai báo (§2.7):** cả B và C đều có AI sinh nội dung → nhóm **không có hướng user-led / no-inference** làm đối chứng cho `H_C`. Chấp nhận có chủ đích, phải ghi vào README.

---

## 3. Chặng 3 — Human–AI Design pass · 30 phút → ✅ **GATE 3 ĐẠT**

Kết quả: `three-option-design-sheet.md` §3.1–§3.5 — **nội dung do Gia Huy soạn**, đã sắp lại theo khung `docs/5.md`.

- [x] **Expectation** — cả hai gọi kết quả là *"đề xuất"* / *"bản nháp cần kiểm tra"*, nói rõ AI có thể nhóm sai / bỏ sót / suy diễn
- [x] **Role & Agency** — B: `Ask → Act` · C: `Act → Ask for confirmation`, **không tự lưu**. Không option nào sửa/xoá dấu vết gốc
- [x] **Evidence & Uncertainty** — mọi nội dung AI tạo đều có đường về nguồn; nhãn *"Cần bạn làm rõ"* (B) và nhãn cảnh báo (C); **nguồn mâu thuẫn thì AI không tự chọn**
- [x] **Control & Recovery** — preview trước khi lưu, **không autosave**; B có lối thoát *chuyển sang tự viết*, C có *huỷ toàn bộ và tạo lại hẹp hơn*
- [x] Human–AI Decision Table đủ 5 dòng × 2 cột
- [x] Feedback & data check — chỉnh sửa **không** dùng để huấn luyện; user rút quyền được

**4 giả định mang sang Chặng 5–6** (§3.4): B có làm ngắt mạch tổng hợp không · C có thật sự kiểm tra nguồn không · cả hai có giữ đủ ngữ cảnh không · tự tổng hợp là pain hay giá trị.

---

## 4. Chặng 4 — Build hai micro-prototype · 80 phút → ✅ **GATE 4 ĐẠT (tự kiểm)**

> ✅ **Spec đã chốt xong:** `prototype-build-spec.md` — 15 điểm trống trong bản của Gia Huy đã giải quyết hết (bài học, 7 dấu vết, logic nhóm của B, 2 câu hỏi làm rõ, bản nháp của C, 2 recovery path, Màn 3, **đường reset**, **thứ tự test đảo chiều**, cấu trúc file, annotation, giới hạn). **Build được ngay.**

**Scope:** mỗi option chỉ 2–3 màn hình/trạng thái → `COMMON CONTEXT → CRITICAL INTERACTION → RESULT / USER DECISION`
**Dùng chung ~70%:** context screen · content/data fixture · component và visual style · task và desired outcome. **Chỉ critical interaction khác rõ.**

### Build order
- [x] **Phút 0–10** — common context, task và content fixture dùng chung → `index.html` + `fixture.js`
- [x] **Phút 10–55** — build 2 option bằng shared components → `option-b.html` · `option-c.html`
- [x] **Phút 55–65** — control/recovery và evidence/uncertainty → lối thoát ở cả hai, link nguồn, nhãn ⚠
- [x] **Phút 65–75** — tự test chéo bằng trình duyệt → `three-option-design-sheet.md` §4.4
- [x] **Phút 75–80** — chuẩn hoá B/C, kiểm link và reset path

### Definition of testable — soát từng mục
- [x] Tester tự mở và thao tác được cả B/C — HTML tĩnh, chạy offline, không cần cài gì
- [x] Cả hai bắt đầu từ **cùng một context và task** — cùng `index.html`, cùng Outcome task
- [x] Không cần facilitator narrate mới hiểu — mọi nhãn và nút đều tự giải thích trên màn hình
- [x] Nội dung đủ thật để tester ra quyết định — bài Prompt Engineering 4 mục, dấu vết do learner tự tạo
- [x] Mỗi option thể hiện rõ **điểm user lấy lại control** — B: *Tự viết* · C: *Huỷ bản nháp* / *Tạo lại hẹp hơn*
- [x] Có **đường reset** về common context — *"Bắt đầu lại"* ở thanh dưới, có mặt ở **mọi màn**
- [x] **Quy ước 70% dùng chung được kiểm bằng code** — không file HTML nào có `<style>` riêng, cả ba nạp `shared.css`, Màn 3 của B và C gọi **cùng** `renderSaved()`
- [x] **Dry-run 41/41** trên đúng đường tester sẽ đi → `dry-run-report.md`
- [x] Một người chưa thấy prototype đã mở thử — Dương Quốc Khánh, 05/10/2026. ⚠️ **Nhưng facilitator đã phải giải thích** khi tester hỏi → **GATE 4 trượt ở tiêu chí "không cần narrate"**, đã khai báo ở `prototype-feedback-note.md` §0 và §4

### Prototype annotation — đặt ngoài frame, tester không thấy
- [x] Mỗi màn ghi đủ `We expect the tester to` / `Watch for` / `Do not explain` → `prototype/ANNOTATION.md`
- [x] Ghi rõ **chỗ cài cắm** (dòng 3 bản nháp của C nói ngược với mục 3 của bài) + câu trả lời khi tester hỏi *"cái này đúng không?"*

### Ranh giới
- ✅ Được dùng: Figma/Framer, HTML-CSS-JS, prototype giấy có flow rõ, canned AI output, Wizard of Oz (người mô phỏng AI **không giải thích giao diện hộ tester**)
- ❌ Không cần: model hoặc API thật, full onboarding/dashboard, responsive đa thiết bị, visual polish hoàn chỉnh, failure catalog đầy đủ

- [x] Ghi link B/C vào `prototype-link.md` — kèm ba màn hình, ba đường vào Sổ ghi chú, giới hạn đã biết

> **GATE 4 — Test-ready:** Một người **không build** mở được, làm cùng task qua B/C và quay về context ban đầu mà **không cần ai giải thích**.
> ❌ Trượt nếu: facilitator phải giải thích, hoặc một option hoàn thiện hơn hẳn hai option còn lại.

---

## 5. Chặng 5 — Chuẩn bị test · 15 phút → ✅ **XONG** → `test-script.md`

- [x] **1 câu hỏi relevant context** → `test-script.md` §2, kèm bảng xử lý ba trường hợp trả lời. Tester không có context liên quan thì **vẫn test**, nhưng ghi rõ *không đưa value claim mạnh*
- [x] **Outcome task** → §3 — nói kết quả cần đạt *(lưu phần quan trọng · một tháng sau vẫn hiểu · biết nguồn)*, **không nhắc nút, không nhắc chữ "AI"**
- [x] **5 observation focus** → §4, mỗi focus nối thẳng về một giả định ở `three-option-design-sheet.md` §3.4: F1 first action · F2 hesitation/ngắt mạch · F3 evidence đọc hay bỏ qua · F4 mất ngữ cảnh · F5 correction + option được chọn
- [x] **6 luật facilitation** → §5
- [x] **3 câu cứu hộ** → §5
- [x] Nhờ AI rà soát bộ câu hỏi — **bắt được 3 chỗ dẫn dắt, đã sửa; 1 đề xuất của AI bị tôi bỏ** → `test-script.md` §8 · `ai-support-log.md` Entry 10
- [x] **Thêm:** chốt thứ tự đảo chiều B→C / C→B giữa các tester, và checklist mang theo phiên → §6, §9
- [x] Việc tay trước phiên — đã làm, phiên đã chạy 05/10/2026

---

## 6. Chặng 6 — Test với ba người · 20 phút cuối hoặc ngoài giờ → **GATE 5** · 🔴 **CHƯA CHẠY**

> **Khung đã sẵn, nội dung cố ý để trống.** `prototype-feedback-note.md` và `group-feedback-synthesis.md` đã có đủ ô và luật điền.
> **Không điền bù, không nhờ AI sinh quote/observation** — `docs/10.md` cấm tuyệt đối. Đây là phần **chỉ chạy phiên test thật mới có**.

### Đã chuẩn bị xong — không cần tester

- [x] **Script facilitation** → `test-script.md`
- [x] **Tin nhắn mời tester** (bản gửi riêng · bản đăng nhóm · câu xin phép ghi âm) → `session-kit.md` §A
- [x] **Cue card một trang** cầm trong tay suốt phiên → `session-kit.md` §B
- [x] **Bản ghi tay thô** in sẵn, có dòng thời gian và ô bấm giây → `session-kit.md` §C
- [x] **Dry-run prototype — 41/41 điểm kiểm** → `dry-run-report.md`
  - [x] Tìm ra và **đã sửa** lỗi dấu vết *"Chưa hiểu"* biến mất ở lượt option thứ hai *(phá Comparison Contract)*
  - [x] Ghi nhận **Option B có thể hỏi 0 câu làm rõ** — cố ý không sửa, đã cảnh báo trong `prototype/ANNOTATION.md`
  - [x] 4 ảnh chụp các màn → `prototype/screenshots/`
- [x] **Xử lý sự cố giữa phiên** → `prototype/ANNOTATION.md`
- [x] **Việc làm ngay sau phiên**, 5 bước 10 phút → `session-kit.md` §D

### Còn lại — chỉ phiên test thật mới làm được

- [x] ~~Chốt 3 tester~~ → **1 tester đã test**: Dương Quốc Khánh (ngoài nhóm). ⬜ còn FB2, FB3. ⚠️ Tester này **không có relevant context** — đã khai báo
- [x] Hùng đã facilitate 1 phiên, chạy đủ **B → C** · ⬜ Gia Huy chưa chạy phiên C → B
- [ ] Nếu 20 phút cuối không đủ: tự hẹn tester và hoàn tất **ngoài giờ trước deadline** (không cần transcript hay report dài)

### Timeline mỗi phiên 20 phút
- [x] **0–2'** make comfortable + hỏi relevant context ngắn
- [x] **2–14'** tester dùng B/C *(thực tế 10 phút cả phiên — ngắn hơn protocol, đã khai báo)*, khoảng 4 phút mỗi option
- [x] **14–18'** so sánh: *"Bạn chọn **cách thứ nhất hay cách thứ hai**? Vì sao?"* ← **không** gọi tên B/C, tester không biết tên option · *"Bạn muốn tự làm phần nào, giao AI phần nào?"* · *"Điều gì ở phương án đã chọn khiến bạn chưa thoải mái?"*
- [x] **18–20'** hoàn thành Feedback Note ngay tại chỗ
- [x] Đọc đúng **Opening** — bản chuẩn ở `test-script.md` §1: *"Chúng mình đang thử **hai** cách thiết kế, không kiểm tra bạn. Không có câu trả lời đúng hoặc sai…"* ⚠️ Đề bài viết *"ba"*; nhóm chỉ có hai option → **nói đúng "hai"**

### Prototype Feedback Note cá nhân → `prototype-feedback-note.md` *(khung ✅ · nội dung 🔴 chờ phiên test)*
- [x] Tester / context
- [x] First action
- [x] Chỗ dừng, do dự hoặc hiểu sai
- [x] Evidence được đọc hay bỏ qua
- [x] Cách tester sửa hoặc lấy lại control
- [x] Option được chọn → **B**
- [x] Lý do và trade-off
- [x] **Evidence chống lại kỳ vọng của nhóm** — 4 dòng
- [x] Tách rõ 4 lớp: **OBSERVED** → **INTERPRETED** → **DECIDED (Next Change)** → **STILL UNPROVEN**

### Group Feedback Synthesis — sau khi có đủ note → `group-feedback-synthesis.md` *(khung ✅ · nội dung 🔴 chờ note)*
- [ ] Bảng 5 dòng × 3 feedback + cột **Pattern hoặc khác biệt**: first action · breakdown chính · cách lấy lại control · option được chọn · trade-off
- [ ] Chốt **một Next Change** của nhóm: giữ 1 option và sửa interaction / kết hợp 2 option nhưng giữ 1 cơ chế chính rõ ràng / bỏ 1 option / sửa cả ba rồi test người tiếp theo
- [ ] Ghi **evidence nào dẫn tới quyết định đó**
- [ ] Ghi **Still Unproven** sau ba feedback

> **GATE 5 — Learning, not praise:** 3 Feedback Notes độc lập + pattern hoặc khác biệt + 1 Next Change + 1 điều chưa chứng minh.
> ❌ Trượt nếu: chỉ đếm "ba tester thích B", hoặc tuyên bố solution đã validated.

---

## 7. AI Support Log → `ai-support-log.md` — **11 entry đã ghi**

- [x] Ghi rõ **AI đã giúp gì** và **AI sai hoặc hời hợt ở đâu** — 5 chỗ sai đã ghi nhận: reset xoá dấu vết làm hỏng Comparison Contract · mục 3 nổi hơn các mục khác · thiếu nút reset · câu hỏi *"bạn có tin không?"* bị tôi bỏ · Outcome task nói cơ chế thay vì kết quả
- [x] Chỉ dùng AI trong phạm vi được phép: cơ chế tương tác · dữ liệu mẫu · canned output · code giao diện · rà soát câu hỏi dẫn dắt · **khung trống** của Feedback Note
- [x] Không vi phạm điều nghiêm cấm — **không một quote/observation/feedback nào do AI sinh**; `prototype-feedback-note.md` và `group-feedback-synthesis.md` đang trống đúng vì lý do này
- [x] Mọi lần dùng AI đều khai báo — Entry 01–11
- [x] **Phần tôi tự viết:** *"Khai báo cuối"* và toàn bộ ô *"Tôi đã sửa gì"* ở Entry 01–13 — đã xong

---

## 8. Nộp bài

### Cấu trúc repo tối thiểu
- [x] `README.md` — 6 phần đầy đủ
- [x] `three-option-design-sheet.md` — Chặng 1–4
- [x] `prototype-link.md` — link B/C + cách mở + giới hạn đã biết
- [x] `prototype-feedback-note.md` — **khung sẵn**, 🔴 nội dung chờ phiên tôi facilitate
- [x] `group-feedback-synthesis.md` — **khung sẵn**, 🔴 nội dung chờ đủ note
- [x] `ai-support-log.md` — 12 entry
- [x] `test-script.md` · `session-kit.md` · `dry-run-report.md` · `prototype-build-spec.md` · `day17-input-pack.md` *(thêm)*

### README phải đủ 6 phần
- [x] 1. Thông tin cá nhân và nhóm + **bảng khai báo 3 điểm lệch chuẩn**
- [x] 2. Hypothesis Problem — 5 thành phần, 2 ô 🔴 để nguyên
- [x] 3. Solution Options — bảng so sánh B/C + link prototype
- [x] 4. **Đóng góp của tôi** — Option B · shared context/fixture · Human–AI decisions · facilitation · observation/synthesis · 3 lỗi tự phát hiện
- [x] 5. Prototype Feedback — **đã ghi rõ trạng thái 🔴 chưa chạy test**, kèm bảng 5 giả định viết trước khi test + Still Unproven
- [x] 6. AI Support Log — AI giúp gì, **5 chỗ sai**, chỗ tôi không nhận đề xuất của AI
- [x] Cập nhật **§5** README bằng observation thật

### Soát lần cuối
- [x] Repo đúng tên `Track1_Day18_2A202602942_LuuManhHung`
- [x] Link trong repo đều là **đường dẫn tương đối**, mở được sau khi clone
- [x] Hai prototype cùng user, situation, task, content và desired outcome — cùng `index.html`, cùng `fixture.js`, Màn 3 cùng `renderSaved()`
- [x] **Không chỗ nào tuyên bố "solution đã được validated"** — đã soát `README.md`, `prototype-feedback-note.md`, `group-feedback-synthesis.md`
- [x] Hùng đã test cả B/C với một người ngoài nhóm · ⬜ **chờ Gia Huy**
- [x] Group Synthesis đã tách rõ · ⬜ cột *Pattern* **chờ FB2** — một phiên không tạo ra pattern
- [x] Phần phản ánh cá nhân trong AI Support Log do **chính tôi viết**
- [ ] ⬜ Nếu nộp qua GitHub: push và kiểm repo **mở được với giảng viên/TA**

---

## 7 luật xuyên suốt — soát lại trước khi nộp

1. [x] Giữ **một** Hypothesis Problem cho cả B/C — `three-option-design-sheet.md` §1.3, không bản nào khác
2. [x] **Solution**, không phải phiên bản giao diện — Distance Check §2.5 viết **không dùng một từ nào** về màu/layout/wording
3. [x] Mỗi option một **Human–AI interaction** rõ ràng — B: `Ask → Act` · C: `Act → Ask for confirmation`
4. [x] Prototype **vừa đủ để test** — 3 màn, chỉ Màn 2 khác nhau
5. [x] Tester FB1 đã trải nghiệm **cả hai** option (B → C) · ⬜ FB2 chạy ngược chiều C → B
6. [x] Ghi **hành vi trước**, diễn giải sau — `prototype-feedback-note.md` tách §1 OBSERVED khỏi §2 INTERPRETED, kèm luật *"dòng nào có chữ «vì / có vẻ / chắc là» thì thuộc §2"*
7. [x] **Không tuyên bố validated** — `group-feedback-synthesis.md` §2 chỉ cho ba kết luận: *có dấu hiệu, cần test tiếp* · *có evidence ngược lại* · *phiên test không trả lời được*

---

## Kết luận được phép / không được phép

✅ "Với Hypothesis Problem này, chúng tôi đã thử ba cách giải. Tester đã làm…, vì vậy iteration tiếp theo chúng tôi sẽ…"
❌ "User đã xác nhận solution này đúng."
