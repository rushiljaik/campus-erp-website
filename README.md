# 🎓 CampusAI ERP

**CampusAI ERP** is a modern, responsive, and scalable College Enterprise Resource Planning (ERP) platform designed for Engineering Institutions (modeled for TSEC Mumbai / Mumbai University standards).

---

## 🚀 Tech Stack

- **Frontend Framework**: React 18
- **Build Tool**: Vite
- **Language**: JavaScript (ESModules)
- **Styling**: Tailwind CSS
- **Routing**: React Router DOM v6
- **Animations**: Framer Motion
- **Data Visualizations**: Recharts
- **Icons**: Lucide React
- *(Firebase & Gemini AI ready for Phase 2 integration)*

---

## 📂 Project Architecture

```
TSEC MUMBAI/
├── public/
├── src/
│   ├── assets/               # Brand assets & logos
│   ├── components/
│   │   ├── common/           # Reusable Atomic UI Primitives
│   │   │   ├── Badge.jsx
│   │   │   ├── Button.jsx
│   │   │   ├── DashboardCard.jsx
│   │   │   ├── EmptyState.jsx
│   │   │   ├── Input.jsx
│   │   │   ├── LoadingState.jsx
│   │   │   ├── Modal.jsx
│   │   │   ├── ProgressBar.jsx
│   │   │   ├── Select.jsx
│   │   │   ├── Table.jsx
│   │   │   └── Toast.jsx
│   │   └── layout/           # Global Shell & Navigation
│   │       ├── AppLayout.jsx
│   │       ├── Navbar.jsx
│   │       └── Sidebar.jsx
│   ├── context/
│   │   ├── AuthContext.jsx   # Role Switching & Simulated Auth
│   │   └── ToastContext.jsx  # Notification Manager
│   ├── data/
│   │   └── mockData.js       # Complete Realistic Datasets
│   ├── pages/
│   │   ├── auth/             # Login, Signup
│   │   ├── student/          # Student Portal (6 Routes)
│   │   ├── faculty/          # Faculty Portal (4 Routes)
│   │   ├── admin/            # Admin Portal (4 Routes)
│   │   └── NotFound.jsx
│   ├── routes/
│   │   └── AppRoutes.jsx     # Central Route Declarations
│   ├── styles/
│   │   └── index.css         # Tailwind & Custom Styles
│   ├── utils/
│   │   └── cn.js             # Tailwind Class Utility
│   ├── App.jsx
│   └── main.jsx
├── index.html
├── package.json
├── tailwind.config.js
└── vite.config.js
```

---

## 🧭 Implemented Routes

### 🔐 Authentication
- `/login` — Split-hero authentication screen with 1-click demo persona quick-fills
- `/signup` — Student registration & faculty onboarding form

### 🎓 Student Portal (`/student`)
- `/student/dashboard` — KPI cards (86.4% attendance, 9.42 CGPA), today's lecture schedule, circular alerts
- `/student/attendance` — University 75% attendance criteria monitor, Recharts trend graph, subject safety margins, duty/medical leave request modal
- `/student/marks` — SGPI semester history progression bar chart, Internal Assessment (IA-1 & IA-2) gradebook, transcript modal
- `/student/timetable` — Interactive Monday-Friday weekly schedule with room locations and faculty
- `/student/assignments` — Assignment tabs (Pending, Submitted, Graded) with file upload modal
- `/student/career` — Super Dream Tier placement eligibility, active drives (Google, Microsoft, Morgan Stanley, Barclays), technical skills assessment

### 👨‍🏫 Faculty Portal (`/faculty`)
- `/faculty/dashboard` — Active teaching subjects, today's schedule, pending grading queue
- `/faculty/attendance` — Batch/division selector, interactive attendance roster with 1-click toggle
- `/faculty/marks` — Direct grade entry for Unit Tests, Term Work, Practicals with auto statistics
- `/faculty/assignments` — Create assignment modal, evaluate student submissions with scoring & remarks

### 🏛️ Admin Portal (`/admin`)
- `/admin/dashboard` — College-wide KPIs (2,840 students, 168 faculty, 91.2% placement rate), department breakdown chart
- `/admin/students` — Filterable student directory with Add Student modal and profile preview
- `/admin/faculty` — Faculty directory with designation and workload allocation
- `/admin/notices` — Broadcast notice manager with category and priority flags

---

## ⚡ How to Run Locally

```bash
# 1. Install dependencies (if not already installed)
npm install

# 2. Start Vite development server
npm run dev

# 3. Build for production
npm run build
```

---

## 🎭 Persona Switching for Quick Testing
You can switch between **Student (Aarav Sharma)**, **Faculty (Prof. Sneha Kulkarni)**, and **Admin (Dr. Rajesh Iyer)** anytime using the **Role dropdown** in the top Navbar or using the 1-click demo buttons on the `/login` screen.
