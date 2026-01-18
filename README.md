# 🏙️ AI Urban Planner Crew
**Powered by LangGraph + OpenAI GPT-4.1-mini**

> **Transform urban planning constraints into comprehensive city designs. Define your scenario, and watch a multi-agent AI crew generate zoning plans, infrastructure layouts, sustainability assessments, and citizen experience narratives—all in seconds.** ⚡

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![Next.js](https://img.shields.io/badge/Next.js-16-black.svg)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19.2-61DAFB.svg)](https://react.dev/)
[![LangGraph](https://img.shields.io/badge/LangGraph-AI_Agents-purple.svg)](https://langchain-ai.github.io/langgraph/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0+-blue.svg)](https://www.typescriptlang.org/)
[![MUI](https://img.shields.io/badge/MUI-6-blue.svg)](https://mui.com/)

---

## ✨ What It Does

AI Urban Planner Crew orchestrates a **five-agent LangGraph workflow** to transform high-level city planning constraints into actionable urban design:

1. **Requirements Intake** — Intelligently extracts and structures scenario parameters from free-form input
2. **Zoning Planner** — Generates comprehensive land-use allocations with density, mixed-use, and green space considerations
3. **Sustainability Scorer** — Evaluates environmental impact with A-E ratings, carbon footprint analysis, and climate resilience strategies
4. **Economic Evaluator** — Analyzes infrastructure costs, budget feasibility, revenue potential, and job creation estimates
5. **Narrative Generator** — Creates vivid, first-person citizen experience stories that bring the plan to life

All orchestrated seamlessly through a modern, responsive interface with real-time progress tracking.

---

## 🎯 Core Features

### 🤖 **AI-Powered Multi-Agent Workflow**
- **LangGraph Orchestration** — Five specialized agents working in sequence with state management
- **OpenAI GPT-4.1-mini Integration** — Optimized prompts for detailed, actionable planning outputs
- **Real-Time Progress Tracking** — Live updates as each agent completes its task
- **Context-Aware Processing** — Each agent builds upon previous outputs for coherent results

### 📊 **Comprehensive Planning Outputs**
- **Detailed Zoning Plans** — Residential, commercial, industrial, mixed-use, and green space allocations with percentages
- **Infrastructure Analysis** — Roads, utilities, public facilities with cost estimates and budget fit assessment
- **Sustainability Breakdown** — Environmental scoring, carbon footprint, green space ratios, transit accessibility
- **Citizen Narratives** — Engaging first-person stories describing daily life in the planned city

### 🎨 **Modern UI/UX**
- **State-Driven Architecture** — Smooth transitions without page reloads, showcasing React 19.2 capabilities
- **Dark/Light Mode** — Beautiful glassmorphic design with system preference detection
- **Mobile-First Responsive** — Optimized for all devices with 44px+ touch targets and bottom navigation
- **Hero Video Backgrounds** — Dynamic, theme-aware video backgrounds for immersive landing experience
- **Real-Time Visualizations** — Interactive charts and metrics dashboards

### 📱 **Enhanced Feature Set**
| Feature | Description |
|---------|-------------|
| 🎯 **Scenario Templates** | Quick-start presets (Green City, Smart City, Compact City) |
| 📈 **Plan Visualization** | Interactive charts for sustainability, budget, and density metrics |
| 💬 **AI Chat Interface** | Context-aware Q&A about your generated plans |
| 📄 **Export Functionality** | Download plans as PDF or JSON |
| 🔗 **Shareable Links** | Generate read-only share URLs for collaboration |
| 🔍 **Plan Search** | Full-text search across all saved plans |
| 📊 **Advanced Metrics** | Comprehensive analytics dashboard |
| 📋 **Plan Comparison** | Side-by-side comparison of multiple scenarios |
| 📜 **Plan History** | Complete history with version tracking |
| 🎨 **Interactive Playground** | Tabbed interface for results, visualization, and chat |

---

## 🏗️ Tech Stack

### **Frontend** ⚛️
| Technology | Purpose |
|------------|---------|
| **Next.js 16** | React 19.2 with App Router, Server Components, and optimized routing |
| **TypeScript** | Full type safety across the application |
| **MUI (Material UI) v6** | Component library with custom theme system |
| **React 19.2** | Latest React features with state-driven UI patterns |
| **Recharts** | Data visualization and interactive charts |

### **Backend** 🐍
| Technology | Purpose |
|------------|---------|
| **FastAPI** | High-performance async Python API with automatic OpenAPI docs |
| **LangGraph** | Multi-agent AI orchestration with state management |
| **OpenAI GPT-4.1-mini** | Intelligent planning analysis with optimized prompts |
| **Pydantic v2** | Data validation and serialization |
| **Python 3.11+** | Modern Python with async/await support |

### **Data & Cache** 💾
| Technology | Purpose |
|------------|---------|
| **Supabase** | PostgreSQL database with RPC functions for secure schema access |
| **Upstash Redis** | Job queue, caching, and rate limiting |

### **Deployment** 🚀
| Platform | Service |
|----------|---------|
| **Vercel** | Frontend hosting with edge optimization |
| **Railway** | Backend API with auto-scaling |

---

## 🔄 How It Works

```
┌─────────────────────────────────────────────────────────────┐
│                    USER INPUT                               │
│    Scenario: Population, Land Size, Climate, Budget         │
│         (Structured form or free-form text)                 │
└─────────────────────┬───────────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────────┐
│                 LANGGRAPH WORKFLOW                         │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐      │
│  │ Requirements │  │    Zoning     │  │Sustainability│      │
│  │    Intake    │──│   Planner     │──│    Scorer    │      │
│  │  (OpenAI)    │  │   (OpenAI)    │  │   (OpenAI)   │      │
│  └──────────────┘  └──────────────┘  └──────┬───────┘      │
│                                                │               │
│  ┌──────────────┐                    ┌────────▼────────┐      │
│  │  Economic    │                    │   Narrative      │      │
│  │ Evaluator    │────────────────────│   Generator      │      │
│  │  (OpenAI)    │                    │   (OpenAI)       │      │
│  └──────────────┘                    └────────┬────────┘      │
└───────────────────────────────────────────────┼───────────────┘
                                                │
                                                ▼
┌─────────────────────────────────────────────────────────────┐
│                       OUTPUT                                │
│  • Zoning Plan (detailed land-use allocations)              │
│  • Infrastructure Analysis (costs, budget fit)                │
│  • Sustainability Breakdown (A-E rating, metrics)            │
│  • Citizen Experience Narrative (vivid storytelling)         │
│  • Metrics (sustainability index, budget fit, density)        │
└─────────────────────────────────────────────────────────────┘
```

---

## 📸 Key Features Showcase

### 🏠 **Hero Section**
*Immersive landing experience with dynamic video backgrounds, glassmorphic design, and clear value proposition*

### 🎮 **Scenario Playground**
*Interactive planning interface with real-time progress indicators, tabbed results view, and AI chat integration*

### 📊 **Results Dashboard**
*Comprehensive plan management with search, filtering, metrics visualization, and comparison tools*

### 💬 **AI Chat Assistant**
*Context-aware conversational interface for exploring and refining your urban plans*

### 📈 **Visualization & Analytics**
*Interactive charts, metrics dashboards, and export capabilities for professional presentations*

---


## 📖 User Guide

### Getting Started

1. **Define Your Scenario** — Navigate to `/scenario` and enter:
   - Population (e.g., 50,000)
   - Land Size in km² (e.g., 100)
   - Climate (Temperate, Tropical, Arid, Cold)
   - Budget in billions (e.g., 10)
   
   Or use a **quick-start template** (Green City, Smart City, Compact City)

2. **Generate Your Plan** — Click "Generate Urban Plan" and watch the five-agent workflow execute in real-time

3. **Explore Results** — View comprehensive outputs:
   - **Zoning Plan** — Detailed land-use allocations
   - **Infrastructure** — Cost estimates and budget analysis
   - **Sustainability** — Environmental scoring and recommendations
   - **Narrative** — Citizen experience story

4. **Refine & Export** — Use the AI chat to ask questions, visualize metrics, and export as PDF or JSON

### Understanding Your Results

| Section | What It Shows |
|---------|---------------|
| **Zoning Plan** | Comprehensive land-use breakdown with percentages, density levels, and spatial organization |
| **Infrastructure** | Roads, utilities, public facilities with cost estimates and budget fit assessment |
| **Sustainability Breakdown** | A-E environmental rating, carbon footprint, green space ratios, transit accessibility |
| **Citizen Narrative** | Engaging first-person story describing daily life in the planned city |
| **Metrics** | Sustainability index, budget fit (under/at/over), density health (low/balanced/high) |

### Pro Tips

- **Use Templates** — Start with pre-configured scenarios for faster iteration
- **Free-Form Input** — Enter natural language descriptions in the playground for flexible input
- **Compare Plans** — Generate multiple scenarios and compare them side-by-side
- **Chat Integration** — Ask specific questions about your plan for deeper insights
- **Export & Share** — Download plans or generate shareable links for collaboration

---

## 🎨 Customization

### Theme Options
- ☀️ **Light Mode** — Clean, professional interface with glassmorphic effects
- 🌙 **Dark Mode** — Immersive dark theme with neon accents (default)
- 🖥️ **System** — Automatically follows OS preference

### Planning Options
- **Structured Input** — Use the scenario form for precise control
- **Free-Form Text** — Enter natural language descriptions in the playground
- **Templates** — Quick-start with pre-configured scenarios
- **Custom Constraints** — Add specific requirements via chat interface

---

## 📊 Performance

| Metric | Value |
|--------|-------|
| Plan Generation Time | ~15-30 seconds |
| Frontend Bundle Size | Optimized with Next.js 16 |
| Lighthouse Score | 90+ |
| Mobile Ready | ✅ Fully responsive |
| Real-Time Updates | Progress tracking every 750ms |
| API Response Time | < 2 seconds |

---

## 🛡️ Security & Architecture

- ✅ **Secure Schema Access** — Supabase RPC functions prevent direct schema exposure
- ✅ **Service Role Authentication** — Backend uses service_role key for database operations
- ✅ **Environment Variables** — All secrets managed via environment configuration
- ✅ **Input Validation** — Pydantic models ensure data integrity
- ✅ **CORS Protection** — Configured for production domains
- ✅ **Error Handling** — Graceful degradation with fallback content

---

## 🏗️ Architecture Highlights

### **Adapter Pattern**
- **AI Adapter** (`langgraphUrbanAdapter`) — Flexible AI framework integration
- **UI Adapter** (`planUiAdapter`) — Framework-agnostic component abstraction

### **State Management**
- React 19.2 state-driven UI with no page reloads
- Real-time progress tracking via WebSocket-like polling
- Optimistic updates for smooth user experience

### **Data Flow**
1. User input → Frontend validation
2. Frontend → Backend API (`POST /agent/run`)
3. Backend → LangGraph workflow orchestration
4. LangGraph → Five specialized agents (OpenAI-powered)
5. Results → Supabase persistence + Redis caching
6. Frontend → Real-time polling and display

### **Persistence Strategy**
- **Supabase** — PostgreSQL with `urbanplanner` schema (RPC functions for security)
- **Redis** — Job state, caching, rate limiting (prefix: `urbanplanner`)
- **Message History** — Full conversation tracking per project

---

## 👨‍💻 Creator

**Derril Filemon**  
*AI Engineer & Fullstack Developer*

📍 Goteborg, SWEDEN  
📧 +46 70 774 08 36

[![GitHub](https://img.shields.io/badge/GitHub-derril--tech-black?logo=github)](https://github.com/derril-tech)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Derril_Filemon-blue?logo=linkedin)](https://www.linkedin.com/in/derril-filemon-a31715319)

### Technical Expertise Demonstrated

This project showcases proficiency in:

- 🤖 **AI/ML Integration** — LangGraph multi-agent workflows, OpenAI GPT-4.1-mini, optimized prompt engineering
- ⚛️ **Modern React Development** — Next.js 16, React 19.2, App Router, Server Components, state-driven architecture
- 🐍 **Python Backend** — FastAPI, async/await patterns, Pydantic validation, LangChain integration
- 🎨 **UI/UX Design** — MUI theming, glassmorphic effects, responsive design, mobile-first approach
- ☁️ **Cloud Architecture** — Supabase (PostgreSQL), Upstash Redis, Railway, Vercel deployment
- 🔧 **DevOps & Tooling** — Environment management, CI/CD readiness, comprehensive testing
- 📊 **Data Visualization** — Recharts integration, interactive dashboards, metrics presentation
- 🔐 **Security Best Practices** — RPC functions, service role authentication, input validation

---

## 🙏 Acknowledgments

- **[LangGraph](https://langchain-ai.github.io/langgraph/)** — Multi-agent orchestration framework
- **[OpenAI](https://openai.com/)** — GPT-4.1-mini API for intelligent planning
- **[Supabase](https://supabase.com/)** — PostgreSQL database and RPC functions
- **[Upstash](https://upstash.com/)** — Redis caching and job queue
- **[Railway](https://railway.app/)** — Backend API deployment
- **[Vercel](https://vercel.com/)** — Frontend hosting and edge optimization
- **[MUI](https://mui.com/)** — Material UI component library
- **[Next.js](https://nextjs.org/)** — React framework with App Router

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

<div align="center">

Made with ❤️ and ☕ by [Derril Filemon](https://github.com/derril-tech)

</div>
