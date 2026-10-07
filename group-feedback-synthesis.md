# Group Feedback Synthesis — Double Hờ

**Case:** Case B — AI Notes: Personal Learning Notes
**Hypothesis Problem:** một giả thuyết duy nhất cho cả B và C — `three-option-design-sheet.md` §1.3
**Options:** B — Cùng tổ chức *(Lưu Mạnh Hùng)* · C — Nháp sẵn *(Trần Vũ Gia Huy)*

---

> ## 🟡 MỚI CÓ 1 / 3 FEEDBACK NOTE
>
> **FB1 — Lưu Mạnh Hùng** · tester Dương Quốc Khánh · 05/10/2026 · thứ tự B → C · ✅ đã có → `prototype-feedback-note.md`
> **FB2 — Trần Vũ Gia Huy** · thứ tự C → B · ⬜ **chưa chạy** — đã đối chiếu repo `Track1_Day18_2A202602705_TranVuGiaHuy` ngày 07/10/2026: `prototype-feedback-note.md` và `group-feedback-synthesis.md` bên đó vẫn là **template rỗng** (*"Bổ sung từ phiên test thật"*), chưa có dữ liệu tester nào
> **FB3 — ngoài giờ** · ⬜ chưa chạy
>
> Bảng dưới đã điền **cột FB1**. Hai cột còn lại để trống đúng vì chưa có phiên — **không nhân bản FB1 thành FB2**.
>
> Cột *Pattern hoặc khác biệt* **chưa điền được**: một phiên không tạo ra pattern. Chỉ điền sau khi có FB2.

---

## §0. Khai báo lệch chuẩn — đọc trước khi dùng bảng

| Đề bài yêu cầu | Thực tế nhóm | Hệ quả khi đọc synthesis |
| --- | --- | --- |
| 3 thành viên · 3 options A/B/C | **2 thành viên · 2 options B/C** | Cột *"Option được chọn"* chỉ có 2 lựa chọn; không có hướng **user-led / no-inference** làm đối chứng cho `H_C` → `three-option-design-sheet.md` §2.7 |
| **3 Feedback Notes** | **2** chắc chắn, **3** nếu chạy thêm được 1 tester ngoài giờ | Nếu chỉ có 2 note thì bảng còn 2 cột — **phải ghi rõ**, không nhân bản một phiên thành hai |
| 3 Practice Notes làm evidence Day 17 | **1** (P01 — Tài) | Hypothesis Problem đứng trên một nguồn duy nhất; Barrier và Consequence vẫn là 🔴 giả thuyết |

**Số Feedback Note thật tổng hợp ở đây: `1`** — dưới cả mức tối thiểu của đề bài. Khai báo rõ thay vì làm tròn lên.

---

## §0.1 ⚠️ Rủi ro chưa xử lý — nhóm đang có **hai prototype khác nhau**

Đối chiếu repo của Gia Huy ngày 07/10/2026:

| | Repo Hùng | Repo Gia Huy |
| --- | --- | --- |
| File prototype | `prototype/index.html` · `option-b.html` · `option-c.html` · `shared.css` · `shared.js` · `fixture.js` | `prototype/index.html` · `app.js` · `styles.css` |
| Chọn option | Facilitator đổi bằng `?opt=` trên URL — tester **không thấy** có mấy option | Tester **tự chọn** ở màn hình đầu: *"B — Cùng AI tổ chức"* / *"C — AI tạo bản nháp"* |
| Fixture bài học | Chốt cụ thể: **Prompt Engineering — 4 thành phần**, có mệnh đề đánh đổi cài sẵn ở mục 3 | Vẫn ghi chung chung *"một bài học mẫu"* — chưa chốt nội dung |

**Hệ quả nếu cứ gộp hai Feedback Note:** FB1 và FB2 sẽ nói về **hai sản phẩm khác nhau**, không phải hai lượt test trên cùng một thiết kế. Comparison Contract (`three-option-design-sheet.md` §2.1) chỉ ràng buộc trong từng build, không ràng buộc giữa hai build.

Thêm nữa, prototype của Gia Huy **cho tester tự chọn option** — tức tester biết mình đang so sánh hai phương án. Đây là một **biến khác** so với FB1, nơi tester chỉ thấy một sản phẩm.

### Nhóm phải chọn một trong hai, trước khi Gia Huy chạy phiên

