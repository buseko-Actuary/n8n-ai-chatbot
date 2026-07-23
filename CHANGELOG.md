# Changelog

All notable changes to this project are documented here.
The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]
### Changed
- Tightened the AI Agent's system prompt (`workflow/ai-agent-lead-capture.json`): removed em dashes to match brand voice guidelines, added explicit criteria for classifying `buyer_type` as serious vs. casual, added email to the fields the agent always tries to capture, and shortened the target reply length for a warmer, chat-like feel.

## [0.2.0] - 2026-07-23
### Added
- Full AI agent workflow (`workflow/ai-agent-lead-capture.json`): OpenAI chat model, rolling conversation memory, a JavaScript code tool for structured lead extraction, Google Sheets lead logging, and Google Calendar meeting booking.
- Screenshot of the agent canvas (`assets/ai-agent-canvas.png`).
- README section on the chatbot-to-agent evolution and the impact for Zambian SMEs.

### Security
- Sanitized private data before publishing: personal calendar email, live Google Sheet ID, and credential IDs replaced with placeholders. Cropped the agent screenshot to remove a customer's contact details.

## [0.1.0] - 2026-07-23
### Added
- Initial "First Chatbot" workflow (`workflow/first-chatbot.json`): a two-node n8n chat assistant backed by an OpenAI model with an on-brand system prompt.
- Screenshot of the first chatbot running (`assets/chatbot-canvas.png`).
- Professional README, MIT license, and `.gitignore`.
