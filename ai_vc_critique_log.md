# AI VC Critique Log — Synapsy
> Persona: Partner, Sequoia Capital. 50 AI pitches this week. Tired.
> Date: 2026-05-06

---

## PHẦN 1 — PITCH GỐC TRƯỚC CRITIQUE

### Twitter Pitch
> Bọn em là **Synapsy**. Bọn em giúp **sinh viên Y khoa VN đang nước rút trước kỳ thi** giải quyết việc **không biết học gì trước và mất hàng giờ tự làm tài liệu ôn tập** bằng **AI chẩn đoán lỗ hổng kiến thức từ tài liệu của chính sinh viên rồi tạo lộ trình ôn thi cho tối nay — kèm flashcard tự động và truy xuất nguồn từng dòng file gốc**.
>
> Chưa launch. Vòng tròn bạn bè ban đầu: **100% nghe xong muốn thử ngay**. Thị trường: ~**60–90K sinh viên Y** đang học tại 15 trường Y trên cả nước.
>
> Gọi **[Số tiền] pre-seed** để ra MVP và đạt **50 user hoàn thành ôn 50+ thẻ trong 48h sau upload đầu tiên** trong vòng 3 tháng.

### Pitch Memo (tóm tắt)
- **Problem**: (1) Không biết học gì trước. (2) Mất 3–5h tự làm flashcard thủ công.
- **Insight**: Bottleneck là không biết lỗ hổng của mình + nỗi sợ AI hallucination trong bối cảnh lâm sàng.
- **Solution**: Upload → Diagnostic Quiz → Lộ trình tối nay → Auto Flashcard (SRS) + Source Traceability + Sandboxed Chatbot.
- **Why Now**: LLM đủ mạnh, EdTech VN $1B→$3B, 60–90K sinh viên Y, 200+ startup chưa ai lấp gap này.
- **Traction**: Bạn bè 100% muốn thử. [X] phỏng vấn. PMF target: 50 users / 50 thẻ / 48h.
- **Ask**: [Số tiền] pre-seed để ra MVP + validate PMF.

---

## PHẦN 2 — FEEDBACK CỦA AI VC (SEQUOIA PARTNER)

*Tôi đã nghe 50 pitch AI tuần này. Đây là đánh giá thẳng thắn.*

---

### 1. THE 8-SECOND TEST
**Câu đầu tiên có giúp tôi muốn nghe thêm 50 giây không?**

**Không.**

Câu mở đầu của bạn là một câu chạy dài cố nhồi 6 ý vào cùng một hơi thở:
- Pain 1: không biết học gì
- Pain 2: mất hàng giờ làm tài liệu
- Solution: AI chẩn đoán
- Feature: lộ trình tối nay
- Feature: flashcard tự động
- Feature: truy xuất nguồn

Sau 8 giây tôi không nhớ bạn làm gì. Tôi nhớ bạn làm *nhiều thứ*.

**Quy tắc:** Câu đầu tiên phải làm một việc — khiến tôi hỏi "ủa, bằng cách nào?" hoặc "ô, họ giải quyết được cái đó à?" Bạn đang pitching một feature list, không phải một insight.

**Rewrite câu mở:**
> "Synapsy là app đầu tiên biết sinh viên Y khoa chưa biết gì — trước khi họ tự biết."

Một câu. Một ý. Và nó buộc tôi phải hỏi tiếp.

---

### 2. THE INSIGHT TEST
**Insight nào thực sự không hiển nhiên?**

Bạn đưa ra hai insight trong pitch memo:

**Insight A — "Bottleneck là không biết lỗ hổng của mình, không phải thiếu nỗ lực"**
→ **REJECT. Đây là insight hiển nhiên.** Khan Academy, Coursera, Duolingo, mọi adaptive learning platform từ 2010 đến nay đều claim cái này. Tuần này tôi đã nghe câu này 7 lần từ 7 founder khác nhau.

**Insight B — "Sinh viên Y khoa có zero-tolerance với AI hallucination trong bối cảnh lâm sàng — rào cản adoption không phải kỹ thuật mà là tâm lý. Source traceability giải quyết niềm tin, không phải accuracy"**
→ **ACCEPT. Đây mới là insight thực sự không hiển nhiên.** Hầu hết AI edtech đang chạy theo "accuracy cao hơn." Bạn nhận ra rằng với sinh viên Y khoa, *cảm giác có thể kiểm chứng* quan trọng hơn *accuracy thật*. Đây là behavioral insight về tâm lý người dùng, không phải technical insight. Nó đứng vững.

**Vấn đề:** Insight B bị chôn vùi ở phần "Differentiators" như một bullet point feature. Nó phải là câu đầu tiên của pitch.

---

### 3. THE OPENAI THREAT
**Nếu OpenAI ship tính năng này tuần tới, moat của bạn là gì?**

ChatGPT Projects hiện tại đã làm được: upload PDF → hỏi đáp → tạo quiz → gợi ý học gì. Nếu OpenAI thêm "study plan generator" vào GPT-4o next week — và họ sẽ làm — pitch của bạn có đứng vững không?

