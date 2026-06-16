# Meu E-commerce

Plataforma de e-commerce completa com backend em Node.js + Express + MongoDB e frontend em React + Vite.

## Tecnologias

**Backend:** Node.js, Express, MongoDB (Mongoose), JWT, Stripe, Mercado Pago
**Frontend:** React, Vite, Axios, React Router DOM, Context API

## Estrutura

```
meu-ecommerce/
├── backend/    # API RESTful
├── frontend/   # Interface React
└── README.md
```

## Como Rodar

### Com Docker (recomendado)
```bash
# Iniciar todos os serviços (MongoDB + Backend + Frontend)
docker compose up -d

# Acompanhar logs
docker compose logs -f

# Parar tudo
docker compose down

# Parar e remover volumes (dados do banco)
docker compose down -v
```

### Sem Docker (desenvolvimento local)
**Pré-requisito:** Ter MongoDB rodando localmente na porta 27017.

```bash
# Backend (porta 5000)
cd backend
npm install
npm run dev

# Frontend (porta 5173)
cd frontend
npm install
npm run dev
```

### Popular banco com dados de teste
```bash
cd backend
npm run seed
```