| Hướng | Việc phải làm | Đánh đổi |
| --- | --- | --- |
| **A — Thống nhất một build** | Gia Huy chạy phiên trên build trong repo này, mở bằng `?opt=c&fresh=1` *(thứ tự C → B)* | FB1 và FB2 so sánh được; đổi lại Gia Huy không test trên bản mình viết |
| **B — Giữ hai build** | Vẫn chạy, nhưng synthesis **không được gộp** thành pattern — chỉ đặt cạnh nhau và ghi rõ là hai sản phẩm khác nhau | Giữ công sức hai bên, nhưng **mất khả năng rút pattern** — đúng thứ GATE 5 yêu cầu |

### ✅ Nhóm chốt **hướng A** — 07/10/2026

Cả hai phiên chạy trên **một build duy nhất**: `prototype/` trong repo `Track1_Day18_2A202602942_LuuManhHung`.

| | |
| --- | --- |
| **Gia Huy mở** | `prototype/index.html?opt=c&fresh=1` → sau lượt C, bấm *"Bắt đầu lại"*, đổi URL sang `?opt=b` → lượt B |
| **Thứ tự** | **C → B** — ngược chiều FB1, để tách *tác dụng của option* khỏi *tác dụng của việc gặp trước* |
| **Script** | `test-script.md` · cue card `session-kit.md` §B · bản ghi tay §C |
| **Lưu ý từ FB1** | Tester hỏi *"giải thích giúp mình"* thì **không giải thích** — hỏi lại *"Theo bạn, nó nên hoạt động như thế nào?"*. Ở FB1 facilitator đã lỡ giải thích và dữ liệu sau đó bị nhiễu |

**Hệ quả cho bản prototype riêng của Gia Huy** *(`prototype/` trong repo của bạn ấy)*: giữ lại như artifact thiết kế Option C, **không dùng để test**. Khai báo trong README của bạn ấy để không ai tưởng là hai lần test cùng một thứ.

**Hệ quả cho fixture:** build chung đã chốt *Prompt Engineering — 4 thành phần*, nên cờ ⚠️ *"chưa chốt fixture"* ở `ai-support-log.md` Entry 05/06 **được giải toả bằng chính quyết định này**.

---

## §1. Bảng 5 dòng × từng feedback + cột Pattern / khác biệt

| | **FB1** — phiên Hùng<br>Dương Quốc Khánh · B → C | **FB2** — phiên Gia Huy<br>C → B | **FB3** — ngoài giờ | **Pattern hoặc khác biệt** |
| --- | --- | --- | --- | --- |
| **First action** | Bấm thẳng *"Hoàn thành bài học"* ở **cả hai lượt**; đọc lướt bài ~1 phút; tự đánh dấu, có đánh dấu ở mục 3 | ⬜ | ⬜ | ⬜ chờ FB2 |
| **Breakdown chính** | **Dừng 3′ ở B và 2′ ở C ngay khi vào màn Sổ ghi chú**, rồi hỏi *"Bạn có thể giải thích tính năng của màn hình này không?"* | ⬜ | ⬜ | ⬜ chờ FB2 |
| **Cách lấy lại control** | Thấy và thử *"Tự viết, không cần AI"*; sửa nội dung AI tạo ra; **tìm nút "Bắt đầu lại" khá khó khăn** | ⬜ | ⬜ | ⬜ chờ FB2 |
| **Option được chọn** | **B — Cùng tổ chức**. *"cách đánh dấu và note, duyệt qua từng note trực quan và dễ hiểu hơn"* | ⬜ | ⬜ | ⬜ chờ FB2 |
| **Trade-off tự nói ra** | *"Cách thoát khỏi màn hình ghi chú chưa có, tester chưa biết cách thoát như thế nào."* | ⬜ | ⬜ | ⬜ chờ FB2 |

### Số đo đáng chú ý từ FB1

| | Option B | Option C |
| --- | --- | --- |
| Giây từ lúc thấy kết quả AI → bấm Lưu | **3 giây** | **3 giây** |
| Dừng ở khối gắn nhãn ⚠ | không | không |
| Mệnh đề đánh đổi ở mục 3 còn trong note cuối | **còn** | **mất** |
| Tester **tự** bắt được dòng 3 sai *(trước khi được giải thích)* | **có** | **có** |
| Số câu hỏi làm rõ của B | **0** | — |

### Cách điền cột cuối — đúng một trong ba nhãn

