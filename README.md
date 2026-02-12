
# 📚 AI Tutor & Quiz Generator

### LearnSphere Academy

*Mistral / LLaMA 2 + Ollama + FastAPI + Streamlit*

---

## 🌍 Project Overview

LearnSphere Academy delivers online courses and aims to automate intelligent learning support for instructors and students.

Educators spend significant time simplifying lecture notes, creating quizzes, and identifying key revision concepts.
Students often struggle with understanding complex material, knowing what to revise, and practicing effectively.

This project builds an **AI Tutor Assistant** that transforms raw educational content into structured, student-friendly learning material.

---

## 🎯 Project Goal

Convert educational content into:

### 📥 Input

* Lecture notes
* Textbook paragraphs
* Academic content
* Pasted text
* `.txt` files

### 📤 Output

* Student-friendly simplified explanation
* 5-question quiz (MCQ or short-answer with answers)
* 5–10 key concepts for revision

---

## 🧠 Models Used

### Mistral (via Ollama)

* Lightweight and efficient
* Strong structured generation performance

### LLaMA 2 (Optional Alternative)

* Good long-text understanding
* Reliable question generation

Both models are used for:

* Text simplification
* Question generation
* Concept extraction
* Educational structuring

---

## 🛠 Technology Stack

* **Backend:** FastAPI
* **LLM Hosting:** Ollama
* **Models:** Mistral / LLaMA 2
* **Frontend:** Streamlit
* **Input Format:** Text / `.txt`
* **Version Control:** Git & GitHub

---

## 📂 Project Structure

```
ai-tutor-learnsphere/
│
├── backend/
│   └── main.py
│
├── frontend/
│   └── app.py
│
├── data/
│   └── sample_lesson.txt
│
├── requirements.txt
└── README.md
```

---

## ✨ Features

* Simplifies complex lessons into student-friendly explanations
* Automatically generates 5 quiz questions with answers
* Extracts 5–10 key revision concepts
* Fast local inference using Ollama
* Clean FastAPI backend with Streamlit UI
* Structured output for educational workflows

---

## 🔄 System Workflow

1. User uploads or pastes lesson content
2. Frontend sends request to FastAPI backend
3. Backend sends structured prompt to Mistral / LLaMA 2 via Ollama
4. Model generates:

   * Simplified explanation
   * Quiz with answers
   * Key concepts
5. Results displayed in Streamlit dashboard

---

## 🚀 How to Run

### 1️⃣ Install Ollama

Download from: [https://ollama.ai](https://ollama.ai)

---

### 2️⃣ Pull Model

For Mistral:

```bash
ollama pull mistral
```

For LLaMA 2:

```bash
ollama pull llama2
```

---

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 4️⃣ Start Backend

```bash
uvicorn backend.main:app --reload
```

---

### 5️⃣ Start Frontend

```bash
streamlit run frontend/app.py
```

---

## 📌 Example

**Input:**
Photosynthesis lecture note

**Output:**

**Simplified Explanation:**
Photosynthesis is the process by which plants use sunlight, carbon dioxide, and water to produce food and oxygen.

**Quiz Questions:**

1. What is photosynthesis?
2. Which gas do plants absorb?
3. What is produced during photosynthesis?
4. Where does photosynthesis occur?
5. Why is sunlight important?

**Key Concepts:**

* Chlorophyll
* Sunlight
* Carbon dioxide
* Oxygen
* Glucose
* Chloroplast

---

## 📈 Future Improvements

* Difficulty-level control (Beginner / Intermediate / Advanced)
* Bloom’s Taxonomy-based question generation
* PDF upload support
* Export to PDF/DOCX
* Adaptive quizzes
* Multi-language support

---

## ⚠️ Disclaimer

This project is intended for educational and prototype purposes only.
It does not replace professional academic instruction.

