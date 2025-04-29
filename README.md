# to-do-list-fullstack

# 📋 Projeto TODO List - Backend em Go + Frontend em React

Este projeto é uma aplicação completa de gerenciamento de tarefas (TODO List) com backend em Go (Golang) e frontend em React.js, com deploy em infraestrutura moderna baseada em Docker, Kubernetes, CI/CD automatizado e monitoramento completo.

---

## ✨ Funcionalidades

- Cadastro, edição, remoção e listagem de tarefas
- Autenticação segura com JWT
- API RESTful em Go usando Gin
- Banco de dados PostgreSQL
- Deploy backend no Fly.io
- Deploy frontend na Vercel
- Containerização com Docker
- Orquestração com Kubernetes
- Pipeline CI/CD com GitHub Actions
- HTTPS via Let's Encrypt (cert-manager no Kubernetes)
- Monitoramento e Alertas (Prometheus + Grafana)
- Autoescalonamento de pods com HPA

---

## 🛠️ Tecnologias Utilizadas

- **Golang** (Gin Framework)
- **PostgreSQL**
- **React.js** (com TailwindCSS - tema escuro)
- **Docker e Docker Compose**
- **Kubernetes** (k3s, EKS, AKS ou GKE)
- **GitHub Actions**
- **Fly.io** (backend)
- **Vercel** (frontend)
- **Prometheus e Grafana** (monitoramento)

---

## ⚙️ Como Rodar Localmente

### Backend

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/todo-list-go-react.git
cd todo-list-go-react/backend

# Ajuste as variáveis de ambiente
cp .env.example .env

# Suba com Docker
docker-compose up --build
```

### Frontend

```bash
# Acesse a pasta do frontend
cd ../frontend

# Instale as dependências
npm install

# Rode o app
npm start
```

---

## 🚀 Deploy em Produção

- Backend: Fly.io
- Frontend: Vercel
- Banco de Dados: RDS (PostgreSQL gerenciado)

### Deploy com GitHub Actions

O CI/CD automatiza:

- Build da imagem
- Push para Docker Hub
- Deploy para Kubernetes
- Validação do rollout

---

## 🔐 Segurança

- Tokens JWT para autenticação
- HTTPS automático com Let's Encrypt
- Variáveis sensíveis gerenciadas via GitHub Secrets e Kubernetes Secrets

---

## 📈 Monitoramento e Escalabilidade

- **Prometheus** coleta métricas do cluster
- **Grafana** exibe dashboards em tempo real
- **HPA (Horizontal Pod Autoscaler)** escala o backend baseado no uso de CPU e memória
- **AlertManager** envia alertas para Slack ou Email em caso de problemas

---

## 📦 Estrutura de Pastas

```plaintext
├── backend/
│   ├── main.go
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   └── Dockerfile
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   └── App.jsx
│   └── tailwind.config.js
│
├── k8s/
│   ├── backend-deployment.yaml
│   ├── backend-service.yaml
│   └── ingress.yaml
│
├── .github/workflows/
│   └── deploy.yaml
│
└── README.md
```

---

## 🧑‍💻 Autor

Feito com ❤️ por  Ariosto Leal\
Conecte-se comigo : https://www.linkedin.com/in/aryostto-leal/



---

## 📝 Licença

Este projeto está sob a licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.



Yostech.Digital






