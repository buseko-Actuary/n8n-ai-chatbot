# Development Log

A running, dated log of daily improvements to this project. Newest entries at the top.
Each daily automated session appends one entry here describing the single improvement it made,
so future sessions can see what has already been done and avoid repeating it.

---

### 2026-07-24 — Tightened the agent's system prompt
- Removed em dashes from the AI Agent's system prompt (`workflow/ai-agent-lead-capture.json`) to match the Insight Analytics brand voice rule against them, replacing them with periods or commas.
- Added explicit criteria for classifying a lead's `buyer_type` as "serious" versus "casual" (budget, timeline, team/business size, or a direct request to book a call). Previously the Code Tool expected this field but the agent was never told how to decide it, so classification was inconsistent.
- Added email to the list of details the agent should always try to capture, matching what the Code Tool already extracts.
- Tightened the reply-length guidance from "2-4 sentences" to "2-3 sentences" for a warmer, more WhatsApp-like feel, per the idea logged yesterday.
- No structural changes to the workflow, only the system prompt text. Still worth a quick read-through in n8n before the next live conversation, but low risk.
- **Ideas not yet done (candidates for future days):** WhatsApp channel integration, a RAG/knowledge-base tool so the agent answers from real service docs, a team notification when a serious lead is captured, follow-up messages for quiet leads, multi-language support (including local Zambian languages), example conversations in the docs, an architecture diagram image, stricter email format validation (currently just a regex match, no rejection of malformed addresses), and a small analytics view on the leads sheet.

### 2026-07-23 — Project published and evolved
- Published the repository to GitHub.
- Added the "First Chatbot" (v1) and the full "AI Agent" (v2) workflows.
- Wrote the README story and set up this development log plus the changelog.
- **Ideas not yet done (candidates for future days):** WhatsApp channel integration, a RAG/knowledge-base tool so the agent answers from real service docs, a team notification when a serious lead is captured, follow-up messages for quiet leads, multi-language support (including local Zambian languages), tightening the system prompt for shorter and warmer replies, adding example conversations to the docs, an architecture diagram image, input validation on captured emails, and a small analytics view on the leads sheet.
