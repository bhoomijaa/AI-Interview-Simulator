# AI-Interview-Simulator
An intelligent, voice-based mock interview platform that simulates real interview experiences and provides structured feedback using AI.

 **Overview**

Interviews are stressful, inconsistent, and often lack useful feedback. This project was built to solve exactly that.

The system acts as an AI interviewer that:

Generates personalised questions based on your resume
Conducts the interview via voice interaction
Evaluates your answers across multiple criteria
Provides detailed feedback and an overall score

The goal is simple: help candidates practise better and reduce bias in evaluation

✨ Key Features
**Personalised Questions**
Questions are dynamically generated based on your resume and job role — no fixed templates.
**Voice-Based Interaction**
The AI asks questions using text-to-speech, and you respond using your microphone.
**AI Evaluation System**
Each answer is scored on:
Relevance
Completeness
Structure
Specificity
Impact
Professionalism
**Real-Time Processing**
Question generation and answer evaluation run simultaneously to reduce waiting time.
**Noise Reduction + Speech Recognition**
Audio is cleaned before transcription to improve accuracy.
**Detailed Feedback + Final Score**
You get per-question feedback along with an overall performance score.

**System Architecture**

The system follows a layered approach:

Frontend (Streamlit) – interactive UI
State Management (FSM) – controls interview flow
AI Layer (LLM) – generates and evaluates content
Speech Layer – handles audio input/output
Data Layer – stores results in JSON
🛠️ Tech Stack

Core:

Python
Streamlit

AI / NLP:

Mistral LLM (via LiteLLM)
Chain-of-Thought Prompting
Zero-shot prompting

Speech Processing:

Speechmatics (ASR)
Edge TTS (Text-to-Speech)
noisereduce (audio cleaning)

Performance:

asyncio (concurrency)
ThreadPoolExecutor
LRU Cache
**How It Works**
Upload your resume (PDF)
System extracts key information
AI generates personalised questions
Questions are spoken aloud
You answer via microphone
Audio is processed and transcribed
AI evaluates your response
Process repeats for multiple questions
Final score + feedback is generated and saved
**Output**
Structured interview results stored as JSON
Includes:
Questions & answers
Scores
Feedback
Final evaluation
**Future Improvements**
Cloud deployment (multi-user support)
Video + facial expression analysis
Multilingual interviews
Employer dashboard for candidate comparison
**Impact**
Helps candidates practise anytime
Provides structured, unbiased feedback
Reduces dependency on human interviewers
Makes interview prep more accessible
