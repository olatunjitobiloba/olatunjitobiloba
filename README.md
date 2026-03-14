<div align="center">

![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=2F81F7&center=true&vCenter=true&width=600&lines=ML+%26+Backend+Engineer;Building+Production+AI+Systems;Fintech+Infrastructure+%7C+Privacy-Preserving+AI)

</div>

---

# Olatunji Oluwatobiloba Franklin

**ML & Backend Engineer — Building production AI systems and fintech infrastructure.**  
Computer Engineering student @ Covenant University.

I build machine learning systems that run in production — not just notebooks.  
Clean code. Tested. Documented. Deployed.

**Focus areas:** ML inference infrastructure · Fintech backend systems · Behavioral analytics · Privacy-preserving AI

---

## Live Systems

| System | Description | Status |
|--------|-------------|--------|
| [Loan Prediction API](https://loan-predictor-api-91xu.onrender.com/app) | Production ML inference — 88.6% accuracy | Live |
| [FocusPilot](https://huggingface.co/spaces) | Behavioral analytics + autonomous ML agent | Live |
| [FedRec](https://lnkd.in/d54eeeDc) | Federated recommendation engine — 9.5/10 privacy score | Live |

---

## Flagship Systems

### AI Loan Prediction System

Production ML system predicting loan approval risk with 88.62% accuracy.  
4 models benchmarked. REST API with caching, validation, logging, and full test coverage.

**System Architecture**

```
Client Request
     |
REST API (Flask)
     |
Input Validation & Feature Pipeline
     |
ML Model Inference (4 models benchmarked)
     |
Response Caching Layer (3-4x faster)
     |
PostgreSQL Prediction Logging
     |
JSON Response + Confidence Score
```

**Engineering Signals**
- 4 ML models benchmarked: Random Forest, Gradient Boosting, Logistic Regression, SVM
- 83% test coverage with pytest
- REST API with input validation + Swagger/OpenAPI docs
- Rate limiting + response caching
- Deployed to production on Render

`Python` `Flask` `scikit-learn` `PostgreSQL` `pytest` `Swagger` `Render`

---

### FocusPilot — Behavioral Analytics & Autonomous Agent System

Chrome extension + ML pipeline that detects distraction patterns in real-time and intervenes  
autonomously using reinforcement learning.

**System Architecture**

```
Chrome Extension (MV3)
     |
Activity Tracker (tabs, idle time, domains)
     |
FastAPI Backend (HF Spaces)
     |
Feature Engineering Pipeline (15 behavioral features)
     |
Procrastination Predictor (Random Forest)
     |
Autonomous Agent (Monitor -> Decide -> Execute -> Learn)
     |
Supabase (PostgreSQL + Real-time)
     |
React Dashboard (Vercel)
```

**Engineering Signals**
- 15-feature behavioral ML pipeline (temporal, behavioral, historical, contextual)
- Multi-agent architecture: Monitoring, Decision, Execution, Learning agents
- Real-time Supabase subscriptions for agent state management
- ML distraction scorer with 4-factor weighted algorithm
- Chrome Extension Manifest V3 with declarativeNetRequest blocking

`FastAPI` `React` `TypeScript` `Supabase` `scikit-learn` `Chrome Extension API` `Vercel` `HF Spaces`

---

### FedRec — Privacy-Preserving Federated Recommendation Engine

Federated learning system that personalizes recommendations across devices  
without centralizing raw user data. 34% engagement boost. Zero privacy violations.

**System Architecture**

```
Device 1 ... Device N  (local training — no raw data shared)
     |              |
Local Model Updates (encrypted weights only)
     |
FedAvg Aggregation Server
     |
Global Model Update
     |
Streamlit Dashboard
(Privacy Meter · Performance Tracker · Business Impact Calculator)
```

**Engineering Signals**
- FedAvg algorithm — no raw data leaves devices
- Scalable to 1M+ simulated devices
- 9.5/10 privacy score · 34% accuracy boost · $15M+ revenue protection modeled
- Multi-domain datasets: MovieLens, Amazon Reviews, Spotify-like music data

`Python` `PyTorch` `TensorFlow` `Streamlit` `scikit-learn` `Federated Learning`

---

## How I Build Production Systems

Most ML projects stop at notebooks. I focus on shipping systems that run in production.

Typical architecture I build:

```
Client
  |
REST API (input validation + rate limiting)
  |
Feature Engineering Pipeline
  |
Model Inference (benchmarked, versioned)
  |
Caching Layer
  |
Database Logging (predictions + metadata)
  |
JSON Response + Confidence Score
```

Engineering principles I follow:
- Separate training pipelines from inference services
- Validate inputs before model inference
- Benchmark multiple models before selecting one
- Log predictions for retraining pipelines
- Cache responses to reduce compute cost
- Document APIs with OpenAPI / Swagger

---

## Core Engineering Skills

```
Machine Learning     Python · scikit-learn · TensorFlow · PyTorch · feature engineering · model serving
Backend Systems      FastAPI · Flask · REST APIs · PostgreSQL · SQLite · Supabase
Data Engineering     Pandas · NumPy · data pipelines · behavioral analytics
DevOps & Testing     Docker · GitHub Actions · pytest · CI/CD · Render · Vercel
Frontend             React · TypeScript · Tailwind CSS · Recharts
Browser Engineering  Chrome Extension API · Manifest V3 · declarativeNetRequest
```

---

## System Design Interests

- Payment systems and fraud detection pipelines
- ML inference infrastructure at scale
- Behavioral analytics platforms
- Privacy-preserving AI (federated learning, differential privacy)
- Real-time event-driven architectures

---

## Currently Building

```python
current_focus = {
    "focuspilot":    "Behavioral analytics system with autonomous ML agent",
    "ml_inference":  "Serving models through production APIs at scale",
    "system_design": "Building scalable fintech backend architectures",
}

for system, description in current_focus.items():
    print(f"[{system}] -> {description}")
```

---

## Achievements

- 2nd Place — IoT Engineering Competition
- Published technical writer on Medium
- Multiple ML systems in production (deployed, tested, documented)
- High academic performance @ Covenant University

---

## Philosophy

"Calling is greater than comfort. Impact over titles. Execution over excuses."

I build systems that work in production — not just notebooks.

---

## Connect

[LinkedIn](https://linkedin.com/in/olatunji-oluwatobiloba-186659291) · 
[Portfolio](https://olatunjitobiloba.vercel.app) · 
[Email](mailto:olatunjitobiloba@gmail.com)
