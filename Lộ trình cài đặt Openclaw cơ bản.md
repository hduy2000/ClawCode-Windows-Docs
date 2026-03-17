# 🚀 Hướng dẫn cài OpenClaw (Bản dễ đọc)

---

## 1️⃣ Chuẩn bị

* Tạo thư mục (ví dụ):

  ```
  D:\Openclaw_Setup
  ```

* Tải file setup:
  [https://drive.google.com/drive/folders/1Q32QGB_UvpPC6MCV9tkR1WY-WI2TROXY](https://drive.google.com/drive/folders/1Q32QGB_UvpPC6MCV9tkR1WY-WI2TROXY)

---

## 2️⃣ Cài Codex

1. Truy cập: [https://chatgpt.com/](https://chatgpt.com/)
2. Đăng nhập
3. Tải và mở Codex

### 🔹 Model sử dụng

* Free → GPT-5.2 Codex
* Business+ → GPT-5.3 / GPT-5.4

---

## 3️⃣ Cài OpenClaw bằng Codex

### Prompt cài đặt

```text
Hãy đọc kỹ hướng dẫn sau kết hợp với OpenClaw_Setup_Pack, tiến hành cài đặt cho tôi
```

👉 Upload file hướng dẫn vào Codex trước khi chạy prompt

---

### ⚠️ Nếu lỗi cấu hình

```text
không sao, bạn cứ tiếp tục đi
```

---

### 🧾 Thông tin cần nhập

* Tên: (tên bạn)
* Agent: (tên AI)
* Nghề: Engineer (ví dụ)
* Múi giờ: GMT+7
* Xưng hô: gọi anh/chị, xưng em
* Ngôn ngữ: Tiếng Việt
* Telegram ID: nhập ID của bạn

---

## 4️⃣ Kết nối OAuth (Codex)

```bash
openclaw onboard
```

### Chọn:

* Provider: OpenAI
* Auth: Codex (OAuth)
* Model: GPT-5.x

👉 Các bước còn lại: **Skip for now**

---

## 5️⃣ Mở Web UI

Mở trình duyệt:

```
http://127.0.0.1:18789
```

👉 Đây là giao diện chat

---

## 6️⃣ Test nhanh

```bash
openclaw agent --agent main -m "hello"
```

---

## 7️⃣ Tạo Telegram Bot

1. Mở Telegram
2. Tìm: `@BotFather`
3. Gõ:

```text
/newbot
```

4. Đặt:

* Tên bot
* Username (phải có "bot")

👉 Lưu lại **Bot Token**

---

## 8️⃣ Thêm Token vào ENV

1. Tìm: `Edit environment variables`
2. Thêm biến:

```
TELEGRAM_BOT_TOKEN=your_token
```

---

## 9️⃣ Restart OpenClaw

```bash
openclaw gateway restart
```

---

## 🔁 Lệnh quan trọng

```bash
openclaw onboard
openclaw gateway restart
```

---

## 🤖 Dùng Telegram

* `/restart` → restart bot
* `/new` → reset context

---

## 🔗 Kết nối Google (Advanced)

Cho phép agent:

* Gmail
* Drive
* Sheets
* Calendar

### Cài skill "gog"

```text
check skill gog và cài đặt cho tôi
```

---

## 🧠 Ghi nhớ cho Agent

Bạn có thể nói:

```text
em hãy note cái này vào rule của mình
```

👉 Agent sẽ tự lưu vào:

* AGENT.md
* MEMORY.md
* IDENTITY.md

---

## ⚠️ Lưu ý

* Nếu hết rate limit → chạy lại:

```bash
openclaw onboard
```

* Không cần dùng Ollama nếu máy yếu

---

## 🎯 Kết luận

Sau khi setup xong:

✔️ Chat Web UI
✔️ Chat Telegram
✔️ Agent tự động làm việc

---

🔥 Tip:
Nếu lỗi → copy lỗi gửi cho Codex để nó tự sửa

---

Chúc bạn setup thành công 🚀
