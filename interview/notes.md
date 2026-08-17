# Interview Notes — Case B: AI Notes

## Thông tin chung

- **Interviewer:** Vũ Huy Hoàng
- **MHV:** 2A202601057
- **Case đã chọn:** Case B — AI Notes: Personal Learning Notes
- **Số lượt practice interview:** 2
- **Đồng ý ghi âm:** Có ở cả hai lượt

> Hai lượt dưới đây được ghi lại đúng theo nội dung người tham gia đã nói. Không bổ sung hành vi highlight/note nếu người tham gia không đề cập.

---

# Interview Record 1 — P01

## Recruitment / mở đầu

Interviewer xin phép ghi âm để xem lại và ghi chép chính xác. Người tham gia đồng ý.

Interviewer hỏi:

> Trong 7 ngày gần đây, bạn có lần nào đang học mà gặp một phần chưa hiểu và phải tự tìm cách xử lý không?

Người tham gia trả lời **Có**, với tình huống gần nhất khi học **Day 13 — Monitoring, Logging, Observability**, phần **P95 latency**.

---

## Câu chuyện gần nhất

Người tham gia đang học phần monitoring. Khi slide nói về **P50, P95 và P99 latency**, người tham gia không hiểu:

- tại sao P95 lại quan trọng;
- tại sao không chỉ dùng average latency.

---

## User đã thực sự làm gì?

Trình tự hành vi:

1. Đọc lại slide.
2. Tìm Google.
3. Hỏi ChatGPT về sự khác nhau giữa average latency và P95 latency.
4. Xem lại ví dụ về P50, P95, P99.
5. Sau đó mới nhận ra phần chưa hiểu thực sự là khái niệm **percentile**.
6. Quay lại bài học sau khi đã hiểu hơn.

---

## Khó khăn và workaround

### Khó khăn

Người tham gia không xác định ngay được mình đang thiếu kiến thức gì.

Ban đầu:

> “Mình nghĩ mình chưa hiểu monitoring.”

Sau đó mới nhận ra:

> “Mình chưa hiểu rõ khái niệm percentile.”

### Workaround

```text
Đọc lại slide
→ Google
→ ChatGPT
→ Xem lại ví dụ P50/P95/P99
→ Xác định knowledge gap là percentile
```

---

## Hậu quả / chi phí

- Mất khoảng **15–20 phút**.
- Phải dừng phần đang học.
- Bị chậm.
- Bị **mất mạch một chút**.

---

## Pattern có lặp

Người tham gia kể trước đó từng gặp tình huống tương tự khi học **AI Evaluation**:

- có vài metric không hiểu;
- phải tìm thêm nguồn ngoài;
- cũng không biết ngay chính xác phần kiến thức mình thiếu.

---

## Exact Quotes

> “Mình đang học phần monitoring. Khi slide nói về P50, P95 và P99 latency thì mình không hiểu tại sao P95 lại quan trọng và vì sao không chỉ dùng average latency.”

> “Không. Ban đầu mình nghĩ mình chưa hiểu monitoring, nhưng sau đó mới nhận ra mình chưa hiểu rõ khái niệm percentile.”

> “Mình phải dừng phần đang học để tìm hiểu lại percentile, nên bị chậm và mất mạch một chút.”

---

## Evidence Summary — P01

| Cần kiểm tra | Kết quả | Evidence |
|---|---|---|
| Có một sự kiện gần đây | Có | Day 13 — P95 latency |
| User có hành vi học thực tế | Có | Đọc lại slide, Google, ChatGPT |
| Có workaround | Có | Dùng nhiều nguồn để tự xử lý |
| Có consequence | Có | Mất 15–20 phút, chậm và mất mạch |
| Pattern có lặp | Có | Trước đó từng gặp ở AI Evaluation |
| Có evidence trực tiếp về highlight/note của Case B | **Không** | Người tham gia không đề cập highlight/note |

---

# Interview Record 2 — P02

## Recruitment / mở đầu

Interviewer xin phép ghi âm để xem lại và ghi chép chính xác. Người tham gia đồng ý.

Interviewer hỏi:

> Trong 7 ngày gần đây, bạn có lần nào đang học mà gặp một phần chưa hiểu và phải tự tìm cách xử lý không?

Người tham gia trả lời **Có**, với tình huống gần nhất khi học **Day 12 — Agent Service**, phần **Rate Limiting**.

---

## Câu chuyện gần nhất

Người tham gia đang học cách giới hạn số request của user.

Người tham gia:

- hiểu mục đích của rate limit;
- chưa hiểu Sliding Window hoạt động như thế nào;
- chưa hiểu tại sao lại dùng Redis Sorted Set.

---

## User đã thực sự làm gì?

Trình tự hành vi:

1. Đọc lại phần hướng dẫn.
2. Xem code mẫu.
3. Tìm thêm trên Google.
4. Hỏi ChatGPT bằng ví dụ một user gửi **5 request trong 1 phút**.
5. Hiểu rằng Redis Sorted Set dùng để lưu timestamp của request.
6. Sau đó mới nhận ra phần khó thực sự là cơ chế **Sliding Window**.
7. Quay lại đọc code và thấy dễ hiểu hơn.

---

## Khó khăn và workaround

### Khó khăn

Ban đầu người tham gia nghĩ:

> “Mình chưa hiểu Redis.”

Sau đó mới nhận ra:

> Phần mình chủ yếu chưa hiểu là **cơ chế Sliding Window**.

### Workaround

```text
Đọc lại hướng dẫn
→ Xem code mẫu
→ Google
→ ChatGPT
→ Hiểu vai trò Redis Sorted Set
→ Xác định điểm vướng là Sliding Window
```

---

## Hậu quả / chi phí

- Mất khoảng **20 phút**.
- Phải dừng phần đang làm.
- Bị chậm tiến độ một chút.
- Sau khi hiểu thì đọc code dễ hơn.

---

## Pattern có lặp

Người tham gia kể trước đó từng gặp khi học **Docker Compose**:

- không hiểu sự khác nhau giữa localhost và tên service;
- ban đầu chỉ thấy code không chạy như mình nghĩ;
- sau đó mới nhận ra mình chưa hiểu networking giữa các container.

---

## Exact Quotes

> “Mình hiểu mục đích của rate limit nhưng chưa hiểu Sliding Window hoạt động như thế nào và tại sao lại dùng Redis Sorted Set.”

> “Không. Ban đầu mình nghĩ là mình chưa hiểu Redis, nhưng sau đó mới nhận ra mình chủ yếu chưa hiểu cơ chế Sliding Window.”

> “Mình phải dừng phần đang làm để tìm hiểu lại nên bị chậm tiến độ một chút. Nhưng sau khi hiểu thì mình đọc code dễ hơn.”

---

## Evidence Summary — P02

| Cần kiểm tra | Kết quả | Evidence |
|---|---|---|
| Có một sự kiện gần đây | Có | Day 12 — Rate Limiting |
| User có hành vi học thực tế | Có | Hướng dẫn, code mẫu, Google, ChatGPT |
| Có workaround | Có | Dùng nhiều nguồn để tự xử lý |
| Có consequence | Có | Mất khoảng 20 phút, chậm tiến độ |
| Pattern có lặp | Có | Trước đó từng gặp ở Docker Compose |
| Có evidence trực tiếp về highlight/note của Case B | **Không** | Người tham gia không đề cập highlight/note |

---

# Cross-Interview Summary

## Pattern chung

Hai cuộc phỏng vấn đều cho thấy:

```text
Learner gặp một phần chưa hiểu
→ Nhận ra mình bị vướng
→ Không xác định ngay được điểm thiếu thực sự
→ Đọc lại / Google / ChatGPT / xem code
→ Sau một thời gian mới xác định đúng điểm thiếu
→ Quay lại bài học
```

## Workaround chung

Cả hai người tham gia đều dùng nhiều nguồn:

- nội dung bài học;
- Google;
- ChatGPT;
- ví dụ hoặc code mẫu.

## Consequence chung

| Participant | Thời gian | Ảnh hưởng |
|---|---:|---|
| P01 | 15–20 phút | Dừng bài, chậm, mất mạch |
| P02 | ~20 phút | Dừng phần đang làm, chậm tiến độ |

---

# Liên hệ với Case B

Hai lượt practice interview này cung cấp evidence tốt về **friction khi learner gặp phần chưa hiểu**, nhưng **không cung cấp evidence trực tiếp cho hai Pain Hypothesis của Case B về hành vi highlight/note**.

Cụ thể, hai interview không trả lời được các câu hỏi cốt lõi:

- Learner highlight/note với mục đích gì?
- Learner có quay lại sử dụng note/highlight không?
- Việc tìm/gom/tổng hợp note có tạo friction không?
- Highlight/note có chỉ phục vụ việc tập trung trong lúc học không?

Do đó, các interview này được dùng chủ yếu để **review kỹ thuật hỏi và sửa Conversation Guide**, không được dùng để khẳng định Pain A hay Pain B của Case B là đúng.

---

# Ghi chú của interviewer

Điểm cần cải thiện sau practice:

1. Recruitment Check cần bám đúng tiêu chí Case B: hành vi highlight/note trong 7 ngày gần đây.
2. Story Opener cần mở bằng một lần highlight/note cụ thể, không mở bằng “một phần chưa hiểu”.
3. Cần hỏi trực tiếp mục đích của hành vi highlight/note.
4. Cần kiểm tra user có quay lại dùng note hay không.
5. Nếu user có quay lại, mới đào friction/workaround/consequence.
6. Nếu user không quay lại, cần đào xem highlight/note giúp gì ngay trong lúc học.

> Chưa tuyên bố Pain A hoặc Pain B đã được validated.
