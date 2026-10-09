# 🎯 PPPE Study Finder

> Plataforma de estudos desenvolvida para facilitar a busca e organização de conteúdos em vídeo para preparação para o concurso da **Polícia Penal de Pernambuco (PPPE)**.

O **PPPE Study Finder** transforma o conteúdo programático do edital em uma ferramenta de pesquisa de estudos, permitindo identificar disciplinas, assuntos e encontrar vídeos relacionados no YouTube.

O projeto foi desenvolvido com foco em **automação, organização de conteúdo e experiência de estudo**, utilizando uma arquitetura que pode ser expandida para outros concursos e editais.

---

## 🚀 Showcase

### 📚 Organização baseada no edital

O sistema utiliza a estrutura do conteúdo programático para organizar os estudos por:

* Disciplinas
* Assuntos
* Subassuntos
* Termos relacionados
* Conteúdos de apoio

A ideia é permitir que o estudante saia de uma lista extensa de tópicos do edital diretamente para conteúdos específicos de estudo.

---

### 🔎 Busca inteligente de vídeos

O projeto utiliza a **YouTube Data API** para localizar conteúdos relacionados aos assuntos do edital.

O mecanismo de busca considera os termos do assunto para encontrar materiais potencialmente relevantes, facilitando a descoberta de:

* Videoaulas
* Revisões
* Resumos
* Questões comentadas
* Aulas específicas por assunto

---

### ⚙️ Automação

O projeto foi pensado para reduzir o trabalho manual necessário para pesquisar conteúdo.

Fluxo simplificado:

```text
                 ┌─────────────────┐
                 │  Edital da PPPE │
                 └────────┬────────┘
                          │
                          ▼
                ┌───────────────────┐
                │ Módulo do Edital  │
                └─────────┬─────────┘
                          │
                          ▼
                ┌───────────────────┐
                │ Disciplina/Tópico │
                └─────────┬─────────┘
                          │
                          ▼
                ┌───────────────────┐
                │ Motor de Pesquisa │
                └─────────┬─────────┘
                          │
                          ▼
                ┌───────────────────┐
                │   YouTube API     │
                └─────────┬─────────┘
                          │
                          ▼
                ┌───────────────────┐
                │ Vídeos encontrados│
                └───────────────────┘
```

---

## 🖥️ Interface

O projeto também possui uma interface Web para facilitar a utilização da ferramenta.

A aplicação apresenta uma experiência voltada para estudo, permitindo navegar pelos conteúdos e realizar pesquisas sem precisar utilizar diretamente a API ou comandos no terminal.

### Principais conceitos da interface

* Dashboard de estudos
* Seleção de disciplinas
* Seleção de assuntos
* Pesquisa de conteúdos
* Resultados do YouTube
* Organização visual dos tópicos
* Interface responsiva

---

## 🛠️ Tecnologias

### Backend / CLI

* **Node.js**
* **TypeScript**
* **YouTube Data API v3**
* Arquitetura modular
* Variáveis de ambiente

### Frontend

* **React**
* **TypeScript**
* **Vite**
* **Tailwind CSS**

### Ferramentas

* Git
* GitHub
* npm
* APIs REST

---

## 🧩 Arquitetura

O projeto foi estruturado de forma modular para separar as responsabilidades da aplicação.

```text
PPPE-Study-Finder
│
├── CLI
│   ├── comandos
│   └── execução via terminal
│
├── Edital
│   ├── disciplinas
│   ├── assuntos
│   └── estrutura programática
│
├── YouTube
│   ├── pesquisa
│   ├── integração com API
│   └── resultados
│
└── Web
    ├── React
    ├── componentes
    ├── interface
    └── pesquisa de conteúdos
```

---

## 💻 CLI

Além da interface Web, o projeto conta com uma versão de linha de comando.

Exemplo conceitual:

```bash
npm install
npm run build
npm start
```

A aplicação permite consultar os conteúdos do edital e realizar pesquisas relacionadas.

---

## 🔐 Configuração

A chave da YouTube Data API deve ser configurada através de variável de ambiente.

Exemplo:

```env
YOUTUBE_API_KEY=sua_chave_aqui
```

> **Importante:** nunca coloque sua chave real diretamente no código ou faça commit do arquivo `.env`.

Para o GitHub, utilize um arquivo `.env.example`:

```env
YOUTUBE_API_KEY=
```

---

## 📌 Objetivos do projeto

O projeto foi desenvolvido com alguns objetivos principais:

1. Transformar o edital em uma estrutura pesquisável.
2. Automatizar a procura por conteúdos de estudo.
3. Reduzir o tempo gasto procurando videoaulas.
4. Criar uma experiência de estudo organizada.
5. Praticar integração com APIs externas.
6. Desenvolver uma aplicação utilizando TypeScript.
7. Criar uma arquitetura que possa ser reutilizada em outros concursos.

---

## 🔄 Possíveis evoluções

O projeto pode evoluir para uma plataforma de estudos mais completa.

Algumas possibilidades:

* [ ] Sistema de progresso por disciplina
* [ ] Controle de assuntos estudados
* [ ] Favoritos
* [ ] Histórico de vídeos
* [ ] Checklist do edital
* [ ] Cronograma de estudos
* [ ] Estatísticas de desempenho
* [ ] Integração com questões
* [ ] Banco de questões
* [ ] Sistema de revisão
* [ ] Flashcards
* [ ] Suporte a outros concursos
* [ ] Autenticação de usuários
* [ ] Persistência dos dados

---

## 🎓 Contexto

O **PPPE Study Finder** surgiu como um projeto de estudo e desenvolvimento de software voltado para resolver um problema real:

> **Como transformar um edital extenso em um caminho mais simples para encontrar conteúdo de estudo?**

A partir desse problema, o projeto combina **estruturação de dados, automação, APIs externas e desenvolvimento Web** em uma única aplicação.

---

## 👨‍💻 Desenvolvedor

**Karlyson Felipe Bastos Araujo Santos**

Desenvolvedor de Software com experiência em:

* Flutter / Dart
* Laravel / PHP
* PostgreSQL
* APIs REST
* Desenvolvimento Web
* Desenvolvimento Mobile
* Integração de APIs
* Arquitetura de software

### Tecnologias

```text
Flutter       ████████████████████
Dart          ████████████████████
Laravel       ████████████████████
PHP           ████████████████████
PostgreSQL    ████████████████████
TypeScript    ████████████████
React         ████████████████
Node.js       ████████████████
```

---

## ⭐ Sobre o projeto

Este projeto faz parte do meu portfólio de desenvolvimento e demonstra minha capacidade de transformar uma necessidade prática em uma solução de software utilizando **TypeScript, React, Node.js, APIs externas e organização de dados**.

Se este projeto for útil para você, considere deixar uma ⭐ no repositório.
