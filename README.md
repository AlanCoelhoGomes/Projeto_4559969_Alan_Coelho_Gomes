# 🏥 Projeto_4559969_Alan_Coelho_Gomes  
**PROJETO MULTIDISCIPLINAR — ÊNFASE: DESENVOLVIMENTO FRONT-END**  
**SISTEMA DE GESTÃO HOSPITALAR E DE SERVIÇOS DE SAÚDE (SGHSS)**  

---

### 🌐 **Link da Página Online:**  
🔗 [https://alancoelhogomes.github.io/Projeto_4559969_Alan_Coelho_Gomes/](https://alancoelhogomes.github.io/Projeto_4559969_Alan_Coelho_Gomes/)

### 🎨 **Protótipo no Figma:**  
🖥️ [Acessar o protótipo interativo no Figma](https://www.figma.com/design/2hIqSbNH2YvvkW3jlzxX5p/Projeto_4559969_Alan_Coelho_Gomes?node-id=0-1&t=eg9PfDDUXNUHTU5J-1)

### 🎥 **Vídeo de Demonstração do Protótipo:**  
▶️ [Assistir ao vídeo de demonstração do SGHSS](https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes/blob/main/Projeto_4559969_Alan_Coelho_Gomes.mp4)

### 🧪 **Casos de Teste Funcionais:**  
📄 [Acessar arquivo de casos de teste (PDF)](https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes/blob/main/_Casos%20de%20Teste%20Funcionais%20.pdf)

---

## 🎓 **CENTRO UNIVERSITÁRIO INTERNACIONAL UNINTER**  
**CURSO:** Tecnologia em Análise e Desenvolvimento de Sistemas (EaD)  
**PROJETO MULTIDISCIPLINAR — ÊNFASE: DESENVOLVIMENTO FRONT-END**  
**TEMA:** Sistema de Gestão Hospitalar e de Serviços de Saúde (SGHSS)  

**Autor:** Alan Coelho Gomes  
**RU:** 4559969  
**Local:** Petrolina/PE  
**Ano:** 2025  

---

## 📑 **SUMÁRIO**

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

## 1. **INTRODUÇÃO**
Este projeto apresenta a concepção, modelagem e prototipagem de um **Sistema de Gestão Hospitalar e de Serviços de Saúde (SGHSS)** para a instituição fictícia **VidaPlus**, com ênfase em **Desenvolvimento Front-end**.  
O objetivo é demonstrar um **protótipo interativo e funcional** que suporte os processos de **cadastro e atendimento de pacientes**, **gestão de profissionais** e **telemedicina**, com foco em **usabilidade**, **responsividade** e **acessibilidade (WCAG)**.  

O trabalho integra práticas de **engenharia de software**, **design centrado no usuário** e **testes de qualidade**, entregando:
- Protótipo funcional (SPA – single file `index.html`);
- Protótipo visual interativo (Figma);
- Plano de testes com casos funcionais e de acessibilidade;
- Documentação completa conforme o roteiro da disciplina.  

---

## 2. **ESTUDO DE CASO: SGHSS (VidaPlus)**

**Contexto:**  
A VidaPlus administra clínicas, hospitais e serviços de home care e precisa de um sistema centralizado para:
- Cadastro e atendimento de pacientes;
- Gestão de agendas de profissionais;
- Controle de telemedicina e prontuários.  

**Principais Atores:**
- Paciente (usuário final)  
- Profissional de Saúde (médico/enfermeiro)  
- Administrador (gestão geral)  
- Sistema (serviços de autenticação e agendamento)  

**Escopo do projeto:**  
Prototipagem front-end dos fluxos de **Paciente** e **Profissional**, incluindo:
- Login;  
- Dashboard;  
- Agendamento;  
- Prontuário básico;  
- Teleconsulta (simulada).  

---

## 3. **ANÁLISE E REQUISITOS**

### 3.1 Requisitos Funcionais
- **RF001:** Login e logout de Paciente e Profissional.  
- **RF002:** Cadastro de Pacientes com validação front-end.  
- **RF003:** Agendamento em 3 etapas (Especialidade → Profissional → Data/Hora).  
- **RF004:** Acesso à teleconsulta (simulação).  
- **RF005:** Dashboard do Profissional com consultas do dia.  

### 3.2 Requisitos Não Funcionais
- **RNF001:** Acessibilidade (WCAG 2.1, roles ARIA, contraste).  
- **RNF002:** Responsividade (desktop, tablet e mobile).  
- **RNF003:** Segurança simulada (máscara de dados, LGPD).  
- **RNF004:** Usabilidade e feedbacks visuais.  
- **RNF005:** Desempenho leve (SPA em um único arquivo).  

### 3.3 Diagrama de Casos de Uso
Atores: Paciente, Profissional, Administrador.  
Casos principais:  
- Paciente → Login → Agendar → Teleconsulta → Histórico  
- Profissional → Login → Agenda → Prontuário → Prescrição  
- Administrador → Login → Usuários → Relatórios  

---

## 4. **MODELAGEM E ARQUITETURA (Foco Front-end)**

**Arquitetura:**  
- Simulação de **Single Page Application (SPA)**;  
- Navegação controlada via JavaScript;  
- Estilo gerenciado por **CSS Variables** (tema claro/escuro).  

**Padrões e Boas Práticas:**
- Componentização (botões, cards, modais);  
- Uso de roles ARIA e labels para acessibilidade;  
- Responsividade garantida por Flexbox e Media Queries.  

**Protótipo Visual:**  
📱 [Acesse o protótipo interativo no Figma](https://www.figma.com/design/2hIqSbNH2YvvkW3jlzxX5p/Projeto_4559969_Alan_Coelho_Gomes?node-id=0-1&t=eg9PfDDUXNUHTU5J-1)

---

## 5. **IMPLEMENTAÇÃO (PROTOTIPAGEM)**

**Tecnologias Utilizadas:**  
- HTML5  
- CSS3  
- JavaScript (vanilla, sem frameworks)  

**Acesso ao Protótipo:**  
👉 [Abrir o protótipo funcional online](https://alancoelhogomes.github.io/Projeto_4559969_Alan_Coelho_Gomes/)

**Instruções:**  
1. Acesse o link acima no navegador.  
2. Faça login com as credenciais de exemplo:  
   - Paciente: `paciente@vidaplus.com / 123456`  
   - Profissional: `medico@vidaplus.com / 123456`  
3. Explore os fluxos de **Login → Dashboard → Agendamento → Teleconsulta**.

---

## 6. **PLANO DE TESTES E QUALIDADE**

### 6.1 Estratégia
- Testes manuais de fluxo;  
- Testes de acessibilidade (Lighthouse);  
- Testes de responsividade em 3 breakpoints;  
- Testes de usabilidade com usuários simulados.  

### 6.2 Casos de Teste Funcionais
| ID | Caso de Teste | Resultado Esperado |
|----|----------------|--------------------|
| CT001 | Login válido | Usuário acessa Dashboard |
| CT002 | Login inválido | Mensagem de erro |
| CT003 | Agendamento conflito | Sugere horários alternativos |
| CT004 | Alternância de tema | Tema muda e é salvo |
| CT005 | Navegação por teclado | Todos os campos acessíveis |

📄 [Ver arquivo completo de casos de teste (PDF)](https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes/blob/main/_Casos%20de%20Teste%20Funcionais%20.pdf)

---

## 7. **CONCLUSÃO**
O protótipo SGHSS demonstra a viabilidade técnica e visual de um sistema de gestão hospitalar moderno, acessível e responsivo.  
Cumpre os principais requisitos funcionais e não funcionais, destacando boas práticas de **design system**, **usabilidade** e **segurança simulada (LGPD)**.  

Próximas etapas:
- Implementar backend (API REST + autenticação JWT);  
- Integrar videoconferência segura (WebRTC);  
- Automatizar testes (Cypress);  
- Refinar acessibilidade via testes com usuários.  

---

## 8. **REFERÊNCIAS**
- Pressman, R. S. — *Engenharia de Software: Uma Abordagem Profissional.*  
- W3C — *Web Content Accessibility Guidelines (WCAG) 2.1.*  
- MDN Web Docs — *Acessibilidade e Padrões Web.*  
- Cypress Docs — *End-to-end testing for the modern web.*  
- OWASP — *Top 10 Security Risks & Secure Coding Practices.*

---

## 9. **ANEXOS**
- **Anexo A:** Diagrama de Casos de Uso (imagem).  
- **Anexo B:** Wireframes e Prints (Login, Dashboard, Agendamento).  
- **Anexo C:** Código Fonte (`index.html`).  
- **Anexo D:** Resultados de Testes (Lighthouse, checklist).  
- **Anexo E:** [🎥 Vídeo de Demonstração do Projeto](https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes/blob/main/Projeto_4559969_Alan_Coelho_Gomes.mp4)  
- **Anexo F:** [🎨 Protótipo Interativo no Figma](https://www.figma.com/design/2hIqSbNH2YvvkW3jlzxX5p/Projeto_4559969_Alan_Coelho_Gomes?node-id=0-1&t=eg9PfDDUXNUHTU5J-1)

---

📘 **Repositório do Projeto:**  
[https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes](https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes)
