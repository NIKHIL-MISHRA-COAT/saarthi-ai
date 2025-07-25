# 🧠 Saarthi AI – Your Personal AI Mock Interview Assistant 🎙️


**Saarthi AI** is a voice-interactive mock interview platform where users practice real-time interviews, guided by AI. With smart role-based questions and instant feedback, Saarthi helps candidates level up their confidence and interview skills.

---

## 🌀 Complete Workflow (Realistic)

![WhatsApp Image 2025-07-22 at 18 02 17_fd5799de](https://github.com/user-attachments/assets/7cd36427-2efa-489e-be69-451415dc8d79)



### 👤 Ek Typical Interview Flow:

1. **User Login / Signup**:
   - Candidate logs in or registers on Saarthi platform.

2. **Interview Scheduling**:
   - Candidate clicks on “Schedule Interview”.
   - AI Assistant (via Vapi) asks:
     - 💼 Job Role (e.g., Frontend Dev)
     - ⚙️ Tech Stack (React, MongoDB, etc.)
     - ⏳ Experience Level (Fresher/1-3/3+)
     - ❓ Number of Questions

3. **AI Flow Begins**:
   - Vapi AI collects the inputs and sends them to the Saarthi app.
   - Saarthi app forwards this data to **Gemini API**.
   - Gemini generates **custom questions** based on the input.
   - Questions are saved in **Firebase**.
   - Interview is now visible in the candidate’s **dashboard**.

4. **Live Interview**:
   - User starts the interview from dashboard.
   - Vapi AI asks questions one by one.
   - User responds via mic → Vapi transcribes and records.

5. **Feedback Generation**:
   - All responses are sent to Gemini for **AI-based analysis**.
   - Gemini provides personalized feedback.
   - Saarthi saves feedback in **Firebase**.

6. **Interview Ends**:
   - Dashboard shows summary: 📊 Score, 📝 Feedback, 🔁 Retry Option

---

## 🛠️ Tech Stack

| Tech       | Purpose                                  |
|------------|------------------------------------------|
| 🧱 Next.js  | Frontend with SSR                        |
| 🎨 Tailwind | UI styling                              |
| 🔥 Firebase | Auth, Firestore DB, Realtime Storage    |
| 🧠 Gemini   | AI Question + Feedback Generator         |
| 🎤 Vapi AI  | Voice API: question-asking + transcribe  |

---

## 🖼️ Screenshots

<img width="1759" height="898" alt="image" src="https://github.com/user-attachments/assets/649b7387-ea39-48d5-aefc-6c08b2f7cdcd" />
<img width="1801" height="896" alt="image" src="https://github.com/user-attachments/assets/3980a2a7-7364-4208-b65a-419a6b9f4f3b" />



---

## ⚙️ Setup Locally

```bash
git clone https://github.com/your-username/saarthi-ai.git
cd saarthi-ai
npm install
npm run dev
