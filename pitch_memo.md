# Pitch Memo — Synapsy
> 1-pager | Pre-launch | 2026

---

## Problem

Sinh viên Y khoa VN trong giai đoạn nước rút (1–3 tuần trước kỳ thi) đối mặt với hai vấn đề song song:

1. **Không biết học gì trước.** Với hàng trăm trang slide mỗi môn, họ không có cách nào xác định lỗ hổng kiến thức của bản thân — nên học dàn trải, hoặc học lại những gì đã biết.
2. **Mất hàng giờ chuẩn bị tài liệu trước khi học.** Tự tạo flashcard thủ công trên Anki/Quizlet từ slide PDF tốn 3–5h — họ kiệt sức ở khâu chuẩn bị, chưa kịp bước vào khâu học thuộc.

Kết quả: hoảng loạn sát thi, hiệu suất ôn tập thấp, rủi ro cao với các môn lâm sàng có zero-tolerance về kiến thức sai.

---

## Insight

Điểm nghẽn **không phải** là thiếu nỗ lực — mà là thiếu một hệ thống biết *cái gì sinh viên chưa biết* và *nên học cái đó theo thứ tự nào tối nay*.

Và với sinh viên Y khoa, rào cản dùng AI không phải năng lực kỹ thuật — mà là **nỗi sợ AI bịa kiến thức lâm sàng** (hallucination) trong bối cảnh high-stakes. Giải quyết niềm tin = mở khóa hành vi dùng sản phẩm.

---

## Solution

**Synapsy** là app ôn thi cho sinh viên Y khoa. Luồng cốt lõi:

1. **Upload tài liệu** (PDF slide bài giảng, ghi chú) — AI parse ra structured content.
2. **Diagnostic Quiz** — Hệ thống tự tạo bộ câu hỏi chẩn đoán, xác định chính xác lỗ hổng kiến thức của từng sinh viên.
3. **Lộ trình ôn thi cá nhân hóa cho tối nay** — AI ưu tiên nội dung cần học ngay dựa trên kết quả diagnostic, thời gian còn lại, và lịch thi.
4. **Tự động tạo Flashcard** (Concept Cards) — Trích xuất cặp Q&A trọng tâm, hỗ trợ SRS (Spaced Repetition / SM-2) để ôn dài hạn.

**Differentiators:**
- **Truy xuất nguồn 1-chạm**: Mỗi flashcard gắn tag trực tiếp tới trang và dòng trong file gốc — sinh viên bấm "Xem nguồn", màn hình chia đôi highlight đúng dòng PDF. Giải quyết nỗi sợ hallucination.
- **Chatbot sandbox**: Chat đào sâu một thẻ bất kỳ, AI chỉ trả lời dựa trên file đã upload — không dùng kiến thức ngoài internet.

---

## Why Now

- **LLM đủ mạnh**: Mô hình ngôn ngữ lớn đã đạt ngưỡng xử lý tài liệu y khoa tiếng Việt có cấu trúc phức tạp (bảng, sơ đồ, thuật ngữ lâm sàng) với độ chính xác đủ để deploy sản phẩm.
- **Thị trường EdTech VN đang bùng nổ**: ~$1 tỷ USD (2024), dự kiến $3 tỷ USD vào 2033 — CAGR 13%. 200+ EdTech startup đang hoạt động, nhưng chưa ai lấp gap riêng cho sinh viên Y khoa.
- **Addressable market rõ ràng**: ~60,000–90,000 sinh viên Y đang học tại 15 trường Y trên cả nước, trong tổng số 2 triệu+ sinh viên đại học VN (2024).
- **Hành vi AI-native nhưng thiếu kiểm soát**: Sinh viên Y thế hệ mới đang dùng ChatGPT để ôn thi — nhưng không có source tracing, không sandbox, rủi ro hallucination cao trong bối cảnh lâm sàng.
- **Áp lực thi cử tăng**: Chuẩn hóa bài thi lâm sàng OSCE và thi quốc gia ngành Y tạo ra nhu cầu ôn tập cá nhân hóa, hiệu quả cao hơn bao giờ hết.

---

## Traction

Pre-launch. Đang trong giai đoạn Customer Discovery:

- **Vòng tròn bạn bè ban đầu**: 100% người được nghe mô tả sản phẩm muốn thử ngay — early demand signal trước cả khi có MVP.
- **[X] buổi phỏng vấn sâu** với sinh viên Y khoa năm 3–5 tại [Trường] *(điền khi hoàn thành)*.
- **[Y]%** xác nhận pain "mất quá nhiều thời gian chuẩn bị tài liệu ôn tập" *(điền từ transcript)*.
- PMF Signal target: **50 user hoàn thành ôn 50+ thẻ trong 48h** kể từ lần upload đầu tiên.

---

## Ask

Gọi **[Số tiền] VND pre-seed** để:

- [ ] Ra MVP (PDF parse → Diagnostic → Lộ trình → Flashcard) trong **[X] tháng**.
- [ ] Đạt **50 beta users đạt PMF signal** (50 thẻ / 48h).
- [ ] Validate LTV/CAC và unit economics trước khi scale.

Dùng vốn cho: engineering (2 dev), cloud infra (OpenAI + MinerU API), và chi phí customer acquisition cho cohort beta đầu tiên.
