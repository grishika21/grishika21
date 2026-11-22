<!--
Replace these sections in grishika21/grishika21/README.md.
Everything not listed here (header, badges, Toolbox, Research & Patents, By the Numbers, snake) stays as is.
-->

<!-- ===================== 1) whoami block ===================== -->

```
# rishika@accenture:~$ whoami

name      : Naga Venkata Rishika Guggilam
role      : AI/ML Engineer @ Accenture
experience: 2+ years building production LLM systems, RAG pipelines & multi-agent apps
domain    : Aerospace engineering workflows
loves     : multi-agent orchestration, RAG, clean async APIs
education : B.Tech CSE, VR Siddhartha Engineering College (CGPA 9.05)
open_to   : [AI Engineer, Generative AI, Agentic AI, Backend]
```

<!-- ===================== 2) Stats (replaces 28+ / 13 / 1 / 1) ===================== -->

<table align="center">
  <tr>
    <td align="center"><h2>10</h2>AI sub-agents orchestrated</td>
    <td align="center"><h2>85%</h2>faster eBOM prep</td>
    <td align="center"><h2>~95%</h2>less lookup effort</td>
    <td align="center"><h2>1</h2>WIPO patent</td>
    <td align="center"><h2>1</h2>SCI journal paper</td>
  </tr>
</table>

<!-- ===================== 3) Things I've Built ===================== -->

## 🚀 Things I've Built

<table>
<tr>
<td width="50%" valign="top">

### 📞 [Callie](https://github.com/grishika21/callie)
**A voice support agent that answers the phone.**

Bookstore voice agent built on TalkTable (MCP), for hands-free staff queries and a customer order line.

- Plain-English questions to read-only queries over SQLite, PostgreSQL & MongoDB
- Speech in/out with faster-whisper and Piper
- Customer order phone line via Twilio
- Runs on a local LLM with Ollama

`LangChain` `MCP` `faster-whisper` `Piper` `Twilio` `Ollama`

[GitHub](https://github.com/grishika21/callie) · [Live Demo](ADD_YOUR_DEMO_LINK_HERE)

</td>
<td width="50%" valign="top">

### 🏠 Rental Agent
**An AI leasing assistant that never sleeps.**

Event-driven assistant running on a local LLM with tool calling across social channels.

- Messenger & Instagram via Meta Graph API
- Books viewings in Google Calendar
- Automatic lead tiering
- Sends property photos on request

`FastAPI` `Ollama` `Qwen3` `Tool Calling`

</td>
</tr>
</table>

<!-- ===================== 4) Journey ===================== -->

## 🛤️ Journey

<details open>
<summary><b>🟢 Full Stack LLM Development Analyst — Accenture · Jun 2026 – Present</b></summary>

- FastAPI orchestrator using Azure OpenAI tool calling, with a LangGraph sub-orchestrator for agent discovery
- Picks agents from a **live catalog**; Redis Pub/Sub auto-discovery with heartbeats means new agents plug in with **zero orchestrator changes**
- Skills framework of **8 `SKILL.md` playbooks**, so new document types ship with zero code changes
- Resumable **human-in-the-loop** workflows using LangGraph interrupts and a Redis checkpointer
- Per-user agent access from Azure B2C JWT claims, plus Azure Blob document handling; replies streamed over SSE

</details>

<details>
<summary><b>🔵 Full Stack LLM Development Associate — Accenture · Sep 2024 – May 2026</b></summary>

- **LangGraph Multi-Agent Chatbot:** Supervisor Agent routes queries by user role across 10 sub-agents (ingestion, retrieval, STE validation, authoring) with RBAC and human-in-the-loop, cutting manual tool switching by **40%**
- **KB Ingestion & Extraction Agents:** turn manuals and spreadsheets (including scanned PDFs) into a searchable knowledge base; answers engineers' questions in ~1 min with sources, cutting lookup effort by **~95%**
- **eBOM Agent:** Azure OpenAI agent that turns Teamcenter, SAP or JSON parts data into a validated Teamcenter-ready BOM with a gap report, using a 7-stage pipeline and MCP sub-agents, cutting prep time by **85%**
- **Process Instruction Agent:** page-indexed PDF/DOCX extraction with no vector DB, avoiding retrieval drift
- **STE Validator:** re-engineered the ASD-STE100 Simplified Technical English validator with spaCy, cutting false positives by **30%**
- **Illustration Comparison:** mapped CGM callouts to procedure steps for automated aircraft authoring

</details>

<details>
<summary><b>⚪ Computer Vision Intern — Accenture · Feb 2024 – Jun 2024</b></summary>

- Illustration comparison pipeline with SAM segmentation, VGG features and Mistral LLM analysis for aerospace documentation

</details>