| Nhãn | Dùng khi | Ví dụ cách viết |
| --- | --- | --- |
| **Pattern** | ≥ 2 tester làm **cùng một hành vi** | *"2/2 tester đều …"* |
| **Khác biệt** | Các tester làm **ngược nhau** | *"FB1 … còn FB2 thì ngược lại …"* |
| **Chỉ 1 lần** | Chỉ xuất hiện ở một phiên | *"chỉ FB2, chưa đủ gọi là pattern"* |

❌ Không viết *"đa số tester thích B"*. ❌ Không ghi tỉ lệ phần trăm trên 2–3 phiên.

### Kiểm tra order effect

Thứ tự B → C và C → B được chia cố ý để tách *tác dụng của option* khỏi *tác dụng của việc gặp trước*.

| Câu hỏi | Trả lời sau khi có note |
| --- | --- |
| Tester có xu hướng chọn option **gặp sau** không? | |
| Có hành vi nào chỉ xuất hiện ở **lượt hai** (khi đã quen màn hình)? | |
| Nếu có → ảnh hưởng gì tới cách đọc dòng *"Option được chọn"*? | |

---

## §2. Bốn giả định của Chặng 3 — đối chiếu với quan sát thật

| # | Giả định *(§3.4)* | Quan sát thật đã nói gì | Kết luận được phép |
| --- | --- | --- | --- |
| 1 | Câu hỏi làm rõ + đề xuất nhóm của **B** **hỗ trợ** hay **làm ngắt mạch** tổng hợp | FB1: **B hỏi 0 câu** — bước *Ask* không xuất hiện với bộ dấu vết tester tạo | **phiên test không trả lời được** |
| 2 | Người dùng **C** **thật sự kiểm tra nguồn** hay **chỉ xác nhận** bản nháp | FB1: có mở link nguồn, nhưng **3 giây** sau đã bấm Lưu và **không dừng ở khối ⚠**. Cùng con số ở B | **có evidence ngược lại** — 1 phiên |
| 3 | Cả hai cách có **giữ đủ ngữ cảnh** *(mệnh đề đánh đổi ở mục 3)* | FB1: **B giữ được, C mất**. Đáng chú ý: tester **tự phát hiện** dòng 3 sai, trước khi facilitator giải thích — nhưng note cuối của C **vẫn mất** mệnh đề. **Bắt được lỗi không đồng nghĩa với sửa được lỗi** | **có dấu hiệu, cần test tiếp** |
| 4 | Tự tổng hợp là **pain** cần giảm hay **hoạt động học cần bảo toàn** | FB1 nói: *"Muốn tự đánh dấu các phần nội dung chưa hiểu, AI sẽ tổng hợp lại theo cấu trúc"* — là **lời nói**, không phải hành vi quan sát được | **có dấu hiệu, cần test tiếp** |
| 5 | *(§1.3)* Learner có coi **"hết bài học"** là lúc muốn ghi chú | FB1: thao tác đầu tiên ở **cả hai lượt** là bấm *"Hoàn thành bài học"* | **có dấu hiệu, cần test tiếp** |

### Phát hiện ngoài bảng giả định — nặng nhất của FB1

Tester **dừng 3 phút ở B và 2 phút ở C** ngay khi vào màn Sổ ghi chú, rồi hỏi *"Bạn có thể giải thích tính năng của màn hình này không?"* — và facilitator **đã giải thích**.

| Hệ quả | |
| --- | --- |
| **GATE 4 trượt** | Tiêu chí *"không cần facilitator narrate mới hiểu"* không đạt — ở **cả hai** option |
| **Dữ liệu sau đó bị nhiễm** | Mọi quan sát sau thời điểm giải thích không còn độc lập, kể cả ô *"có bắt được dòng 3"* |
| **Áp dụng cho FB2** | Gia Huy chạy phiên của mình: tester hỏi thì **hỏi lại** *"Theo bạn, nó nên hoạt động như thế nào?"*, **không giải thích** |
| **Phần không bị nhiễm** | Việc tester bắt được dòng 3 xảy ra **trước** lúc giải thích → quan sát đó vẫn dùng được |

> Cột *"Kết luận được phép"* chỉ nhận một trong ba: **"có dấu hiệu, cần test tiếp"** · **"có evidence ngược lại"** · **"phiên test không trả lời được"**.
> **Không** nhận *"đã xác nhận"* hay *"đã validated"*.

---

## §3. Một Next Change của nhóm

