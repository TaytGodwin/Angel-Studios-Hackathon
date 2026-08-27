# Angel Studios / Movie Recommender Platform

Streaming platforms often present users with thousands of titles without tailored guidance. This creates **Choice Fatigue** — users spend more time scrolling through content catalogs than actually watching movies.

Traditional recommendation widgets rely solely on static popularity lists, ignoring individual user watching histories, genre affinities, and subtle similarity metrics across content libraries.

The **Angel Studios Movie Recommender** solves this by pairing offline Python machine learning models (collaborative filtering and content-based recommendation algorithms) with a high-throughput C# ASP.NET Core REST API backend and an interactive React 19 single-page streaming interface.

*🏆 Featured Machine Learning Architecture — BYU Information Systems INTEX 2025 Competition.*

---

## Project Leadership & Engineering Team

Built and engineered by software engineers:
- **Tayt Godwin** — Project Lead & Full-Stack Developer (React 19 + TypeScript Frontend UI, C# ASP.NET Core REST API, Database Architecture & Auth Security)
- **Mason Dalton** — Machine Learning Engineer & Data Pipeline Developer

---

## How It Works

1. **ML Model Training & Vector Generation**: Python data processing scripts train collaborative filtering and content-based recommendation models on movie ratings and metadata datasets.
2. **Sub-50ms REST API Serving**: C# ASP.NET Core backend exposes optimized REST endpoints that fetch recommendation vectors and filter movie titles with sub-50ms query latency.
3. **Interactive React 19 UI**: Animated React + TypeScript single-page application built with Framer Motion, offering dynamic movie carousels, instant search filtering, and detailed modal deep dives.
4. **Role-Based Auth & Cybersecurity**: Secure user authentication layer with password hashing, role-based access control (User/Admin), and input data validation.
5. **Database & Persistence**: SQLite / SQL Server relational database managed with Entity Framework Core (EF Core) handling user accounts, watchlist items, and movie metadata.

---

## Features

- **Hybrid Recommendation Engine**: Combines collaborative filtering (user rating history) and content-based filtering (metadata similarity) for accurate suggestions.
- **Ultra-Fast API Response Times**: C# ASP.NET Core 8 REST controllers optimized with EF Core query tuning.
- **Rich Animated UI / UX**: Modern streaming layout featuring responsive horizontal sliders, category filters, and smooth state transitions with Framer Motion.
- **Role-Based Security**: Secured admin control panel for catalog management alongside user profile watchlists.
- **Multi-Service Architecture**: Modular repository layout separating `frontend`, `backend`, `ml_python`, and `databaseManagement`.

---

## Tech Stack

| Layer | Technologies |
| :--- | :--- |
| **Frontend** | React 19, TypeScript, Vite, Framer Motion, Bootstrap 5 |
| **Backend API** | C# ASP.NET Core 8 Web API, Entity Framework Core |
| **Machine Learning** | Python, pandas, scikit-learn, NumPy |
| **Database & Auth** | SQLite / SQL Server, ASP.NET Core Identity |
| **Dev Tools** | Visual Studio / VS Code, Git |

---

## Getting Started

### Prerequisites

- .NET 8 SDK
- Node.js (v18+)
- Python 3.10+

### Installation & Local Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/TaytGodwin/INTEX2025.git
   cd INTEX2025
   ```

2. **Run Backend API**:
   ```bash
   cd backend/INTEX2025.API
   dotnet restore
   dotnet run
   ```

3. **Run Frontend Application**:
   ```bash
   cd ../../frontend
   npm install
   npm run dev
   ```

4. **Run Python ML Pipeline (Optional)**:
   ```bash
   cd ../ml_python
   pip install -r requirements.txt
   python generate_recommendations.py
   ```
