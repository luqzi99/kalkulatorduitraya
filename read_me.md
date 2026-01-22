# 🧮 Duit Raya Calculator

**Gamified Raya Budgeting Tool untuk Rakyat Malaysia**

---

## 1. Pengenalan

**Duit Raya Calculator** ialah aplikasi web ringan yang membantu pengguna:

* Mengira **jumlah duit raya** berdasarkan pecahan wang (RM1, RM5, RM10, RM50, RM100)
* Merancang **pecahan duit raya berdasarkan bajet**
* Menyediakan **ringkasan mesra bank** untuk urusan tukar duit
* Memberikan pengalaman **Raya vibe + gamification** supaya penggunaan lebih menyeronokkan

Sesuai untuk:

* Individu / keluarga
* Orang yang buka **servis tukar duit raya**
* Agent / runner bank

---

## 2. Masalah yang Diselesaikan

### Pain Point

* Kira duit raya secara manual leceh
* Salah kira jumlah keseluruhan
* Susah nak explain kepada bank pecahan yang diperlukan
* Bajet terlebih atau berbaki tanpa sedar

### Solusi

* Kalkulator automatik
* Pecahan jelas & tepat
* Boleh terus **share / screenshot**
* Gamification untuk engagement

---

## 3. Core Features (MVP)

### 🔢 Mode A: Pecahan Ikut Bilangan Keping

User masukkan bilangan keping bagi setiap denominasi.

**Input:**

* RM1, RM5, RM10, RM50, RM100 (bilangan keping)

**Output:**

* Jumlah keseluruhan (RM)
* Jumlah keping
* Ringkasan bank-friendly

---

### 💰 Mode B: Pecahan Ikut Bajet

User masukkan jumlah bajet dan pilih denominasi.

**Pilihan logic:**

* Equal distribution
* Priority-based distribution (percentage)

**Output:**

* Pecahan automatik
* Baki (jika ada)
* Visual progress bar

---

## 4. Gamification Design

### 🎯 Progress Bar

* Nama: **Persiapan Duit Raya**
* Berdasarkan penggunaan bajet

### 🏆 Badge System

Badge unlock secara local (tanpa login):

* 🎁 Raja Duit Raya – >500 keping
* 🧧 Budget Master – Bajet tepat (RM0 baki)
* 🌟 Family Hero – Bajet > RM1000
* 🔥 Power Planner – Semua denominasi digunakan

### 🎊 Celebration

* Confetti animation bila kiraan siap
* Copywriting positif & Raya tone

---

## 5. UI / UX Guideline

### Visual Vibe

* Tema: **Raya moden + traditional**
* Warna utama: Emerald Green, Gold Accent
* Elemen visual: Ketupat, geometric Islamic pattern

### UX Flow

1. Pilih mode
2. Masukkan input
3. Tekan "Kira Duit Raya 🎉"
4. Papar result + badge + share

---

## 6. AI Agent (VS Code – Developer Agent)

> **Nota penting:** AI Agent ini **BUKAN untuk end-user**. Ia ialah **developer AI agent** yang digunakan **dalam VS Code** untuk bantu bina, iterate dan ship projek *Duit Raya Calculator* dengan pantas.

---

## 🎯 Tujuan AI Agent (Developer-Focused)

AI Agent ini bertindak sebagai:

* 🧠 **Product co-pilot** (MVP → iteration)
* 🧮 **Logic validator** (kiraan duit raya tepat)
* 🎨 **UI/UX assistant** (Raya vibe + gamification)
* 🧪 **QA checker** (edge case & validation)

Agent ini digunakan secara:

* Chat-based (prompt-driven)
* Code-aware (rujuk file dalam repo)

---

## 🤖 Agent Name

**RayaDev Agent**

---

## 🧩 Agent Roles (Multi-Agent dalam 1 Persona)

### 1️⃣ Calculator Logic Agent

**Tugas:**

* Validate formula kiraan
* Handle rounding & baki
* Check edge case (negative, kosong, overflow)

**Contoh prompt:**

```
Semak logic kiraan duit raya untuk mode pecahan bajet.
Pastikan baki minimum dan jumlah sentiasa tepat.
```

---

### 2️⃣ Gamification Designer Agent

**Tugas:**

* Tentukan badge unlock rule
* Progress bar calculation
* Celebration trigger

**Contoh prompt:**

```
Cadangkan badge rule yang adil dan menyeronokkan
untuk kalkulator duit raya tanpa login.
```

---

### 3️⃣ UI/UX Raya Agent

**Tugas:**

* Pastikan UI ada Raya vibe
* Suggest animation ringan
* Optimize mobile-first UX

**Contoh prompt:**

```
Review UI component ini dan cadangkan
improvement supaya lebih Raya dan fun.
```

---

### 4️⃣ Copywriting & Tone Agent

**Tugas:**

* Generate ayat Raya
* Result message positif
* Share card caption

**Contoh prompt:**

```
Hasilkan ayat ringkas bertema Raya
untuk result screen Duit Raya Calculator.
```

---

### 5️⃣ QA / Edge Case Agent

**Tugas:**

* Cari bug logik
* Test scenario real Malaysian use-case

**Contoh prompt:**

```
Test semua edge case untuk calculator duit raya
termasuk bajet kecil, besar dan pecahan tak seimbang.
```

---

## 🧠 Master System Prompt (UNTUK VS CODE)

Gunakan prompt ini sebagai **system / instruction** dalam VS Code AI tool:

```
You are RayaDev Agent.
You are a senior Malaysian fullstack engineer.
Your task is to help build a gamified Duit Raya Calculator web app.

Rules:
- All calculations must be mathematically correct
- Prioritize simplicity over over-engineering
- UI must feel festive, Raya-themed, and mobile-first
- Assume Malaysian users and local context
- Suggest improvements but respect MVP scope
- Respond in Bahasa Malaysia unless technical clarity requires English
```

---

## 🛠️ Cara Guna Dalam VS Code

### Option A: GitHub Copilot Chat

* Paste **Master System Prompt** sebagai context
* Rujuk file: `calculator.js`, `ui.vue`, `logic.ts`

### Option B: Cursor / Continue / Cody

* Set sebagai **project instruction**
* Aktifkan codebase awareness

---

## 7. Tech Stack

### Frontend

* HTML
* Tailwind CSS
* Alpine.js / Vue

### AI (Optional MVP+)

* HuggingFace Inference API / Groq

### Storage

* LocalStorage (history, badge)

### Backend

* ❌ Not required for MVP

---

## 8. Non-Goals (Out of Scope MVP)

* User login
* Payment gateway
* Bank integration
* Mobile app

---

## 9. Monetization (Future)

### Free

* Calculator
* Basic gamification

### Paid (Optional)

* Export PDF
* Branding untuk agent
* History unlimited

---

## 10. Deployment

### Static Hosting

* Netlify
* Vercel
* GitHub Pages

### Domain Idea

* duitraya.my
* kiraduiraya.my
* rayacalculator.my

---

## 11. Success Metrics

* Daily active users
* Share rate (WhatsApp)
* Average calculation per user

---

## 12. Roadmap (Optional)

### Phase 1

* MVP calculator
* Gamification basic

### Phase 2

* AI suggestion
* Share card image

### Phase 3

* Agent / runner mode
* PDF export

---

## 13. Philosophy

> "Benda simple, tapi solve masalah sebenar rakyat Malaysia masa Raya."

---

## 14. VS Code Prompt Pack (RayaDev Agent)

Gunakan prompt ini **terus dalam VS Code** (Copilot Chat / Cursor / Continue). Susun ikut fasa kerja supaya konsisten.

### 🔹 P0 — Project Bootstrap

**Tujuan:** Set context projek & elak over-engineering.

```
You are RayaDev Agent.
This is a gamified Duit Raya Calculator for Malaysian users.
Scope: static web, no backend for MVP.
Use Tailwind + vanilla JS or Alpine.
Keep logic simple, correct, and mobile-first.
```

---

### 🔹 P1 — Calculator Logic (Mode A: Ikut Keping)

**Tujuan:** Pastikan formula tepat & selamat.

```
Review and implement calculator logic for Mode A (pecahan ikut bilangan keping).
Rules:
- Denominations: RM1, RM5, RM10, RM50, RM100
- Reject negative numbers
- Treat empty input as 0
- Return total amount and total pieces
- Output bank-friendly breakdown string
```

---

### 🔹 P2 — Calculator Logic (Mode B: Ikut Bajet)

**Tujuan:** Agihan bajet praktikal Malaysia.

```
Design Mode B logic (pecahan ikut bajet).
Inputs:
- Total budget (RM)
- Enabled denominations
Options:
- Equal distribution
- Priority-based (percentage)
Constraints:
- Avoid fractional money
- Minimize leftover
- Explain leftover if exists
```

---

### 🔹 P3 — Gamification Rules

**Tujuan:** Engagement tanpa login.

```
Define gamification rules for Duit Raya Calculator.
Include:
- Progress bar calculation
- Badge unlock conditions
- Celebration trigger
Keep everything client-side (localStorage).
```

---

### 🔹 P4 — UI/UX Raya Review

**Tujuan:** Pastikan vibe Raya, bukan app biasa.

```
Review this UI component for Raya vibe.
Check:
- Color harmony (emerald, gold)
- Readability of numbers
- Mobile-first spacing
- Micro-interactions suitability
Suggest improvements only if impactful for MVP.
```

---

### 🔹 P5 — Copywriting (Result Screen)

**Tujuan:** Ayat pendek, mesra Malaysia.

```
Generate short Raya-themed messages in Bahasa Malaysia
for result screen and share card.
Tone:
- Positive
- Friendly
- Not cringe
Examples:
- Success message
- Budget warning
- Badge unlocked
```

---

### 🔹 P6 — QA & Edge Case Sweep

**Tujuan:** Elak bug masa orang guna betul-betul.

```
Act as QA engineer.
Test Duit Raya Calculator for:
- RM0 budget
- Very large budget (RM10,000)
- Single denomination only
- All denominations enabled
- Empty inputs
List bugs and suggest fixes.
```

---

### 🔹 P7 — Refactor & Cleanup

**Tujuan:** Code kemas sebelum deploy.

```
Refactor this code for readability and maintainability.
Constraints:
- No premature optimization
- Keep functions small
- Add comments only where logic is non-obvious
```

---

## 15. Cara Guna (Workflow Cadangan)

1. Paste **P0** sebagai initial context
2. Implement logic guna **P1 → P2**
3. Tambah gamification (**P3**)
4. Polish UI (**P4 + P5**)
5. QA final (**P6 → P7**)

---

## 16. Notes Penting

* Jangan biar agent buat keputusan product besar tanpa semak
* AI = co-pilot, bukan autopilot
* Screenshot friendliness = feature utama

---

**Owner:** Luqman Hakim
**Project:** Duit Raya Calculator
**Agent:** RayaDev Agent
