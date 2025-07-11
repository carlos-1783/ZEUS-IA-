# zeus-mvp/README.md

## Zeus IA MVP – Monorepo SaaS

Este monorepo contiene el backend (FastAPI), frontend (Vite + Vue), infraestructura mínima (Fly.io, Vercel), y scripts de despliegue para lanzar tu propia empresa SaaS con un solo comando.

### 📁 Estructura del proyecto
```
zeus-mvp/
├─ backend/              # FastAPI + PostgreSQL + Auth JWT + Stripe
│  ├─ main.py
│  ├─ models.py
│  ├─ database.py
│  ├─ auth.py
│  └─ routes/
│     └─ users.py
├─ frontend/             # Vue 3 + Vite + Login UI
│  ├─ App.vue
│  ├─ main.ts
│  └─ pages/Login.vue
├─ infra/                # Fly.io + Vercel + env
│  ├─ fly.toml
│  ├─ vercel.json
│  └─ .env.template
├─ scripts/
│  └─ start.sh           # Lanza todo con un comando
└─ README.md
```

### 🚀 Cómo empezar

#### 1. Clonar el repositorio
```bash
git clone https://github.com/tuusuario/zeus-mvp.git
cd zeus-mvp
```

#### 2. Configura tu entorno
Copia las variables de entorno:
```bash
cp infra/.env.template backend/.env
```
Edita con tus claves reales de Stripe, DB, etc.

#### 3. Lanza Zeus IA
```bash
bash scripts/start.sh
```

---
 
 
