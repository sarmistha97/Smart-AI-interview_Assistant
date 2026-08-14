# Smart AI Interview Assistant

A lightweight AI-powered interview preparation tool that evaluates candidate responses using concept coverage analysis and transformer-based semantic similarity.

The application helps users practice technical interview questions, receive automated scoring, identify missing concepts in their answers, and improve their understanding through adaptive follow-up questions.

**Live Demo**

[Smart AI Interview Assistant Live Demo](https://smart-ai-interviewassistant-nsk4xnbyydm2xk3d4edjte.streamlit.app/?utm_source=chatgpt.com)

---

## Overview

Interview preparation often relies on manual feedback or peer review. This project provides an automated evaluation mechanism that analyzes a candidate's answer against an expected response.

Instead of relying only on keyword matching, the system combines:

* Concept coverage analysis
* Semantic similarity using transformer embeddings
* Adaptive follow-up questions based on missing concepts

This approach allows the application to evaluate both the presence of important concepts and the overall meaning of the response.

---

## Features

### Semantic Answer Evaluation

Uses Sentence Transformers to compare a candidate's answer with an ideal answer based on semantic meaning rather than exact wording.

### Concept Coverage Analysis

Checks whether important concepts expected in the answer are present and identifies missing topics.

### Adaptive Follow-up Questions

Generates follow-up questions based on uncovered concepts to encourage deeper understanding.

### Interactive Streamlit Interface

Provides a simple and user-friendly interface for practicing interview questions.

### Technical Interview Dataset

Includes structured interview questions with:

* Question text
* Difficulty level
* Key concepts
* Ideal answers
* Follow-up questions

---

## How It Works

```text
User Answer
     │
     ▼
Concept Coverage Analysis
     │
     ▼
Semantic Similarity Evaluation
     │
     ▼
Combined Score Generation
     │
     ▼
Missing Concept Detection
     │
     ▼
Adaptive Follow-up Questions
```

The final score is computed using a weighted combination of:

* Semantic similarity score
* Concept coverage score

This allows the system to evaluate both understanding and completeness.

---

## Tech Stack

### Frontend

* Streamlit

### NLP and AI

* Sentence Transformers
* all-MiniLM-L6-v2
* Transformer Embeddings

### Machine Learning

* Scikit-learn
* TF-IDF Vectorization
* Cosine Similarity

### Language

* Python

---

## Project Structure

```text
Smart-AI-Interview-Assistant/
│
├── app.py
├── main.py
├── requirements.txt
│
├── data/
│   └── questions.json
│
├── src/
│   ├── question_engine.py
│   ├── scoring.py
│   └── evaluator.py
│
└── README.md
```

---

## Installation

### Clone the Repository

```bash
git clone <repository-url>
cd Smart-AI-Interview-Assistant
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run the Application

```bash
streamlit run app.py
```

The application will launch in your browser.

---

## Requirements

```text
streamlit
sentence-transformers
scikit-learn
torch
```

---

## Example Workflow

1. Select an interview topic.
2. Read the interview question.
3. Submit your answer.
4. The system evaluates:

   * Semantic similarity
   * Concept coverage
5. Receive a score and feedback.
6. Practice follow-up questions for missed concepts.

---

## Current Limitations

* Small interview question dataset
* Rule-based concept matching
* No persistent user history
* No database integration
* No voice-based interview support
* Limited domain coverage

---

## Future Improvements

* Larger interview question bank
* Resume-based question generation
* LLM-powered feedback generation
* Voice interview support
* Adaptive difficulty progression
* Performance analytics dashboard
* User authentication and history tracking
* Multi-domain interview support
* Vector database integration
* Personalized learning recommendations

---

## Learning Outcomes

This project helped explore:

* Natural Language Processing
* Transformer Embeddings
* Semantic Similarity
* Automated Answer Evaluation
* Streamlit Application Development
* AI-Assisted Interview Preparation Systems

---

## Author

Sarmistha Gain

Computer Science Engineering Student

Silicon University, Bhubaneswar

---

## Disclaimer

This project is intended for educational and interview preparation purposes. The scoring system provides an approximation of answer quality and should not be considered a substitute for human interview evaluation.
