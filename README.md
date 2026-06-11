# Nexus Frontend 🧠

A sleek and modern **Project Management Web App** — built with **React 19**, **TypeScript**, and **TanStack Router**. Manage projects, track tasks on a Kanban board, and collaborate with your team in real time.

> 🔗 Backend API → [nexus-backend](https://github.com/t9amw0rk-sys/nexus-backend)

---

## ✨ Features

- 🔐 **Auth** — Login, Register, Google OAuth, Forgot/Reset Password
- 📊 **Dashboard** — Project overview with stats and progress tracking
- 📋 **Kanban Board** — Drag-and-drop task management with priorities & statuses
- 🗂️ **Task Drawer** — Detailed task view with comments, attachments & collaborators
- 🔔 **Notifications** — Real-time activity feed
- 👤 **Profile & Settings** — Update your info and preferences
- 🎨 **Dark / Light Mode** — Theme toggle built-in
- ⌨️ **Command Palette** — Quick navigation with keyboard shortcut
- 🌀 **Smooth Animations** — Powered by Framer Motion

---

## 🛠️ Tech Stack

| Category | Technology |
|----------|-----------|
| Framework | React 19 + TypeScript |
| Routing | TanStack Router |
| Build Tool | Vite 7 |
| Styling | Tailwind CSS v4 + shadcn/ui |
| State Management | Zustand |
| Server State | TanStack Query v5 |
| Forms | React Hook Form + Zod |
| Animations | Framer Motion |
| HTTP Client | Axios |
| Icons | Lucide React |
| Charts | Recharts |
| Deployment | Cloudflare Pages |

---

## 📁 Project Structure

```
src/
├── routes/                     # TanStack Router file-based routes
│   ├── index.tsx               # Landing page
│   ├── login.tsx               # Login page
│   ├── register.tsx            # Register page
│   ├── forgot-password.tsx     # Forgot password
│   ├── reset-password.tsx      # Reset password
│   ├── auth.callback.tsx       # Google OAuth callback
│   ├── dashboard.tsx           # Main dashboard
│   ├── kanban.tsx              # Kanban board
│   ├── notifications.tsx       # Notifications
│   ├── profile.tsx             # User profile
│   ├── settings.tsx            # App settings
│   ├── onboarding.tsx          # New user onboarding
│   └── admin.tsx               # Admin panel
├── components/
│   ├── nexus/                  # Core app components
│   │   ├── app-shell.tsx       # Main layout wrapper
│   │   ├── sidebar.tsx         # Navigation sidebar
│   │   ├── topbar.tsx          # Top navigation bar
│   │   ├── task-card.tsx       # Kanban task card
│   │   ├── task-drawer.tsx     # Task detail drawer
│   │   ├── command-palette.tsx # Keyboard command palette
│   │   ├── google-button.tsx   # Google OAuth button
│   │   └── theme-toggle.tsx    # Dark/light mode toggle
│   └── ui/                     # shadcn/ui components
├── api/                        # Axios API layer
├── store/                      # Zustand global state
└── lib/                        # Utilities & helpers
```

---

## 🚀 Getting Started

### Prerequisites

- [Node.js 18+](https://nodejs.org/)
- [Nexus Backend](https://github.com/t9amw0rk-sys/nexus-backend) running locally or deployed

### 1. Clone the repository

```bash
git clone https://github.com/t9amw0rk-sys/nexus-frontend.git
cd nexus-frontend
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

```bash
cp .env.example .env
```

Edit `.env`:

```env
VITE_API_URL=http://localhost:5144/api
```

### 4. Start the development server

```bash
npm run dev
```

The app will be available at `http://localhost:5173`

---

## 📦 Available Scripts

| Script | Description |
|--------|-------------|
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm run preview` | Preview production build |
| `npm run lint` | Run ESLint |
| `npm run format` | Format code with Prettier |

---

## 🌐 Deployment

### Cloudflare Pages

This project is configured for **Cloudflare Pages** via `@cloudflare/vite-plugin`.

1. Push to GitHub
2. Connect your repo on [Cloudflare Pages](https://pages.cloudflare.com)
3. Set build command: `npm run build`
4. Set output directory: `dist`
5. Add environment variable: `VITE_API_URL=https://your-api-url.com/api`

### Other Platforms (Vercel / Netlify)

```bash
npm run build
# Deploy the dist/ folder
```

---

## 🔗 Related

- **Backend API** → [nexus-backend](https://github.com/t9amw0rk-sys/nexus-backend)

---

## 📄 License

This project is licensed under the MIT License.
