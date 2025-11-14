<h1>📄 <b>AI-Powered Resume Rebuilder & Job Match Analyzer</b></h1>

<p>
An end-to-end <b>Generative AI resume optimization system</b> that analyzes a candidate’s resume, extracts relevant skills, computes a job-match score, and generates a fully optimized, ATS-friendly DOCX resume using NLP, embeddings, and LLMs.
</p>

<br>

<h2>🚀 <b>Project Overview</b></h2>
<p>
This tool processes a <b>resume (PDF/DOCX)</b> and a <b>job description</b>, extracts skills, generates embeddings for similarity scoring, and rebuilds the resume using OpenAI GPT models.  
It produces a <b>clean, professional, ATS-optimized DOCX resume</b> tailored to the job.
</p>

<br>

<h2>🧠 <b>Key Features</b></h2>

<p><b>1. Resume Parsing</b><br>
• Supports PDF and DOCX formats<br>
• Uses <b>pdfplumber</b> and <b>python-docx</b> for text extraction
</p>

<p><b>2. Skill Extraction</b><br>
• Powered by <b>spaCy NLP (en_core_web_sm)</b><br>
• Extracts keywords, entities, and noun chunks
</p>

<p><b>3. Job Match Scoring</b><br>
• Uses <b>Sentence-Transformers (all-MiniLM-L6-v2)</b><br>
• Computes semantic similarity between resume and job description
</p>

<p><b>4. AI Resume Rewriting</b><br>
• Generates ATS-friendly rewritten resumes using <b>OpenAI GPT models</b><br>
• Recommended models: <b>gpt-4o</b>, <b>gpt-4o-mini</b>
</p>

<p><b>5. DOCX Resume Generator</b><br>
• Builds an organized DOCX file with clean sections:<br>
<b>SUMMARY, SKILLS, EXPERIENCE, EDUCATION</b>
</p>

<p><b>6. Automated Workflow</b><br>
Upload Resume → Paste Job Description → Extract Skills → Compute Match Score → Rebuild Resume → Download DOCX
</p>

<br>

<h2>🛠️ <b>Technologies Used</b></h2>

<p><b>Programming</b><br>
• Python<br>
• Google Colab
</p>

<p><b>AI & NLP</b><br>
• OpenAI GPT Models<br>
• Sentence-Transformers (MiniLM)<br>
• spaCy NLP
</p>

<p><b>File Parsing</b><br>
• pdfplumber<br>
• python-docx
</p>

<p><b>Utilities</b><br>
• io, os, datetime, re<br>
• Colab upload & download helpers
</p>

<br>

<h2>📥 <b>Input Types</b></h2>
<p>
• Resume File: <b>PDF / DOCX</b><br>
• Job Description: <b>Plain text</b>
</p>

<br>

<h2>📤 <b>Output Types</b></h2>
<p>
• <b>Optimized ATS-friendly DOCX Resume</b><br>
• <b>Extracted Skills List</b><br>
• <b>Job Match Score (%)</b><br>
• <b>AI-generated resume preview</b>
</p>

<br>

<h2>📚 <b>Use Cases</b></h2>
<p>
• AI-based resume optimization<br>
• Job application assistants<br>
• HR and recruiter screening tools<br>
• Resume rewriting SaaS platforms<br>
• AI-powered career support systems
</p>

<br>

<h2>🏗️ <b>System Workflow</b></h2>
<p>
1. Upload resume<br>
2. Text extracted (PDF/DOCX parsing)<br>
3. Paste job description<br>
4. NLP-based skill extraction<br>
5. Embedding similarity scoring<br>
6. AI resume rewriting<br>
7. DOCX generation & download
</p>

<br>

<h2>🎯 <b>Goal</b></h2>
<p>
To enhance resume quality, improve ATS keyword alignment, increase job match scores, and enable fast, automated, job-specific resume generation.
</p>