Câu trả lời trung thực: **Với pitch hiện tại, không.**

Bạn có 3 moat candidates tiềm năng, nhưng không cái nào được claim rõ trong pitch:

| Moat Candidate | Độ mạnh | Có trong pitch không? |
|---|---|---|
| SRS data tích lũy theo thời gian — càng dùng càng cá nhân hóa, switching cost tăng | Trung bình | Không |
| Tích hợp sâu định dạng thi VN (OSCE, thi quốc gia) — OpenAI không biết format này | Mạnh nếu thật | Không |
| Network effect: sinh viên cùng trường/cùng môn share deck → cold start được xử lý | Mạnh | Không |
| Source traceability UX — OpenAI có thể copy, nhưng bạn có thể đi trước 12 tháng | Yếu dài hạn | Có, nhưng framed sai |

**Tôi buộc bạn phải trả lời:** SRS progress data của người dùng có được lưu lại để cá nhân hóa theo thời gian không, hay mỗi session là fresh start? Nếu không có persistence, bạn không có switching cost và không có moat.

---

### 4. THE NUMBERS TEST
**Các con số có defensible không?**

**"100% bạn bè muốn thử ngay"**
Đây là Mom Test failure kinh điển. Tôi push back ngay:
- "Bạn bè" là bao nhiêu người? 3? 5? 10?
- Họ có phải sinh viên Y khoa đang trong giai đoạn nước rút không, hay chỉ là người quen thấy ý tưởng hay?
- "Muốn thử" có nghĩa là gì? Họ có để lại email, ký beta agreement, hay chỉ nói "ừ hay đó"?
- "Muốn thử" ≠ sẽ dùng ≠ sẽ trả tiền.

Gọi đây là "early demand signal" là tự label một thứ không phải signal. Mọi founder đều có cái này.

**"60–90K sinh viên Y — thị trường"**
TAM thật của bạn: 60–90K users × price point (bạn chưa nói) = ?
Nếu charge 100k VND/tháng (~$4): ARR tối đa ở 10% penetration = ~$2.4M–$3.6M.
Với Sequoia thì không đủ scale. Bạn cần hoặc: (a) mở rộng sang tất cả sinh viên đại học VN ôn thi (2M+), hoặc (b) expansion ra Đông Nam Á, hoặc (c) B2B — bán cho các trường Y.

**"$1B → $3B EdTech VN CAGR 13%"**
Con số này là entire EdTech VN market, không phải addressable market của bạn. Đây là kiểu stat làm đẹp slide nhưng sẽ bị partner bất kỳ gạch ngay trong 30 giây. Đừng dùng.

**"50 users / 50 thẻ / 48h"**
Đây là PMF *target*, không phải traction. Đừng trình bày nó cạnh traction. Nó làm loãng những gì bạn thực sự đã có.

---

### 5. THE WEAKEST LINE

**Câu tôi push back mạnh nhất:**

> *"Vòng tròn bạn bè ban đầu: 100% người được nghe mô tả sản phẩm muốn thử ngay — early demand signal trước cả khi có MVP."*

**Tại sao đây là câu nguy hiểm nhất trong pitch:**
Nó không chỉ yếu — nó signal cho investor rằng founder chưa hiểu sự khác biệt giữa social validation và market validation. Tôi thấy câu này (hoặc biến thể của nó) trong ít nhất 40 trong 50 pitch tuần này. Và 100% trong số đó chưa có paying customer.

Thêm vào đó, tự gán nhãn "early demand signal" cho phản ứng của bạn bè cho thấy bạn đang cố thuyết phục *mình* nhiều hơn thuyết phục *tôi*.

**Rewrite:**

Thay vì:
> ~~"Vòng tròn bạn bè ban đầu: 100% nghe xong muốn thử ngay — early demand signal trước cả khi có MVP."~~

Viết:
> "Chưa có traction số. Đang trong tuần đầu của structured customer discovery — lịch phỏng vấn với 10 sinh viên Y năm 3–5, mục tiêu hoàn thành trong 2 tuần. Số thật sẽ có trước khi ký term sheet."

Ngắn hơn. Trung thực hơn. Và paradoxically — đáng tin hơn.

---

## PHẦN 3 — QUYẾT ĐỊNH ACCEPT / REJECT / PARTIAL

| Điểm | Quyết định | Lý do |
|---|---|---|
| 8-second test — câu mở | **REJECT** | Run-on, 6 ý trong 1 câu, không có hook |
| Insight A — "không biết lỗ hổng" | **REJECT** | Hiển nhiên, mọi adaptive learning claim |
| Insight B — trust gap / source traceability | **ACCEPT** | Non-obvious behavioral insight, specific to med students |
| OpenAI moat — hiện tại | **PARTIAL** | SRS data + VN exam format là moat tiềm năng nhưng chưa được claim |
| Số thị trường 60–90K | **PARTIAL** | Số đúng nhưng TAM quá nhỏ cho VC nếu không có expansion story |
| Số EdTech $1B–$3B | **REJECT** | Misleading, không phải addressable market của bạn |
| Traction "bạn bè 100%" | **REJECT** | Mom test failure, không phải signal |
| PMF target 50/50/48h | **ACCEPT** | Actionable và cụ thể — nhưng phải tách khỏi traction section |
| Insight B làm lede của pitch | **ACCEPT** | Nếu lead bằng insight B thay vì feature list, pitch mạnh hơn nhiều |

