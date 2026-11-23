%-------------------------------------------------------------
% Resume - Naga Venkata Rishika Guggilam
% Layout matched to Akhil Babu Nambur's resume
% (black text, blue links, Computer Modern, A4)
% Compile on Overleaf with pdfLaTeX
%-------------------------------------------------------------
\documentclass[a4paper,10pt]{article}

\usepackage[margin=0.5in]{geometry}
\usepackage[T1]{fontenc}
\usepackage{lmodern}
\usepackage{titlesec}
\usepackage{enumitem}
\usepackage[colorlinks=true,urlcolor=blue,linkcolor=blue]{hyperref}
\usepackage{xcolor}
\usepackage{tabularx}
\usepackage{amssymb}
\usepackage{needspace}

\pagestyle{empty}
\setlength{\parindent}{0pt}
\raggedright
\input{glyphtounicode}
\pdfgentounicode=1   % ATS-friendly (machine-readable text)

% ---------- Section headings: bold, uppercase, full-width rule ----------
\titleformat{\section}
  {\large\bfseries}{}{0em}{\MakeUppercase}[\vspace{-6pt}\rule{\linewidth}{0.6pt}]
\titlespacing*{\section}{0pt}{8pt}{5pt}

% ---------- Custom commands ----------
\newcommand{\company}[2]{%
  \begin{tabularx}{\linewidth}{@{}X r@{}}\textbf{#1} & #2 \\\end{tabularx}\vspace{-3pt}\par}
\newcommand{\role}[2]{%
  \begin{tabularx}{\linewidth}{@{}X r@{}}\textit{#1} & \textit{#2} \\\end{tabularx}\vspace{-2pt}\par}

% Role line like the reference: Bold Role | Company, Location ........ Dates
\newcommand{\roleline}[3]{\vspace{3pt}%
  \noindent{\large\bfseries #1}\ \textbar\ #2\hfill #3\par\vspace{1pt}}

% Education: {College}{Location}{Degree}{Dates}
\newcommand{\entry}[4]{%
  \begin{tabularx}{\linewidth}{@{}X r@{}}
    \textbf{#1} & #2 \\
    \textit{#3} & #4 \\
  \end{tabularx}\vspace{-4pt}%
}

% Sub-heading (bold line above bullets)
\newcommand{\subhead}[1]{\vspace{3pt}\textbf{#1}\par\vspace{-1pt}}

% List settings
\setlist[itemize,1]{leftmargin=10pt, itemsep=1.5pt, topsep=2pt, parsep=0pt, label=\textbullet}

\begin{document}

%-------------------- HEADER --------------------
\begin{center}
  {\fontsize{23}{27}\selectfont\bfseries NAGA VENKATA RISHIKA GUGGILAM}\\[4pt]
  {\fontsize{8.3}{10}\selectfont\bfseries AI/ML ENGINEER --- AGENTIC AI --- GENERATIVE AI --- NLP --- DEEP LEARNING --- COMPUTER VISION}\\[5pt]
  \small
  +91 99084 37637 \ --- \
  \href{mailto:rishikag2102@gmail.com}{rishikag2102@gmail.com} \ --- \
  \href{https://linkedin.com/in/rishika-guggilam}{linkedin.com/in/rishika-guggilam} \ --- \
  \href{https://github.com/rishikag21}{github.com/rishikag21}
\end{center}
\vspace{-6pt}

%-------------------- SUMMARY --------------------
\section{Professional Summary}
AI/ML Engineer with 2+ years at Accenture building production LLM systems, RAG pipelines, multi-agent applications, NLP solutions, and computer vision. Skilled in Python, FastAPI, LangChain, and LangGraph. Automated engineering workflows and deployed enterprise AI. SCI-indexed journal author and WIPO-published patent holder.

%-------------------- EXPERIENCE --------------------
\section{Professional Experience}

\roleline{Full Stack LLM Development Analyst}{Accenture, Bengaluru, India}{Jun 2026 -- Present}
\begin{itemize}
  \item Built a FastAPI orchestrator (Azure OpenAI tool calling) with a LangGraph sub-orchestrator for agent discovery.
  \item Created a skills framework of 8 SKILL.md playbooks; new document types ship with zero code changes.
  \item Implemented resumable human-in-the-loop workflows with LangGraph interrupts and a Redis checkpointer.
\end{itemize}

\vspace{1pt}
\roleline{Full Stack LLM Development Associate}{Accenture, Bengaluru, India}{Sep 2024 -- May 2026}
\begin{itemize}
  \item Developed a LangChain/LangGraph multi-agent chatbot whose Supervisor Agent routes queries by user role across 10 sub-agents for ingestion, retrieval, STE validation, and authoring, cutting manual tool switching by 40\%.
  \item Built the KB Ingestion and Extraction agents, which turn manuals and spreadsheets (incl. scanned PDFs) into a searchable knowledge base and answer engineers' questions in $\sim$1 min with sources, cutting lookup effort by $\sim$95\%.
  \item Built an Azure OpenAI eBOM agent that turns Teamcenter, SAP or JSON parts data into a validated Teamcenter-ready BOM with a gap report, using a 7-stage pipeline and MCP sub-agents, cutting prep time by 85\%.
  \item Re-engineered the ASD-STE100 Simplified Technical English validator with spaCy, cutting false positives by 30\%.
\end{itemize}

\vspace{1pt}
\roleline{Computer Vision Intern}{Accenture, Bengaluru, India}{Feb 2024 -- Jun 2024}
\begin{itemize}
  \item Built an illustration comparison pipeline with SAM segmentation, VGG features, and Mistral LLM analysis.
\end{itemize}

%-------------------- PROJECTS --------------------
\Needspace{8\baselineskip}
\section{Projects}
\subhead{Callie --- Voice Support Agent on TalkTable (MCP) \textnormal{|} \href{https://github.com/grishika21/talktable}{GitHub} \textnormal{|} \href{https://callie-demo.streamlit.app/}{Live Demo}}
\begin{itemize}
  \item Built Callie, a bookstore voice agent with LangChain, MCP, faster-whisper, Piper, Twilio and local Ollama, for hands-free staff queries and a customer order phone line.
  \item Built TalkTable underneath: plain-English questions to read-only queries over SQLite, PostgreSQL, MongoDB.
\end{itemize}

%-------------------- PUBLICATIONS --------------------
\section{Publication \& Patent}
\begin{itemize}
  \item \textbf{Publication:} ``An expert system for privacy-preserving vessel detection leveraging optimized Extended-YOLOv7 and SHA-256,'' \href{https://www.sciencedirect.com/science/article/pii/S1084804525000360}{\textit{J. Netw. Comput. Appl.}}, Vol.~238, 2025. Trained and optimized Extended-YOLOv7 (CSPNet, SPP, NMS) with gradient descent: 9.3\% precision gain over YOLOv7.
  \item \textbf{Patent:} ``Ornithopter Unmanned Remote Control Aerial Vehicle for Intruder Detection and Data Preservation,'' -- WO2025032370, WIPO, 2025.
\end{itemize}

%-------------------- SKILLS --------------------
\section{Technical Skills}
\begin{itemize}
  \item \textbf{Generative AI \& LLMs:} Prompt Engineering, RAG, Tool Calling, LLM Evaluation, Ollama
  \item \textbf{Agentic AI:} Multi-Agent Systems, Supervisor Agents, MCP, A2A, Human-in-the-Loop, Runtime Discovery
  \item \textbf{AI/ML \& NLP:} PyTorch, TensorFlow, Hugging Face, Deep Learning, Model Training, NLP, NLU, Semantic Search, spaCy, Sentence Transformers, Computer Vision, Vector Databases
  \item \textbf{Languages \& Frameworks:} Python, Java, SQL, LangChain, LangGraph, FastAPI, Flask, Pydantic
  \item \textbf{Databases \& Data:} PostgreSQL, MongoDB, SQLite, Redis, Qdrant, SQLAlchemy, sqlglot, NetworkX
  \item \textbf{Cloud \& DevOps:} Azure (OpenAI, AI Search, Blob, B2C), Docker, Git, Linux, REST APIs, SSE, Twilio
  \item \textbf{Security \& Auth:} JWT, OAuth 2.0, RBAC, Input Validation, Read-Only SQL Controls
\end{itemize}

%-------------------- EDUCATION --------------------
\section{Education}
\entry{VR Siddhartha Engineering College}{Vijayawada, Andhra Pradesh}{B.Tech in Computer Science and Engineering --- CGPA: 9.05/10}{2020 -- 2024}

\end{document}
