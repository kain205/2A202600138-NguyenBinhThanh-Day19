# Pitch Memo — Synapsy
> 1-pager | Pre-launch | 2026

---

## Problem

Sinh viên Y khoa VN không thể dùng AI để ôn thi. Không phải vì AI không đủ thông minh — mà vì liều thuốc sai trong một thẻ flashcard có thể hủy hoại niềm tin vào toàn bộ bộ thẻ. Kết quả: họ vẫn đang mất 3–5h/ngày tự tạo flashcard thủ công trên Anki, và vào mùa thi họ không biết ưu tiên ôn gì trước.

---

## Insight

**Insight 1 — Trust gap, không phải accuracy gap.**
Với sinh viên Y khoa, rào cản adoption AI không phải accuracy — mà là *khả năng kiểm chứng*. Họ cần biết AI lấy thông tin đó từ đâu, không phải AI có đúng không. Source traceability giải quyết tâm lý, không phải kỹ thuật. Đây là insight mà tất cả các edtech AI đang bỏ qua.

**Insight 2 — Data flywheel tạo moat thật.**
Mỗi lần sinh viên đánh giá thẻ (Easy / Hard / Again), hệ thống SRS tích lũy dữ liệu về lỗ hổng cá nhân của họ. Càng dùng, lộ trình ôn tập càng cá nhân hóa — switching cost tăng theo thời gian theo cách ChatGPT không thể replicate vì không có persistence data.

---

## Solution

Synapsy: upload slide PDF → AI chẩn đoán lỗ hổng → tạo lộ trình học cho tối nay → auto flashcard với SRS tích lũy theo thời gian.

Pipeline kỹ thuật: MinerU parse PDF → GPT-4o đọc toàn bộ text một lần, tạo quiz chẩn đoán + outline → GPT-4o-mini expand từng lesson thành Concept Cards song song → SRS (SM-2) lưu CardProgress cá nhân.

**Differentiator cốt lõi: mỗi flashcard trỏ thẳng tới trang và dòng trong file gốc của chính sinh viên.** Bấm "Xem nguồn" → màn hình chia đôi, highlight đúng dòng. Không phải feature — đây là cơ chế phá vỡ rào cản tâm lý.

Chatbot sandboxed: hỏi đào sâu một thẻ bất kỳ, AI chỉ dùng file đã upload. Không có hallucination ngoài luồng.

---

## Why Now

- LLM đã đủ tốt để parse tài liệu y khoa tiếng Việt phức tạp (bảng, sơ đồ, thuật ngữ lâm sàng).
- Sinh viên Y thế hệ mới đang dùng ChatGPT để ôn thi — nhưng không có source control, không có persistence, không có lộ trình cá nhân.
- Anki/Quizlet đòi nhập liệu thủ công — gap lớn chưa ai lấp tại VN.
- Áp lực thi ngành Y tăng (OSCE, thi quốc gia) trong khi không có công cụ nào thiết kế riêng cho context này.
- **Beachhead → Expansion**: 60–90K sinh viên Y là thị trường đầu tiên có pain rõ nhất và zero-tolerance cao nhất. Sau PMF: 2M+ sinh viên đại học VN có cùng workflow — upload tài liệu, ôn thi, cần biết học gì trước.

---

## Traction

Chưa có số. Đang trong tuần đầu structured customer discovery với 10 sinh viên Y năm 3–5. Số thật — pain confirmation rate, willingness to pay, beta commitment — sẽ có trước khi ký bất kỳ term sheet nào.

PMF Signal target duy nhất: **50 users hoàn thành ôn 50+ thẻ trong 48h kể từ lần upload đầu tiên.** Nếu không đạt số này, pivot trước khi scale.

---

## Ask

**[Số tiền] VND pre-seed** — dùng cho:
- Cloud infra: OpenAI API + MinerU parsing pipeline cho 50 beta users
- Hosting (Firebase + Vercel) × 6 tháng
- Buffer cho iteration sau beta

**Team**: Solo founder hiện tại — đủ để build và prove MVP. Kế hoạch tìm co-founder kỹ thuật hoặc go-to-market sau khi có PMF signal đầu tiên — tránh dilute equity trước khi có proof.

Milestone duy nhất quan trọng sau vòng này: **50 users / 50 thẻ / 48h**. Đó là số chứng minh người dùng thực sự học — không phải chỉ đăng ký rồi bỏ.