> ⚠️ **Chưa chốt được Next Change của nhóm** — mới có 1/3 Feedback Note. Dưới đây là **đề xuất từ FB1**, chờ FB2 để xác nhận hoặc đổi.

Hướng đang nghiêng về:

- [x] **Sửa cả hai option** rồi test người tiếp theo
- [ ] Giữ 1 option, sửa interaction
- [ ] Kết hợp 2 option
- [ ] Bỏ 1 option

| Trường | Nội dung |
| --- | --- |
| **Next Change đề xuất** | Màn Sổ ghi chú của **cả 2B và 2C** phải có **một dòng nói rõ màn này làm gì** và **một nút thoát hiện rõ ở vị trí cố định** |
| **Evidence dẫn tới** | FB1 §1.2 — dừng 3′/2′ rồi hỏi *"giải thích giúp mình"* ở **cả hai** option · FB1 §1.5 — *"Cách thoát khỏi màn hình ghi chú chưa có"* · FB1 §1.4 — tìm nút *Bắt đầu lại* khó khăn. Cả ba đều là dòng **OBSERVED**, không phải diễn giải |
| **Đã cân nhắc rồi bỏ** | *Sửa cơ chế hỏi của B để bước Ask luôn xuất hiện* — bỏ, vì FB1 **không kiểm được** giả định 1 (B hỏi 0 câu), nên chưa có cơ sở. Xem `dry-run-report.md` §4 |
| **Không thay đổi ở iteration này** | Cơ chế `Ask → Act` của B · `Act → Ask for confirmation` của C · fixture bài học và chỗ cài lỗi ở mục 3 |

> Next Change phải truy được về một dòng **OBSERVED** trong ít nhất một Feedback Note. Nếu chỉ truy về phần INTERPRETED thì ghi rõ điều đó.

---

## §4. Still Unproven — sau tất cả feedback

| # | Vẫn chưa biết | Vì sao đợt test này không trả lời được | Cần gì để trả lời |
| --- | --- | --- | --- |
| 1 | **Có pattern hay không** | Mới 1 phiên. Một tester không tạo ra pattern | FB2 của Gia Huy, thứ tự C → B |
| 2 | B **hỗ trợ hay làm ngắt mạch** tổng hợp | B hỏi 0 câu làm rõ với bộ dấu vết tester tạo ra | Tester đánh dấu kiểu khác, hoặc chạy thêm phiên |
| 3 | Tester có **tự** bắt được dòng 3 không | Facilitator đã giải thích màn hình giữa phiên → quan sát sau đó không độc lập | Phiên có kỷ luật facilitation, không narrate |
| 4 | B được chọn vì **cơ chế** hay vì **gặp trước** | Chỉ một phiên, thứ tự B → C | FB2 chạy ngược chiều C → B |
| 5 | Cách này có giúp **tìm lại** kiến thức về sau không | Tester **không có relevant context**; phiên 10 phút | Tester có trải nghiệm thật, và một thiết kế đo được việc dùng lại |

**Những điều biết chắc là vẫn chưa chứng minh được, bất kể kết quả test:**

- **Barrier** và **Consequence** của Hypothesis Problem vẫn 🔴 **giả thuyết, không evidence** — Chặng 6 không đo được chúng
- `H_C` **không có đối chứng** — cả B và C đều có AI sinh nội dung, thiếu hướng user-led
- Chất lượng **AI thật** chưa đo được — output trong prototype là **canned, cố định**
- Hành vi **tìm lại note một tháng sau** chưa đo được — phiên test chỉ dài 20 phút
- Giả định **chuyển bối cảnh** từ *research tự do với AI* (evidence P01) sang *bài học có cấu trúc trên VLearn* — xem `three-option-design-sheet.md` §1.3

---

## Soát lại trước khi coi là xong

- [x] Số note thật được khai báo đúng: **1**, không làm tròn lên
- [x] Mỗi ô FB1 truy được về một dòng OBSERVED trong `prototype-feedback-note.md`
- [x] **Không** gọi bất cứ thứ gì là "pattern" khi mới có một phiên
- [x] Next Change ghi rõ là **đề xuất**, chưa chốt
- [x] §4 có nội dung thật
- [x] **Không chỗ nào** viết *"solution đã được validated"* hay áp ngưỡng thống kê
- [ ] ⬜ Chạy FB2 → điền cột 2 → điền cột *Pattern hoặc khác biệt* → chốt Next Change
