# SecureVault

# Architecture 
securevault/
│
├── backend/
│   ├── src/
│   │   ├── config/
│   │   │   ├── db.js
│   │   │   ├── env.js
│   │   │   └── logger.js
│   │   │
│   │   ├── modules/
│   │   │   ├── auth/
│   │   │   │   ├── auth.controller.js
│   │   │   │   ├── auth.service.js
│   │   │   │   ├── auth.routes.js
│   │   │   │   └── auth.middleware.js
│   │   │   │
│   │   │   ├── user/
│   │   │   │   ├── user.controller.js
│   │   │   │   ├── user.service.js
│   │   │   │   ├── user.model.js
│   │   │   │   └── user.routes.js
│   │   │   │
│   │   │   ├── vault/
│   │   │   │   ├── vault.controller.js
│   │   │   │   ├── vault.service.js
│   │   │   │   ├── vault.model.js
│   │   │   │   ├── vault.routes.js
│   │   │   │   └── vault.crypto.js
│   │   │   │
│   │   │   ├── logs/
│   │   │   │   ├── log.service.js
│   │   │   │   ├── log.model.js
│   │   │   │   └── log.utils.js
│   │   │   │
│   │   │   ├── threat/
│   │   │   │   ├── threat.service.js
│   │   │   │   ├── threat.rules.js
│   │   │   │   └── threat.controller.js
│   │   │   │
│   │   │   └── session/
│   │   │       ├── session.service.js
│   │   │       ├── session.model.js
│   │   │       └── session.utils.js
│   │   │
│   │   ├── middlewares/
│   │   │   ├── auth.middleware.js
│   │   │   ├── rateLimiter.js
│   │   │   ├── errorHandler.js
│   │   │   └── securityHeaders.js
│   │   │
│   │   ├── utils/
│   │   │   ├── jwt.js
│   │   │   ├── hash.js
│   │   │   ├── crypto.js
│   │   │   └── helpers.js
│   │   │
│   │   ├── app.js
│   │   └── server.js
│   │
│   ├── tests/
│   ├── package.json
│   └── .env
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Navbar.jsx
│   │   │   ├── Sidebar.jsx
│   │   │   ├── ProtectedRoute.jsx
│   │   │   └── Loader.jsx
│   │   │
│   │   ├── pages/
│   │   │   ├── Login.jsx
│   │   │   ├── Register.jsx
│   │   │   ├── Dashboard.jsx
│   │   │   ├── Vault.jsx
│   │   │   ├── Sessions.jsx
│   │   │   └── Alerts.jsx
│   │   │
│   │   ├── services/
│   │   │   ├── api.js
│   │   │   ├── auth.service.js
│   │   │   ├── vault.service.js
│   │   │   └── log.service.js
│   │   │
│   │   ├── hooks/
│   │   │   ├── useAuth.js
│   │   │   ├── useVault.js
│   │   │   └── useLogs.js
│   │   │
│   │   ├── context/
│   │   │   ├── AuthContext.jsx
│   │   │   └── AppContext.jsx
│   │   │
│   │   ├── utils/
│   │   │   ├── constants.js
│   │   │   ├── helpers.js
│   │   │   └── validators.js
│   │   │
│   │   ├── styles/
│   │   │   └── global.css
│   │   │
│   │   ├── App.jsx
│   │   └── main.jsx
│   │
│   ├── package.json
│   └── .env
│
├── database/
│   ├── migrations/
│   ├── seeds/
│   └── schema.sql
│
├── docs/
│   ├── architecture.md
│   ├── api.md
│   ├── database.md
│   ├── security.md
│   ├── threat-model.md
│   └── progress/
│       ├── week-1.md
│       ├── week-2.md
│       └── week-3.md
│
├── docker/
│   ├── backend.Dockerfile
│   ├── frontend.Dockerfile
│   └── docker-compose.yml
│
├── scripts/
│   ├── setup.sh
│   ├── deploy.sh
│   └── seed-db.js
│
├── .gitignore
├── .env.example
├── README.md
└── LICENSE
