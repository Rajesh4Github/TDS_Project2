# TDS Assignment Assistant - Project Documentation

This project is an **LLM-based API application** designed to assist students enrolled in the IIT Madras Online Diploma in Data Science program. The API provides automated answers to questions from five graded assignments in the *Tools in Data Science* course. Below is a detailed description of the process followed during the development and deployment of this project.

---

## **Project Overview**

The **TDS Assignment Assistant** is a REST API that:
- Accepts assignment questions and optional file attachments via a POST request.
- Processes the input using a large language model (LLM).
- Returns accurate answers for questions from Graded Assignments 1–5.

The application is deployed on Vercel, making it accessible to anyone at a public URL:  
'https://python-vercel-app-mu.vercel.app/api/`

---

## **Process Followed**

### 1. **Planning**
- Defined the primary goal: Automating answers for graded assignments.
- Identified user needs: Students require quick, accurate responses for specific assignment questions.
- Chose Vercel for deployment due to its ease of use, scalability, and free-tier hosting.

---

### 2. **API Design**
- Designed a single endpoint:  
  `POST https://python-vercel-app-mu.vercel.app/api/`
  
- Input:
  - `question`: The text of the GA Question (required).
  - `attachments`: Optional file attachments (e.g., datasets or reference materials).

- Output:
  - JSON response containing:
    - The Answer.

---

### 3. **Development**
- Used **Next.js API routes** for serverless functionality.


### 4. **Testing**
- Conducted unit tests for:
  - Validating input fields (`GA question`).
  - Ensuring proper handling of file attachments.
  - Verifying LLM-generated responses match expected outputs.
- Used CURL to test API endpoints manually.

---

### 5. **Deployment**
- Deployed the application on Vercel:
  - Configured environment variables (`OPENAI_API_KEY`, etc.).
  - Set up CORS headers to allow cross-origin requests.
  
- Public URL:  
  `https://python-vercel-app-mu.vercel.app/api/`

---

### 6. **Monitoring**
- Implemented logging for incoming requests and errors using Vercel's built-in monitoring tools.

---

