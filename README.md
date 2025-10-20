# 🏥 Projeto_4559969_Alan_Coelho_Gomes

**PROJETO MULTIDISCIPLINAR — ÊNFASE: DESENVOLVIMENTO FRONT-END**  
**Sistema de Gestão Hospitalar e de Serviços de Saúde (SGHSS)**  

🔗 **Página online (protótipo funcional):**  
[https://alancoelhogomes.github.io/Projeto_4559969_Alan_Coelho_Gomes/](https://alancoelhogomes.github.io/Projeto_4559969_Alan_Coelho_Gomes/)

📄 **Casos de Teste Funcionais:**  
[Ver arquivo PDF](https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes/blob/main/_Casos%20de%20Teste%20Funcionais%20.pdf)

---

## 🧾 Identificação

**CENTRO UNIVERSITÁRIO INTERNACIONAL UNINTER**  
Curso Superior de Tecnologia em **Análise e Desenvolvimento de Sistemas (EaD)**  
Disciplina: **Projeto Multidisciplinar**  
Ênfase: **Desenvolvimento Front-end**  
Aluno: **Alan Coelho Gomes**  
**RU:** 4559969  
**Polo:** Petrolina/PE  
**Ano:** 2025  

---

## 📚 Sumário

1. [Introdução](#1-introdução)  
2. [Estudo de Caso: SGHSS (VidaPlus)](#2-estudo-de-caso-sghss-vidaplus)  
3. [Análise e Requisitos](#3-análise-e-requisitos)  
4. [Modelagem e Arquitetura (Front-end)](#4-modelagem-e-arquitetura-foco-front-end)  
5. [Implementação (Prototipagem)](#5-implementação-prototipagem)  
6. [Plano de Testes e Qualidade](#6-plano-de-testes-e-qualidade)  
7. [Conclusão](#7-conclusão)  
8. [Referências](#8-referências)  
9. [Anexos](#9-anexos)  

---

## 1. INTRODUÇÃO

Este projeto apresenta a concepção, modelagem e prototipagem de um **Sistema de Gestão Hospitalar e de Serviços de Saúde (SGHSS)** para a instituição fictícia **VidaPlus**, com ênfase em **Desenvolvimento Front-end**.

O objetivo é demonstrar um **protótipo interativo e responsivo** que suporte processos críticos como:
- Cadastro e atendimento de pacientes;
- Gestão de profissionais de saúde;
- Agendamento de consultas e telemedicina.

O sistema prioriza **usabilidade, acessibilidade (WCAG)** e **privacidade (LGPD)**, integrando conceitos de **engenharia de software, design centrado no usuário e qualidade de sistemas**.

---

## 2. ESTUDO DE CASO: SGHSS (VidaPlus)

**Contexto:**  
A VidaPlus administra clínicas, hospitais e serviços de home care. A organização necessita centralizar:
- Cadastro e atendimento de pacientes;  
- Agendas e prescrições de profissionais;  
- Administração hospitalar (leitos, suprimentos, relatórios);  
- Telemedicina com videochamadas seguras;  
- Controle de segurança e conformidade (LGPD).  

**Atores principais:**  
👤 Paciente — agenda consultas e acessa histórico.  
🩺 Profissional de Saúde — gerencia agenda e prontuários.  
🧑‍💼 Administrador — controla cadastros, relatórios e acessos.  

**Escopo do protótipo:**  
Fluxos principais de **Paciente** e **Profissional**, com telas de login, dashboard, agendamento e visualização de consultas, simulando o comportamento de um sistema real.

---

## 3. ANÁLISE E REQUISITOS

### 3.1 Requisitos Funcionais
| ID | Descrição |
|----|------------|
| **RF001** | Login e logout de pacientes e profissionais. |
| **RF002** | Cadastro de pacientes com validação front-end. |
| **RF003** | Agendamento em múltiplas etapas (especialidade, profissional, horário). |
| **RF004** | Acesso simulado à teleconsulta (sala virtual placeholder). |
| **RF005** | Dashboard de profissional com consultas do dia e prontuário básico. |

### 3.2 Requisitos Não Funcionais
| ID | Descrição |
|----|------------|
| **RNF001** | Acessibilidade conforme WCAG (aria-labels, contraste, navegação por teclado). |
| **RNF002** | Layout responsivo (desktop, tablet, mobile). |
| **RNF003** | Simulação de segurança/LGPD — dados mascarados e não persistentes. |
| **RNF004** | Feedbacks visuais e mensagens de erro/sucesso. |
| **RNF005** | Desempenho otimizado — sem dependências externas pesadas. |

### 3.3 Casos de Uso (descrição textual)
- **Paciente:** Registrar → Login → Agendar → Teleconsulta → Histórico  
- **Profissional:** Login → Gerenciar Agenda → Prontuário → Prescrição  
- **Administrador:** Login → Gerenciar Usuários → Relatórios  

*(O diagrama visual encontra-se nos anexos.)*

---

## 4. MODELAGEM E ARQUITETURA (Foco Front-end)

### 4.1 Arquitetura
- **HTML / CSS / JavaScript (Vanilla)** — SPA simulada em um único arquivo.  
- **Componentização simulada:**  
  `/components` → Botões, Inputs, Cards, Headers  
  `/pages` → Login, DashboardPaciente, Agendamento, DashboardProfissional  
- **Design System:** variáveis CSS (tema claro/escuro, tipografia, radius).  
- **Acessibilidade:** `aria-*`, contraste de cores, foco visível.  

### 4.2 Wireframes (descrição)
- **Login:** campos CPF/email, senha, botão entrar, alternância de tema.  
- **Dashboard Paciente:** atalhos rápidos (Agendar, Histórico, Telemedicina).  
- **Agendamento:** wizard em 3 etapas (Especialidade → Profissional → Horário).  
- **Dashboard Profissional:** consultas do dia + acesso a prontuários.  

---

## 5. IMPLEMENTAÇÃO (PROTOTIPAGEM)

**Tecnologias:**  
- HTML5, CSS3 (com variáveis de tema)  
- JavaScript (vanilla)  
- Design responsivo (Flexbox + Grid)  
- Modo escuro automático  

**Deploy:** GitHub Pages  
🔗 [Acessar Protótipo Online](https://alancoelhogomes.github.io/Projeto_4559969_Alan_Coelho_Gomes/)

---

## 6. PLANO DE TESTES E QUALIDADE

### 6.1 Estratégia
- Testes manuais dos fluxos principais (login, cadastro, agendamento).  
- Testes de usabilidade com usuários.  
- Testes de acessibilidade (Lighthouse, axe-core).  
- Testes de responsividade (desktop, tablet, mobile).  

### 6.2 Casos de Teste Funcionais
| ID | Caso de Teste | Entrada | Resultado Esperado |
|----|----------------|----------|--------------------|
| CT001 | Login válido | CPF/email + senha | Redireciona ao dashboard |
| CT002 | Login inválido | Campos vazios | Exibe mensagem de erro |
| CT003 | Agendamento conflito | Horário ocupado | Exibe alerta e horários alternativos |
| CT004 | Alternância de tema | Clicar no botão de tema | Tema alterna e persiste preferência |
| CT005 | Navegação por teclado | Pressionar TAB | Foco visível em todos elementos |

---

## 7. CONCLUSÃO

O protótipo **SGHSS (VidaPlus)** demonstrou viabilidade técnica e de usabilidade para processos essenciais de gestão hospitalar.  
Os resultados mostram **boa responsividade, clareza de interface e conformidade parcial com padrões de acessibilidade**.  

**Próximas etapas recomendadas:**
- Implementar API REST com autenticação JWT.  
- Integrar telemedicina via WebRTC.  
- Automatizar testes (Cypress).  
- Validar LGPD e segurança com ferramentas OWASP.  

---

## 8. REFERÊNCIAS
- PRESSMAN, R. S. *Engenharia de Software: Uma Abordagem Profissional.*  
- W3C. *Web Content Accessibility Guidelines (WCAG) 2.1.*  
- MDN Web Docs. *Acessibilidade e boas práticas Front-end.*  
- CYPRESS Docs. *End-to-end testing for the modern web.*  
- OWASP Foundation. *Top 10 Security Risks & Secure Coding Practices.*  

---

## 9. ANEXOS
- **Anexo A:** Diagrama de Casos de Uso  
- **Anexo B:** Wireframes (Login, Dashboard, Agendamento)  
- **Anexo C:** Código fonte (`index.html`)  
- **Anexo D:** Casos de Teste (PDF)  
- **Anexo E:** Relatórios de usabilidade e métricas  

---

💡 **Autor:** Alan Coelho Gomes  
📍 **Petrolina - PE, 2025**