**Verdict tổng thể:** Không đủ để term sheet ngay. Nhưng có **một insight thật** (trust gap) và **một PMF metric thật** (50/50/48h) — hai thứ này đủ để tôi muốn gặp lại sau 2 tuần khi có số phỏng vấn thực tế.

---

## PHẦN 4 — PITCH FINAL ĐÃ SỬA

### Twitter Pitch (rewritten)

Bọn em là **Synapsy**. Bọn em giúp **sinh viên Y khoa VN** giải quyết việc **không thể tin vào AI để ôn thi lâm sàng vì sợ hallucination** bằng **hệ thống chẩn đoán lỗ hổng từ tài liệu của chính sinh viên — mỗi flashcard trỏ thẳng tới dòng PDF gốc, không phải kiến thức AI tự bịa**.

Chưa launch. Structured customer discovery đang chạy: 10 sinh viên Y năm 3–5 trong lịch phỏng vấn 2 tuần tới. Thị trường ban đầu: 60–90K sinh viên Y; expansion path: 2M+ sinh viên đại học VN.

Gọi **[Số tiền] pre-seed** để ra MVP và đạt **50 users ôn 50+ thẻ trong 48h** — PMF signal duy nhất mình đo.

---

### Pitch Memo (rewritten — 6 sections)

---

**Problem**

Sinh viên Y khoa VN không thể dùng AI để ôn thi. Không phải vì AI không đủ thông minh — mà vì liều thuốc sai trong một thẻ flashcard có thể hủy hoại niềm tin vào toàn bộ bộ thẻ. Kết quả: họ vẫn đang mất 3–5h/ngày tự tạo flashcard thủ công trên Anki, và vào mùa thi họ không biết ưu tiên ôn gì trước.

---

**Insight**

Với sinh viên Y khoa, rào cản adoption AI không phải accuracy — mà là *khả năng kiểm chứng*. Họ cần biết AI lấy thông tin đó từ đâu, không phải AI có đúng không. Source traceability giải quyết tâm lý, không phải kỹ thuật. Đây là insight mà tất cả các edtech AI đang bỏ qua.

Và một khi rào cản niềm tin được phá vỡ, hành vi học tập tích cực mở ra hoàn toàn.

---

**Solution**

Synapsy: upload slide PDF → AI chẩn đoán lỗ hổng → tạo lộ trình học cho tối nay → auto flashcard với SRS.

Differentiator duy nhất quan trọng: **mỗi flashcard trỏ thẳng tới trang và dòng trong file gốc của chính sinh viên.** Bấm "Xem nguồn" → màn hình chia đôi, highlight đúng dòng. Không phải feature — đây là cơ chế phá vỡ rào cản tâm lý.

Chatbot sandboxed: hỏi đào sâu một thẻ bất kỳ, AI chỉ dùng file đã upload. Không có hallucination ngoài luồng.

---

**Why Now**

LLM đã đủ tốt để parse tài liệu y khoa tiếng Việt phức tạp. Sinh viên Y thế hệ mới đang dùng ChatGPT — nhưng không có source control. Gap giữa "đang dùng ChatGPT để ôn thi" và "có thể thực sự tin tưởng AI với kiến thức lâm sàng" là khoảng trắng Synapsy lấp.

Áp lực thi ngành Y tại VN đang tăng (OSCE, thi quốc gia) trong khi không có công cụ nào được thiết kế riêng cho context này.

---

**Traction**

Chưa có số. Đang trong tuần đầu structured customer discovery với 10 sinh viên Y năm 3–5. Số thật — pain confirmation rate, willingness to pay, beta commitment — sẽ có trước khi ký bất kỳ term sheet nào.

PMF Signal target duy nhất: **50 users hoàn thành ôn 50+ thẻ trong 48h kể từ lần upload đầu tiên.** Nếu không đạt số này, chúng em pivot trước khi scale.

---

**Ask**

**[Số tiền] VND pre-seed** — dùng cho:
- Engineering: 2 dev × [X] tháng → ra MVP đủ để test PMF signal
- Cloud infra: OpenAI API + MinerU parsing pipeline
- Customer acquisition: 50 beta users có structured onboarding

Milestone duy nhất quan trọng sau vòng này: **50 users / 50 thẻ / 48h**. Đó là số chứng minh người dùng thực sự học — không phải chỉ đăng ký rồi bỏ.

---

*Log tạo bởi AI VC critique session — 2026-05-06*
