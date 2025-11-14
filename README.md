                                                          AI-Powered Resume Rebuilder & Job Match Analyzer
AI-powered resume optimizer that parses PDF/DOCX resumes, extracts skills, analyzes job match using embeddings, and generates an ATS-friendly rewritten resume using OpenAI GPT models. Includes job similarity scoring, skill extraction, and DOCX output generation
Project Overview

The system takes a resume (PDF or DOCX) and a job description as input, extracts key skills, computes a job-match score using sentence embeddings, and rebuilds the resume using OpenAI GPT models. It outputs a professionally rewritten DOCX resume tailored to the job description.

🧠 Key Features

Resume Parsing
Parses resumes in PDF or DOCX format using pdfplumber and python-docx.

Skill Extraction
Uses spaCy NLP (en_core_web_sm) to extract relevant skills, entities, and keywords.

Job Match Scoring
Computes similarity between the resume and the job description using Sentence-Transformers (all-MiniLM-L6-v2) for embeddings.

AI Resume Rewriting
Generates an ATS-optimized resume using OpenAI GPT models (recommended: gpt-4o or gpt-4o-mini).

DOCX Resume Generator
Creates a clean, organized, downloadable DOCX file with sections like SUMMARY, SKILLS, EXPERIENCE, and EDUCATION.

Automated Workflow
Users upload a resume → paste job description → get enhanced resume + skill list + similarity score.

🛠️ Technologies Used
Programming

Python

Google Colab environment

AI & NLP

OpenAI GPT Models (gpt-4o, gpt-4o-mini)

Sentence-Transformers (MiniLM)

spaCy NLP (noun chunks, entity extraction)

File Parsing

pdfplumber — PDF text extraction

python-docx — DOCX reading & writing

Utilities

io, os, datetime, re for file processing

Google Colab file upload/download helpers

📥 Input Types

Resume File (PDF or DOCX)

Job Description (plain text)

📤 Output Types

Optimized Resume (DOCX)

ATS-friendly

Clean headings

Tailored to job description

Extracted Skills List

Job Match Score (%)

Formatted AI-generated resume preview

📚 Use Cases

Automated resume optimization

HR/recruiter screening tools

Job application assistants

AI career support platforms

Resume rewriting SaaS products

🏗️ System Workflow

Upload resume → text extracted

Paste job description

Extract skills with NLP

Generate embeddings & compute similarity score

Rewrite resume with GPT

Create downloadable DOCX resume

🎯 Goal

Improve resume quality, optimize keyword alignment for ATS systems, enhance chances of job selection, and streamline job-specific resume customization.
