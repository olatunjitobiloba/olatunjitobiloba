<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=3B82F6&center=true&vCenter=true&width=700&lines=ML+%26+Backend+Engineer;Building+Production+AI+Systems;Fintech+Infrastructure+%7C+Privacy-Preserving+AI;I+build+systems+that+run+in+production)](https://git.io/typing-svg)

</div>

---

# Olatunji Oluwatobiloba Franklin

ML and Backend Engineer. Building production AI systems and fintech infrastructure.
Computer Engineering student at Covenant University.

I build machine learning systems that run in production — not just notebooks.
Clean code. Tested. Documented. Deployed.

[LinkedIn](https://linkedin.com/in/olatunji-oluwatobiloba-186659291) &nbsp;|&nbsp;
[Email](mailto:olatunjifranklin@email.com) &nbsp;|&nbsp;
[Portfolio](https://github.com/olatunjitobiloba)

---

## Live Systems

| System | Description | Status |
|--------|-------------|--------|
| Loan Prediction API | ML inference API — 88.6% accuracy | [Live](https://loan-predictor-api-91xu.onrender.com/app) |
| FocusPilot Dashboard | Behavioral analytics platform | [Live](https://focuspilot.vercel.app) |
| FedRec Engine | Federated recommendation system | [Live](https://OlatunjiTobi-focuspilot-agent.hf.space) |

---

## Flagship Systems

### AI Loan Prediction System

Production ML inference system predicting loan approval risk with 88.62% accuracy.
Four models benchmarked, REST API with caching, rate limiting, and PostgreSQL logging.

**System Architecture**

```
Client Request
     |
Flask REST API
     |
Input Validation + Feature Pipeline
     |
Model Benchmarking (RF, GBM, LR, SVM)
     |
Prediction + Confidence Score
     |
Response Caching Layer  (3-4x faster)
     |
PostgreSQL Prediction Logging
     |
JSON Response
```

**Example Request**

```bash
curl -X POST https://loan-predictor-api-91xu.onrender.com/predict \
-H "Content-Type: application/json" \
-d '{
  "income": 50000,
  "credit_score": 720,
  "loan_amount": 15000,
  "employment_years": 5
}'
```

**Example Response**

```json
{
  "loan_approval_probability": 0.87,
  "risk_level": "LOW",
  "model_used": "RandomForest",
  "confidence_score": 0.91
}
```

**Engineering Decisions**

- Why multiple models? Benchmarking RF, GBM, LR, and SVM allowed selecting the best bias-variance tradeoff before deployment.
- Why caching? Prediction caching reduced repeated inference cost and improved response time by 3-4x.
- Why PostgreSQL logging? Prediction logs enable future retraining pipelines and drift monitoring.

**Stack:** Python · Flask · scikit-learn · PostgreSQL · pytest · Swagger · Render

---

### FocusPilot — Behavioral Analytics and Autonomous Agent System

Chrome extension and ML pipeline that detects distraction patterns in real-time
and intervenes autonomously using reinforcement learning.

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
Autonomous Agent (Monitor > Decide > Execute > Learn)
     |
Supabase (PostgreSQL + Real-time)
     |
React Dashboard (Vercel)
```

**Project Structure**

```
focuspilot/
|
|-- app/
|   |-- api/            # FastAPI endpoints
|   |-- agents/         # autonomous agent logic
|   |-- models/         # ML model loading and inference
|   |-- services/       # business logic layer
|   |-- schemas/        # request and response validation
|
|-- extension/          # Chrome Extension MV3
|-- frontend/           # React + TypeScript dashboard
|-- tests/              # pytest test suite
|-- notebooks/          # experimentation and analysis
|-- requirements.txt
|-- README.md
```

**Engineering Decisions**

- Why multi-agent architecture? Separating monitoring, decision, execution, and learning agents allows each to be tested and scaled independently.
- Why Supabase real-time? Agent state changes need to propagate to the dashboard instantly without polling.
- Why Chrome MV3? Manifest V3 is the current standard and required for Chrome Web Store submissions.

**Stack:** FastAPI · React · TypeScript · Supabase · scikit-learn · Chrome Extension API · Vercel · HF Spaces

---

### FedRec — Privacy-Preserving Federated Recommendation Engine

Federated learning system that personalizes recommendations across devices
without centralizing raw user data.
Achieves 34% engagement boost with zero privacy violations.

**System Architecture**

```
Device 1 ... Device N  (local training, no raw data shared)
     |              |
Local Model Updates  (encrypted weights only)
     |
FedAvg Aggregation Server
     |
Global Model Update
     |
Streamlit Dashboard
(Privacy Meter · Performance Tracker · Business Impact Calculator)
```

**Engineering Decisions**

- Why FedAvg? It is the most established federated aggregation algorithm with proven convergence guarantees.
- Why no raw data transfer? Privacy-by-design means the system is GDPR-compliant by architecture, not by policy.
- Why multi-domain datasets? Testing across MovieLens, Amazon Reviews, and Spotify-like data validates generalization.

**Key Results:** 9.5/10 privacy score · 34% accuracy boost · $15M+ revenue protection modeled · Scalable to 1M+ simulated devices

**Stack:** Python · PyTorch · TensorFlow · Streamlit · scikit-learn · Federated Learning

---

## Core Engineering Skills

| Domain | Technologies |
|--------|-------------|
| Machine Learning | Python · scikit-learn · TensorFlow · feature engineering · model serving |
| Backend Systems | FastAPI · Flask · REST APIs · PostgreSQL · SQLite · Supabase |
| Data Engineering | Pandas · NumPy · data pipelines · behavioral analytics |
| DevOps and Testing | Docker · GitHub Actions · pytest · CI/CD · Render · Vercel |
| Frontend | React · TypeScript · Tailwind CSS · Recharts |
| Browser Engineering | Chrome Extension API · Manifest V3 · declarativeNetRequest |

---

## System Design Interests

- ML inference infrastructure at scale
- Payment systems and fraud detection pipelines
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
    print(f"[{system}] --> {description}")
```

---

## Achievements

- 2nd Place — IoT Engineering Competition
- Published technical writer on Medium
- Multiple ML systems in production (deployed, tested, documented)
- High academic performance at Covenant University

---

## How I Build Production Systems

Most ML projects stop at notebooks.
I focus on shipping systems that run in production.

Typical architecture I build:

```
Client --> REST API --> Validation Pipeline --> Feature Engineering -->
Model Inference --> Caching Layer --> Database Logging --> Response
```

Engineering principles I follow:

- Separate training pipelines from inference services
- Validate inputs before model inference
- Benchmark multiple models before deployment
- Log predictions for retraining pipelines
- Cache responses to reduce compute cost
- Document APIs with OpenAPI and Swagger

---

## Philosophy

Calling is greater than comfort. Impact over titles. Execution over excuses.

I build systems that work in production — clean code, tested, documented, deployed.

---

<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=14&pause=1000&color=3B82F6&center=true&vCenter=true&width=600&lines=Open+to+ML+Engineering+internships+and+opportunities;github.com%2Folatunjitobiloba)](https://git.io/typing-svg)

</div>
