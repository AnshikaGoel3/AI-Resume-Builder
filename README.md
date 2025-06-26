# AiIResume Builder

Ai Resume Builder is a modern, beginner-friendly web application that uses AI to help you create professional resumes in minutes. Just enter your details, and our AI (powered by DeepSeek via Ollama) will generate a tailored, job-ready resume for you—no writing or design skills needed!

## 🚀 Features

- **AI-Powered Resume Generation:** Automatically creates resume content using the DeepSeek model through the Ollama API.
- **Live Preview:** Instantly see your resume update as you fill in your information.
- **PDF Download:** Download your completed resume as a polished PDF.
- **No Database Required:** All data is handled in-memory for simplicity.
- **Clean, Modular Code:** Backend follows Object-Oriented Programming (OOP) principles for easy understanding and maintenance.

## 🛠️ Tech Stack

- **Frontend:** Next.js (React), Tailwind CSS
- **Backend:** Spring Boot (Java)
- **AI Integration:** DeepSeek via Ollama API



text

## ⚡️ Getting Started

### 1. Clone the Repository

git clone https://github.com/yourusername/Ai-Resume-Builder.git
cd Ai-Resume-Builder

text

### 2. Set Up the Backend

**Requirements:**  
- Java 17+  
- Maven  
- [Ollama](https://ollama.com/) installed and running DeepSeek model locally

**Steps:**
1. Go to the `backend` folder:
cd backend

text
2. Configure Ollama and DeepSeek:
- Start Ollama:  
  ```
  ollama serve
  ollama run deepseek
  ```
- Make sure your Spring Boot app is set to call Ollama's API (usually at `http://localhost:11434`).
3. Start the backend server:
mvn spring-boot:run

text

### 3. Set Up the Frontend

**Requirements:**  
- Node.js 18+

**Steps:**
1. Go to the `frontend` folder:
cd ../frontend

text
2. Install dependencies:
npm install

text
3. Start the frontend server:
npm run dev

text
4. Open `http://localhost:3000` in your browser.

## 🧠 How It Works

1. **Enter Your Details:** Fill in your skills, experience, and desired job role on the frontend.
2. **AI Generation:** The frontend sends your info to the backend API (Spring Boot).
3. **DeepSeek AI:** The backend formats your data and sends it to DeepSeek via Ollama. The AI generates professional resume content.
4. **Live Preview:** The frontend displays the AI-generated resume in real time.
5. **Download:** Export your resume as a PDF.

## 📦 Example API Usage

**Endpoint:**  
`POST /api/generate-resume`

**Request Body:**
{
"name": "Jane Doe",
"skills": "Java, Spring Boot, React",
"experience": "2 years at TechCorp",
"jobRole": "Backend Developer"
}

text

**Response:**
{
"resume": "Jane Doe\nBackend Developer\nSkills: Java, Spring Boot, React\nExperience: 2 years at TechCorp\n..."
}

text

## 📝 License

This project is open source and available under the [MIT License](LICENSE).


**Start building your professional resume in minutes with Ai Resume Builder!**
