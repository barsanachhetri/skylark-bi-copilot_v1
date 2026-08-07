# 🚀 Skylark BI Copilot

> AI-powered Business Intelligence Agent for Monday.com

Skylark BI Copilot is an AI-powered business intelligence assistant that enables founders and executives to query business data conversationally. It integrates directly with Monday.com boards, cleans inconsistent data, generates actionable insights, and prepares executive-level leadership updates.

---

## ✨ Features

- 🔗 Live Monday.com API Integration (No hardcoded CSV data)
- 🤖 AI-powered conversational business intelligence
- 📊 Real-time analytics dashboard
- 📈 Pipeline health analysis
- 💼 Deal & Work Order insights
- 🧹 Automatic data cleaning and normalization
- ⚠️ Graceful handling of missing and inconsistent data
- 📝 Leadership report generation
- 📉 KPI metrics and business summaries

---

## 🏗️ Architecture

```
             User
               │
               ▼
        React Dashboard
               │
          Axios API Calls
               │
               ▼
        FastAPI Backend
        ┌──────────────┐
        │              │
        ▼              ▼
 Monday.com API    Gemini AI
        │
        ▼
 Deals & Work Orders
```

---

## 🛠️ Tech Stack

### Frontend
- React
- Vite
- Axios
- Recharts
- Framer Motion

### Backend
- FastAPI
- Python
- Monday.com GraphQL API
- Google Gemini API

---

## 📊 Supported Queries

Examples:

- How is our sales pipeline looking this quarter?
- Which sector has the highest revenue?
- What are the operational risks?
- Generate a leadership update.
- Show pipeline health.
- Which deals require immediate attention?

---

## 📂 Project Structure

```
Skylark-BI-Copilot

backend/
frontend/
docs/

README.md
DECISION_LOG.md
```

---

## 🚀 Installation

### Clone

```bash
git clone https://github.com/<your-username>/skylark-bi-copilot.git
```

### Backend

```bash
cd backend

pip install -r requirements.txt

python -m uvicorn main:app --reload
```

Backend runs on

```
http://localhost:8000
```

Swagger Docs

```
http://localhost:8000/docs
```

---

### Frontend

```bash
cd frontend

npm install

npm run dev
```

Frontend runs on

```
http://localhost:5173
```

---

## 🔑 Environment Variables

Create

```
backend/.env
```

```
MONDAY_API_KEY=your_api_key
GEMINI_API_KEY=your_api_key

DEALS_BOARD_ID=xxxx
WORKORDER_BOARD_ID=xxxx
```

---

## 📌 API Endpoints

| Method | Endpoint | Description |
|----------|----------|-------------|
| GET | /analytics | Business KPIs |
| GET | /deals | Deals Data |
| GET | /workorders | Work Order Data |
| POST | /chat | AI Business Assistant |

---

## 🎯 Business Value

Skylark BI Copilot helps leadership:

- Understand pipeline health
- Track operational performance
- Identify business risks
- Generate executive summaries
- Make faster data-driven decisions

---

## 🔮 Future Improvements

- Predictive analytics
- Revenue forecasting
- Interactive dashboards
- PDF leadership reports
- Email summaries
- Slack integration

---

## 📄 License

MIT License
