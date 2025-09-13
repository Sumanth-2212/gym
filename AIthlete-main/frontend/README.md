# AI Fitness Frontend

A modern, responsive React frontend for an AI-powered fitness application built with React, TailwindCSS, and Framer Motion.

## ✨ Features

- 🔐 **Authentication** - Login/Signup with JWT token management
- 📊 **Dashboard** - Overview with progress charts and statistics
- 💪 **Workouts** - AI-generated workout plans with filtering and search
- 🍎 **Nutrition** - Diet planning and meal tracking (coming soon)
- 🤖 **AI Chatbot** - Real-time fitness coaching and Q&A
- 📹 **Pose Analysis** - Live webcam exercise form analysis
- 📈 **Progress Tracking** - Charts and analytics for fitness goals
- 📱 **Responsive Design** - Mobile-first design with Tailwind CSS
- ✨ **Smooth Animations** - Framer Motion for seamless transitions

## 🚀 Tech Stack

- **React 18** - Frontend framework
- **Vite** - Build tool and dev server
- **TailwindCSS** - Utility-first CSS framework
- **Framer Motion** - Animation library
- **Recharts** - Chart library for data visualization
- **React Router** - Client-side routing
- **Axios** - HTTP client for API calls
- **Lucide React** - Beautiful icon set

## 🏁 Getting Started

### Prerequisites

- Node.js 18+ and npm

### Installation

1. Install dependencies:
   ```bash
   npm install
   ```

2. Start development server:
   ```bash
   npm run dev
   ```

3. Open [http://localhost:5173](http://localhost:5173) in your browser

### Build for Production

```bash
npm run build
```

## 📁 Project Structure

```
src/
├── components/          # Reusable UI components
│   ├── Layout.jsx      # Main app layout with navigation
│   └── ProtectedRoute.jsx  # Route protection component
├── contexts/           # React contexts
│   └── AuthContext.jsx # Authentication state management
├── pages/              # Page components
│   ├── auth/          # Authentication pages
│   ├── Dashboard.jsx   # Main dashboard
│   ├── Workouts.jsx    # Workout management
│   ├── Chatbot.jsx     # AI fitness coach
│   ├── PoseAnalysis.jsx # Exercise form analysis
│   └── Landing.jsx     # Marketing page
├── services/           # API integration
│   └── api.js         # API calls and configuration
└── lib/               # Utilities
    └── utils.js       # Common utilities
```

## 🎯 Demo

The application includes:

1. **Landing Page** - Beautiful marketing page with features showcase
2. **Authentication** - Login/Signup with form validation
3. **Dashboard** - Interactive charts and fitness overview
4. **Workouts** - Browse and filter AI workout plans
5. **AI Chatbot** - Interactive fitness coach
6. **Pose Analysis** - Real-time webcam exercise form checking

## 🚀 Deployment

Configured for Vercel deployment with `vercel.json`.

```bash
# Deploy to Vercel
vercel
```

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.
