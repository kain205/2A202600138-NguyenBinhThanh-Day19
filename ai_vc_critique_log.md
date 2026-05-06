# AI VC Critique Log — Synapsy
> Persona: Partner, Sequoia Capital. 50 AI pitches this week. Tired.
> Date: 2026-05-06

---

## PHẦN 1 — PITCH GỐC TRƯỚC CRITIQUE

### Twitter Pitch (v1)
> Bọn em là **Synapsy**. Bọn em giúp **sinh viên Y khoa VN đang nước rút trước kỳ thi** giải quyết việc **không biết học gì trước và mất hàng giờ tự làm tài liệu ôn tập** bằng **AI chẩn đoán lỗ hổng kiến thức từ tài liệu của chính sinh viên rồi tạo lộ trình ôn thi cho tối nay — kèm flashcard tự động và truy xuất nguồn từng dòng file gốc**.
>
> Chưa launch. Vòng tròn bạn bè ban đầu: **100% nghe xong muốn thử ngay**. Thị trường: ~**60–90K sinh viên Y** đang học tại 15 trường Y trên cả nước.
>
> Gọi **[Số tiền] pre-seed** để ra MVP và đạt **50 user hoàn thành ôn 50+ thẻ trong 48h sau upload đầu tiên** trong vòng 3 tháng.

### Pitch Memo v1 (tóm tắt)
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

Câu mở đầu là một câu chạy dài cố nhồi 6 ý vào cùng một hơi thở: Pain 1, Pain 2, Solution, Feature 1, Feature 2, Feature 3. Sau 8 giây tôi không nhớ bạn làm gì. Tôi nhớ bạn làm *nhiều thứ*.

**Quy tắc:** Câu đầu tiên phải làm một việc — khiến tôi hỏi "ủa, bằng cách nào?" Bạn đang pitching một feature list, không phải một insight.

---

### 2. THE INSIGHT TEST
**Insight nào thực sự không hiển nhiên?**

**Insight A — "Bottleneck là không biết lỗ hổng của mình"** → REJECT. Hiển nhiên. Mọi adaptive learning platform từ 2010 đều claim cái này.

**Insight B — "Sinh viên Y khoa có zero-tolerance với hallucination — rào cản adoption là tâm lý, không phải kỹ thuật. Source traceability giải quyết niềm tin, không phải accuracy"** → ACCEPT. Non-obvious behavioral insight. Đứng vững.

Vấn đề: Insight B bị chôn vùi như một bullet point feature thay vì làm lede của pitch.

---

### 3. THE OPENAI THREAT
**Nếu OpenAI ship tính năng này tuần tới, moat của bạn là gì?**

ChatGPT Projects đã làm được: upload PDF → quiz → study suggestions. Với pitch v1, không có câu trả lời rõ ràng.

Moat candidates thật:
| Moat | Độ mạnh | Có trong pitch v1? |
|---|---|---|
| SRS data tích lũy — switching cost tăng theo thời gian | Mạnh | Không |
| Vietnamese medical exam format specificity (OSCE...) | Mạnh nếu thật | Không |
| Source traceability UX | Yếu dài hạn | Có, framed sai |

---

### 4. THE NUMBERS TEST

**"100% bạn bè muốn thử ngay"** — Mom Test failure. "Muốn thử" ≠ sẽ dùng ≠ sẽ trả tiền. Không phải signal.

**"60–90K sinh viên Y"** — TAM quá nhỏ nếu không có expansion story. TAM thực: 2M+ sinh viên đại học VN.

**"$1B → $3B EdTech VN"** — Entire market, không phải addressable market. Gạch ngay trong 30 giây.

**"50 users / 50 thẻ / 48h"** — Đây là target, không phải traction. Trình bày cạnh traction làm loãng.

---

### 5. THE WEAKEST LINE

**Câu push back mạnh nhất:**
> ~~"Vòng tròn bạn bè ban đầu: 100% người được nghe mô tả sản phẩm muốn thử ngay — early demand signal trước cả khi có MVP."~~

Tự gán nhãn "early demand signal" cho phản ứng bạn bè signal founder chưa hiểu sự khác biệt giữa social validation và market validation. Mọi pitch tuần này đều có câu này.

**Rewrite:**
> "Chưa có traction số. Đang trong tuần đầu structured customer discovery — lịch phỏng vấn 10 sinh viên Y năm 3–5, hoàn thành trong 2 tuần. Số thật sẽ có trước khi ký term sheet."

---

## PHẦN 3 — QUYẾT ĐỊNH + FOUNDER ANSWERS

| Điểm | Quyết định VC | Founder Answer | Status |
|---|---|---|---|
| Câu mở 8 giây — run-on | REJECT | Rewrite: lead bằng clear pain ("ôn thi không biết bắt đầu từ đâu") thay vì trust gap — founder decision: user resonance > VC cleverness | ✅ Fixed |
| Insight A — "không biết lỗ hổng" | REJECT | Removed as primary insight | ✅ Fixed |
| Insight B — trust gap / source traceability | ACCEPT | Promoted to lede | ✅ Fixed |
| OpenAI moat — SRS data flywheel | PARTIAL → cần confirm | **Confirmed: data flywheel là moat chính. Càng dùng, SRS data tích lũy, lộ trình càng cá nhân hóa.** | ✅ Fixed |
| TAM 60–90K quá nhỏ | PARTIAL → cần expansion story | **Expansion: med students là beachhead → 2M+ sinh viên đại học VN** | ✅ Fixed |
| TAM stat $1B–$3B EdTech | REJECT | Removed | ✅ Fixed |
| Traction "bạn bè 100%" | REJECT | Replaced bằng structured customer discovery | ✅ Fixed |
| PMF target 50/50/48h | ACCEPT | Giữ nguyên, tách khỏi traction section | ✅ Fixed |
| Solo founder — red flag | FLAG | **Plan C: solo đủ để prove MVP, tìm co-founder sau PMF signal đầu tiên. Tránh dilute equity trước proof.** | ✅ Addressed |
| Raise amount | BLOCKER | Chưa xác định — infra-only raise, founder không cần living expenses | ⚠️ Còn [Số tiền] |

---

## PHẦN 4 — PITCH FINAL ĐÃ SỬA

### Twitter Pitch (v2)

Bọn em là **Synapsy**. Bọn em giúp **sinh viên Y khoa VN** giải quyết việc **ôn thi không biết bắt đầu từ đâu** bằng **hệ thống chẩn đoán lỗ hổng kiến thức từ tài liệu của chính sinh viên — tạo lộ trình học cho tối nay, tự động sinh flashcard, mỗi thẻ trỏ thẳng tới dòng PDF gốc để dám tin vào AI. Càng dùng, hệ thống càng biết bạn cần học gì.**

Chưa launch. Structured customer discovery đang chạy: 10 sinh viên Y năm 3–5 trong lịch phỏng vấn 2 tuần tới. Beachhead: 60–90K sinh viên Y; expansion: 2M+ sinh viên đại học VN.

Gọi **[Số tiền] pre-seed** để ra MVP và đạt **50 users ôn 50+ thẻ trong 48h** — PMF signal duy nhất mình đo.

---

### Pitch Memo (v2 — xem pitch_memo.md)

*(File pitch_memo.md đã được cập nhật với toàn bộ thay đổi từ critique session này.)*

---

*Log tạo bởi AI VC critique session — 2026-05-06*
*Cập nhật lần cuối: 2026-05-06 sau founder Q&A*
