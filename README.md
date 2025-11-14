<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>AI-Powered Resume Rebuilder & Job Match Analyzer</title>

  <!-- Simple, professional styling -->
  <style>
    :root{
      --bg:#ffffff;
      --muted:#6b7280;
      --accent:#0f172a;
      --card:#f8fafc;
      --heading: 24px;
      --subheading:18px;
      --body:16px;
      --mono: "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace;
      --sans: "Inter", system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }

    html,body{
      height:100%;
      margin:0;
      background:linear-gradient(180deg, #fbfdff 0%, #ffffff 100%);
      color:var(--accent);
      font-family:var(--sans);
      line-height:1.6;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
    }

    .container{
      max-width:900px;
      margin:36px auto;
      padding:28px;
      background:var(--card);
      border-radius:12px;
      box-shadow: 0 6px 18px rgba(15,23,42,0.06);
      border:1px solid rgba(15,23,42,0.04);
    }

    header{
      display:flex;
      align-items:flex-start;
      gap:18px;
      margin-bottom:18px;
    }

    header h1{
      font-size:32px;
      margin:0 0 6px 0;
      letter-spacing:-0.2px;
    }

    header p.lead{
      margin:0;
      color:var(--muted);
      font-size:var(--body);
    }

    .meta{
      display:flex;
      gap:12px;
      margin-top:8px;
      color:var(--muted);
      font-size:14px;
    }

    section{
      margin-top:20px;
    }

    h2{
      font-size:var(--subheading);
      margin:0 0 10px 0;
      color:var(--accent);
    }

    h3{
      font-size:16px;
      margin:0 0 8px 0;
      color:var(--accent);
    }

    p{ margin:0 0 10px 0; color:#0b1220; font-size:var(--body); }

    ul { margin:8px 0 12px 20px; }
    li { margin:6px 0; }

    .two-col{
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap:18px;
    }

    pre.code{
      background:#0b1220;
      color:#e6eef8;
      padding:14px;
      border-radius:8px;
      overflow:auto;
      font-family:var(--mono);
      font-size:13px;
      margin:10px 0;
    }

    .badge{
      display:inline-block;
      padding:6px 10px;
      font-size:13px;
      background:#eef2ff;
      color:#1e293b;
      border-radius:8px;
      margin-right:6px;
    }

    footer{
      margin-top:26px;
      padding-top:12px;
      border-top:1px solid rgba(15,23,42,0.04);
      color:var(--muted);
      font-size:14px;
    }

    /* Responsive */
    @media (max-width:720px){
      .two-col{ grid-template-columns: 1fr; }
      header{ flex-direction:column; align-items:flex-start; }
    }
  </style>
</head>
<body>
  <div class="container" role="main">
    <header>
      <div>
        <h1>AI-Powered Resume Rebuilder & Job Match Analyzer</h1>
        <p class="lead">End-to-end Generative AI system to analyze, score, and rewrite resumes into ATS-friendly DOCX output.</p>
        <div class="meta">
          <span class="badge">Python</span>
          <span class="badge">OpenAI GPT</span>
          <span class="badge">spaCy</span>
          <span class="badge">Sentence-Transformers</span>
        </div>
      </div>
    </header>

    <section aria-labelledby="overview">
      <h2 id="overview">🚀 Project Overview</h2>
      <p>
        The system accepts a <strong>resume (PDF or DOCX)</strong> and a <strong>job description</strong>, extracts skills and text, computes semantic similarity using embeddings, and rewrites the resume using OpenAI GPT models. The final output is a professionally formatted, ATS-optimized DOCX resume.
      </p>
    </section>

    <section aria-labelledby="features">
      <h2 id="features">🧠 Key Features</h2>
      <div class="two-col">
        <div>
          <h3>Resume Parsing</h3>
          <p>Reliable PDF/DOCX parsing with <code>pdfplumber</code> and <code>python-docx</code> to extract text and structure.</p>

          <h3>Skill Extraction</h3>
          <p>spaCy NLP (<code>en_core_web_sm</code>) extracts noun chunks, named entities, and domain keywords.</p>

          <h3>Job Match Scoring</h3>
          <p>Sentence-Transformers (<code>all-MiniLM-L6-v2</code>) produces embeddings to compute a job-fit similarity score.</p>
        </div>

        <div>
          <h3>AI Resume Rewriting</h3>
          <p>Generates ATS-optimized sections (SUMMARY, SKILLS, EXPERIENCE, EDUCATION) using OpenAI GPT models (recommended: <code>gpt-4o</code>, <code>gpt-4o-mini</code>).</p>

          <h3>DOCX Resume Generator</h3>
          <p>Creates a clean, downloadable DOCX with consistent headings and bullet formatting suitable for ATS ingestion.</p>

          <h3>Automated Workflow</h3>
          <p>Upload → Extract → Score → Rewrite → Download. Minimal user interaction for fast job-specific resume customization.</p>
        </div>
      </div>
    </section>

    <section aria-labelledby="tech">
      <h2 id="tech">🛠️ Technologies Used</h2>
      <ul>
        <li><strong>Programming:</strong> Python, Google Colab</li>
        <li><strong>AI & NLP:</strong> OpenAI GPT (gpt-4o / gpt-4o-mini), Sentence-Transformers (MiniLM), spaCy</li>
        <li><strong>File Parsing:</strong> pdfplumber, python-docx</li>
        <li><strong>Utilities:</strong> io, os, datetime, re; Colab upload/download helpers</li>
      </ul>
    </section>

    <section aria-labelledby="io">
      <h2 id="io">📥 Inputs & 📤 Outputs</h2>
      <div class="two-col">
        <div>
          <h3>Inputs</h3>
          <ul>
            <li>Resume file (PDF or DOCX)</li>
            <li>Job description (plain text)</li>
          </ul>
        </div>
        <div>
          <h3>Outputs</h3>
          <ul>
            <li>Optimized DOCX resume (ATS-friendly, clean headings)</li>
            <li>Extracted skills list</li>
            <li>Job match score (%)</li>
            <li>Formatted AI-generated resume preview</li>
          </ul>
        </div>
      </div>
    </section>

    <section aria-labelledby="workflow">
      <h2 id="workflow">🏗️ System Workflow</h2>
      <ol>
        <li>Upload resume → text extracted (PDF/DOCX parsing)</li>
        <li>Paste job description</li>
        <li>Extract skills via spaCy NLP</li>
        <li>Generate embeddings & compute similarity score</li>
        <li>Rewrite resume with OpenAI GPT</li>
        <li>Create downloadable DOCX resume</li>
      </ol>
    </section>

    <section aria-labelledby="usecases">
      <h2 id="usecases">📚 Use Cases</h2>
      <p>Automated resume optimization, HR/recruiter screening tools, job application assistants, AI career support platforms, and resume-rewriting SaaS offerings.</p>
    </section>

    <section aria-labelledby="goal">
      <h2 id="goal">🎯 Goal</h2>
      <p>Improve resume quality, optimize keyword alignment for ATS systems, enhance job-match relevance, and streamline job-specific resume customization.</p>
    </section>

    <footer>
      <p>For setup instructions, examples, and code, add a <code>README.md</code> and script samples to your repository. Want a downloadable HTML or PDF version styled differently? Ask and I’ll generate it.</p>
    </footer>
  </div>
</body>
</html>
