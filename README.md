# Crime Scene Solver – AI-Powered Crime Scene Detection System

## Overview
Crime Scene Solver is an AI-driven system that analyzes CCTV footage to detect suspicious activities and generate human-readable incident summaries. It integrates computer vision and natural language processing to convert raw video data into structured insights.

## Features
- Detects suspicious activities from CCTV footage  
- Generates captions from video frames using CLIP  
- Removes redundant captions using Sentence-BERT (SBERT)  
- Produces concise summaries using BART (BART-MNLI)  
- Supports real-time inference using FastAPI  
- Implements secure authentication using JWT  
- Stores reports and logs using MongoDB  

## System Architecture
The system follows a modular three-tier architecture:

1. Frontend – Built using Next.js for user interaction  
2. Backend – FastAPI and Node.js for API handling and authentication  
3. AI Layer – CLIP, SBERT, and BART models for analysis and summarization  

## How It Works
1. Input CCTV video  
2. Extract frames using OpenCV  
3. Generate captions using CLIP  
4. Remove redundant captions using SBERT  
5. Summarize events using BART  
6. Store results in MongoDB  
7. Display results on dashboard  

## Tech Stack

### AI / ML
- PyTorch  
- CLIP  
- Sentence-BERT (SBERT)  
- BART (BART-MNLI)  

### Backend
- FastAPI  
- Node.js  

### Frontend
- Next.js  

### Database
- MongoDB  

### Tools and Libraries
- OpenCV  
- JWT Authentication  

## Installation and Setup

### 1. Clone the repository
```bash
git clone https://github.com/bhavyasai139/crime_scene_solver.git
cd crime_scene_solver

### 2. Install dependencies
pip install -r requirements.txt

### 3. Run backend server
uvicorn main:app --reload

### 4. Run frontend (if applicable)
cd frontend
npm install
npm run dev
