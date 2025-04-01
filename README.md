# Finance Dashboard MVP

Uma aplicação completa de consulta de preços de **ações** e **moedas** em tempo real, com visualização de gráficos históricos, construída com **React + FastAPI**, containerizada com **Docker** e integrada a APIs públicas como **Yahoo Finance** e **AwesomeAPI**.

---

## :art: Fluxograma da Arquitetura

<p align="center">
  <img src="docs/fluxograma-arquitetura.png" alt="Fluxograma da Arquitetura" width="700">
</p>

---

## :hammer: Tecnologias Utilizadas

- **Frontend**: React + Vite + Recharts
- **Backend**: FastAPI + yfinance + requests
- **Banco de dados**: Simulação em tempo de execução (in-memory)
- **API Externa**: Yahoo Finance, AwesomeAPI
- **Containerização**: Docker + Docker Compose

---

## :rocket: Funcionalidades

- Consulta de preço de **ações brasileiras e internacionais**
- Consulta de **moedas** (USD/BRL, EUR/BRL, etc.)
- Histórico de consultas com persistência temporária
- Gráfico de variação de preço (90 dias)
- Interface responsiva com sugestões automáticas e tecla Enter para buscar
- Swagger para testes de API REST
- Suporte a 4 rotas REST:
  - `GET` - buscar
  - `POST` - adicionar no histórico
  - `PUT` - editar histórico
  - `DELETE` - excluir do histórico

---

## :gear: Repositórios Individuais

| Componente | Link |
|------------|------|
| Backend    | [finance-dashboard-backend](https://github.com/Aquino0/finance-dashboard-backend) |
| Frontend   | [finance-dashboard-frontend](https://github.com/Aquino0/finance-dashboard-frontend) |

---

## :clipboard: Como Executar o Projeto

### :whale: Requisitos

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

### :computer: Executando com Docker

```bash
git clone https://github.com/Aquino0/finance-dashboard-mvp.git
cd finance-dashboard-mvp
git clone https://github.com/Aquino0/finance-dashboard-backend.git backend
git clone https://github.com/Aquino0/finance-dashboard-frontend.git frontend


# Subir containers (backend + frontend)
docker-compose up --build
```

Acesse:
- Frontend: [http://localhost](http://localhost)
- Swagger: [http://localhost:8000/docs](http://localhost:8000/docs)

---

## :man_technologist: Autor

**Cristopher Aquino**

- [LinkedIn](https://www.linkedin.com/in/%F0%9F%8E%AF-cristopher-aquino-4992b251/)
- 📱 (21) 98005-9430

---

> Este repositório serve como ponto de apresentação oficial do MVP Finance Dashboard. Confira os repositórios específicos para detalhes de implementação.



