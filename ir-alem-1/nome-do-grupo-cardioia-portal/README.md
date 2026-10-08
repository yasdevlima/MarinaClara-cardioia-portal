# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
    <a href= "https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Admnistração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# CardioIA — Diagnóstico Automatizado com Inteligência Artificial

## 👨‍🎓 Integrantes: 

- Marina Clara Constantino Ribeiro - RM568576
- Yasmin Kauane Silva Lima - RM566645

## 👋 Visão Geral

O CardioIA é um projeto acadêmico desenvolvido na FIAP com o objetivo de simular o uso de Inteligência Artificial como ferramenta de apoio ao diagnóstico e à triagem de pacientes na área de cardiologia.

# 🎥 Demonstração

O vídeo apresenta o funcionamento da solução desenvolvida na Fase 2, incluindo a execução dos códigos, a identificação dos sintomas, a sugestão de possíveis diagnósticos e o funcionamento do classificador de risco.

**Vídeo no YouTube:** [Assistir à demonstração](https://youtu.be/xVTydZK3dh4)

Portal front-end do CardioIA em **React + Vite**, com dados simulados.

## Funcionalidades
- Autenticação simulada via **Context API** (JWT fake no `localStorage`; senha `123456`).
- **Proteção de rotas** com `ProtectedRoute` + `AuthContext`: sem login, redireciona para `/login`.
- Listagem de **pacientes** via API fake (JSONPlaceholder `/users`).
- **Formulário de agendamento** com `useState` (campos) e `useReducer` (lista de consultas, persistida no `localStorage`).
- **Dashboard** com contagem de pacientes e de consultas agendadas.
- Estilização com **CSS Modules**, layout responsivo.

## Estrutura
```
src/
  contexts/    AuthContext.jsx, AppointmentsContext.jsx
  components/  Navbar, ProtectedRoute, StatCard
  services/    api.js
  pages/       Login, Dashboard, Patients, Appointments
```

## Instalação e execução
```bash
npm install
npm run dev      # abre em http://localhost:5173
npm run build    # build de produção
```
Login: qualquer e-mail + senha `123456`.
