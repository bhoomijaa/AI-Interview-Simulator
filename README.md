# AI-Powered Interview Simulation and Evaluation System

## Overview

The traditional interview process is often inconsistent, time-consuming, and provides little to no feedback to candidates. This project aims to address these issues by building an AI-based interview system that can simulate real interview scenarios and evaluate candidate responses.

The system acts as an automated interviewer that generates personalised questions based on a candidate’s resume and evaluates their answers using predefined criteria. It provides structured feedback and an overall score to help candidates improve their performance.

## Features

- Personalised interview questions generated from the candidate’s resume and job role  
- Voice-based interaction using text-to-speech and speech recognition  
- Real-time answer evaluation using multiple criteria  
- Feedback provided for each response  
- Final score calculated based on overall performance  
- Interview results stored in JSON format for future reference  

## Evaluation Criteria

Each answer is evaluated on the following parameters:
- Relevance  
- Completeness  
- Structure  
- Specificity  
- Impact  
- Professionalism  

## Tech Stack

**Programming Language:**  
Python  

**Frontend:**  
Streamlit  

**AI and NLP:**  
Mistral LLM (via LiteLLM)  
Zero-shot and Chain-of-Thought prompting  

**Speech Processing:**  
Speechmatics (Speech-to-Text)  
Edge TTS (Text-to-Speech)  
noisereduce (noise reduction)  

**Concurrency and Performance:**  
asyncio  
ThreadPoolExecutor  
LRU Cache  

**Other Libraries:**  
PyPDF2 / pypdf  
numpy  
scipy  
pygame  

## How It Works

1. The user uploads a resume in PDF format  
2. The system extracts key information from the resume  
3. Interview questions are generated based on the resume and job description  
4. The system asks questions using text-to-speech  
5. The user responds using a microphone  
6. Audio is processed and converted to text  
7. The response is evaluated using AI  
8. The process repeats for multiple questions  
9. Final feedback and score are generated and stored

AI-Interview-System/
│
├── app.py
├── main.py
├── utils/
├── requirements.txt
├── README.md
├── schema.json
├── .env.example
└── PROJECT_SYNOPSIS.md


## Future Improvements

- Cloud deployment for multi-user access  
- Multilingual interview support  
- Video-based interview analysis  
- Employer dashboard for candidate comparison  


## Note

This project is developed as part of an academic submission. It is a local prototype and may be extended further with additional features in the future.

## Project Structure
