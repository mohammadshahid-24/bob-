# ⚖️ Legal Aid Multi-Agent System

A React + TypeScript application simulating a multi-agent AI system for legal aid case management. Five specialized AI agents collaborate to process legal cases through an automated workflow.

## 🤖 Agents

| Agent | Name | Role |
|-------|------|------|
| Supervisor | Alex Chen | Oversees all cases, coordinates agents, ensures quality |
| Intake Specialist | Maya Rodriguez | Client interviews, eligibility, case classification |
| Legal Researcher | James Okafor | Statutory research, case law, precedent analysis |
| Legal Strategist | Priya Sharma | Strategy formulation, risk assessment, options evaluation |
| Documentation | David Walsh | Legal drafting, court filings, document management |

## 🚀 Quick Start

```bash
npm install
npm start
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## 🏗️ Architecture

```
src/
├── types/          # TypeScript interfaces (agents, cases, messages)
├── data/           # Agent definitions, sample cases
├── services/       # Agent response engine, workflow orchestration
├── context/        # React Context + useReducer state management
└── components/
    ├── CaseManager.tsx     # Left sidebar: case list + new case form
    ├── ChatInterface.tsx   # Center: message thread + workflow controls
    ├── AgentPanel.tsx      # Right sidebar: agent cards + workflow progress
    ├── AgentCard.tsx       # Individual agent status card
    └── MessageBubble.tsx   # Chat message renderer with Markdown support
```

## ✨ Features

- **Multi-agent workflow**: Intake → Research → Strategy → Documentation → Supervisor
- **5 sample cases** across housing, employment, family, immigration, and benefits law
- **Live agent status indicators** (Idle, Thinking, Responding, Done)
- **Workflow progress tracker** with step-by-step visualization
- **Case creation form** — add your own cases with custom details
- **Chat interface** — send messages to agents or run the full automated workflow
- **Rich message rendering** — Markdown, tables, bullet points, handoff notices
- **Stop workflow** at any time

## 🛠️ Tech Stack

- **React 18** with TypeScript
- **React Context + useReducer** for state management
- **CSS-in-JS** (inline styles) — zero external CSS dependencies
- **uuid** for unique IDs

## 📋 Legal Areas Supported

Housing, Family Law, Employment, Immigration, Criminal Defense, Consumer Protection, Civil Rights, Government Benefits
