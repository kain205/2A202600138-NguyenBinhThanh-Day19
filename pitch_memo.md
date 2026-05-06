# Pitch Memo — Synapsy
> 1-pager | Pre-launch | 2026

---

## Problem

Sinh viên Y khoa VN không thể dùng AI để ôn thi. Không phải vì AI không đủ thông minh — mà vì liều thuốc sai trong một thẻ flashcard có thể hủy hoại niềm tin vào toàn bộ bộ thẻ. Kết quả: họ vẫn đang mất 3–5h/ngày tự tạo flashcard thủ công trên Anki, và vào mùa thi họ không biết ưu tiên ôn gì trước.

---

## Insight

Với sinh viên Y khoa, rào cản adoption AI không phải accuracy — mà là *khả năng kiểm chứng*. Họ cần biết AI lấy thông tin đó từ đâu, không phải AI có đúng không. Source traceability giải quyết tâm lý, không phải kỹ thuật. Đây là insight mà tất cả các edtech AI đang bỏ qua.

Và một khi rào cản niềm tin được phá vỡ, hành vi học tập tích cực mở ra hoàn toàn.

---

## Solution

Synapsy: upload slide PDF → AI chẩn đoán lỗ hổng → tạo lộ trình học cho tối nay → auto flashcard với SRS.

Differentiator duy nhất quan trọng: **mỗi flashcard trỏ thẳng tới trang và dòng trong file gốc của chính sinh viên.** Bấm "Xem nguồn" → màn hình chia đôi, highlight đúng dòng. Không phải feature — đây là cơ chế phá vỡ rào cản tâm lý.

Chatbot sandboxed: hỏi đào sâu một thẻ bất kỳ, AI chỉ dùng file đã upload. Không có hallucination ngoài luồng.

---

## Why Now

LLM đã đủ tốt để parse tài liệu y khoa tiếng Việt phức tạp. Sinh viên Y thế hệ mới đang dùng ChatGPT — nhưng không có source control. Gap giữa "đang dùng ChatGPT để ôn thi" và "có thể thực sự tin tưởng AI với kiến thức lâm sàng" là khoảng trắng Synapsy lấp.

Áp lực thi ngành Y tại VN đang tăng (OSCE, thi quốc gia) trong khi không có công cụ nào được thiết kế riêng cho context này.

---

## Traction

Chưa có số. Đang trong tuần đầu structured customer discovery với 10 sinh viên Y năm 3–5. Số thật — pain confirmation rate, willingness to pay, beta commitment — sẽ có trước khi ký bất kỳ term sheet nào.

PMF Signal target duy nhất: **50 users hoàn thành ôn 50+ thẻ trong 48h kể từ lần upload đầu tiên.** Nếu không đạt số này, chúng em pivot trước khi scale.

---

## Ask

**[Số tiền] VND pre-seed** — dùng cho:
- Engineering: 2 dev × [X] tháng → ra MVP đủ để test PMF signal
- Cloud infra: OpenAI API + MinerU parsing pipeline
- Customer acquisition: 50 beta users có structured onboarding

Milestone duy nhất quan trọng sau vòng này: **50 users / 50 thẻ / 48h**. Đó là số chứng minh người dùng thực sự học — không phải chỉ đăng ký rồi bỏ.
