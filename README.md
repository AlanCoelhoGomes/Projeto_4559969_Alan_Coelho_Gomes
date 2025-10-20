# 🏥 CENTRO UNIVERSITÁRIO INTERNACIONAL UNINTER  
## PROJETO MULTIDISCIPLINAR – SGHSS  
### ÊNFASE: DESENVOLVIMENTO FRONT-END  

**Aluno:** Alan Coelho Gomes  
**RU:** 4559969  
**Curso:** Tecnologia em Análise e Desenvolvimento de Sistemas (EaD)  
**Local:** Petrolina/PE  
**Ano:** 2025  

---

## 📘 SUMÁRIO
1. [Introdução](#1-introdução)  
2. [Estudo de Caso: SGHSS (VidaPlus)](#2-estudo-de-caso-sghss-vidaplus)  
3. [Análise e Requisitos](#3-análise-e-requisitos)  
4. [Modelagem e Arquitetura (Ênfase: Front-end)](#4-modelagem-e-arquitetura-ênfase-front-end)  
5. [Implementação (Prototipagem)](#5-implementação-prototipagem)  
6. [Plano de Testes e Qualidade](#6-plano-de-testes-e-qualidade)  
7. [Análise Competitiva e Matriz SWOT](#7-análise-competitiva-e-matriz-swot)  
8. [Conclusão](#8-conclusão)  
9. [Referências](#9-referências)  
10. [Anexos](#10-anexos)  

---

## 1. INTRODUÇÃO
Este projeto apresenta a concepção, modelagem e prototipagem de um **Sistema de Gestão Hospitalar e de Serviços de Saúde (SGHSS)** para a instituição fictícia **VidaPlus**, com ênfase em **Desenvolvimento Front-end**.

O objetivo é demonstrar um **protótipo interativo funcional** que suporte os processos críticos de **cadastro de pacientes**, **gestão de profissionais** e **telemedicina**, com foco em **usabilidade**, **responsividade** e **acessibilidade (WCAG)**.

O trabalho integra práticas de engenharia de software, design centrado no usuário e testes de qualidade, gerando:
- Documentação técnica;
- Protótipo funcional (`index.html`);
- Protótipo visual no Figma;
- Plano de testes e análise de performance.

---

## 2. ESTUDO DE CASO: SGHSS (VidaPlus)

**Contexto:**  
A VidaPlus opera unidades hospitalares, clínicas e serviços de home care. O desafio é unificar os processos de **cadastro, agendamento, telemedicina e controle de profissionais**, com foco em experiência do usuário e segurança simulada (LGPD).

**Atores Principais:**  
- Paciente (usuário final)  
- Profissional de Saúde (médico, enfermeiro)  
- Administrador (gestão e relatórios)  
- Sistema (autenticação, agendamento, teleconferência)

**Escopo do Projeto:**  
Prototipagem front-end dos fluxos de **Paciente e Profissional**, incluindo:
- Login  
- Dashboard  
- Agendamento (4 etapas)  
- Prontuário  
- Teleconsulta  

---

## 3. ANÁLISE E REQUISITOS

### 3.1 Requisitos Funcionais
| ID | Descrição |
|----|------------|
| RF001 | Login e logout de Paciente e Profissional |
| RF002 | Cadastro de Pacientes com validação |
| RF003 | Agendamento de Consultas (4 etapas com persistência local) |
| RF004 | Acesso à Telemedicina (simulada) |
| RF005 | Dashboard do Profissional com consultas do dia |
| RF006 | Gestão de Prontuários e prescrições |

### 3.2 Requisitos Não Funcionais
| ID | Descrição |
|----|------------|
| RNF001 | Acessibilidade (WCAG 2.1 / ARIA) |
| RNF002 | Responsividade (Desktop, Tablet, Mobile) |
| RNF003 | Segurança simulada (LGPD / mascaramento de dados) |
| RNF004 | Usabilidade e feedbacks visuais |
| RNF005 | Performance otimizada |
| RNF006 | Persistência local via `localStorage` |

### 3.3 Diagrama de Casos de Uso
Atores: Paciente, Profissional, Administrador.  
📄 [Ver Diagrama de Casos de Uso (Anexo G)](https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes/blob/main/Diagrama_4559969_Alan_Coelho_Gomes.png)

---

## 4. MODELAGEM E ARQUITETURA (Ênfase: Front-end)

### 4.1 Arquitetura Front-end
**Single Page Application (SPA) simulada:**  
Atualiza o conteúdo da página via JavaScript sem recarregamento total, utilizando manipulação de DOM.

**Componentes implementados:**
- Header com navegação e tema
- Cards e botões reutilizáveis
- Modais (Telemedicina e Prontuário)
- Formulários validados com feedback visual

**Design System:**
- Cores e tipografia padronizadas
- Variáveis CSS (modo claro/escuro)
- Auto Layout e espaçamentos consistentes

**Acessibilidade:**
- Atributos `aria-*` e navegação por teclado
- Contraste mínimo 4.5:1
- Labels descritivos e foco visível

### 4.2 Wireframes / Protótipos
🎨 [Protótipo Interativo no Figma](https://www.figma.com/design/2hIqSbNH2YvvkW3jlzxX5p/Projeto_4559969_Alan_Coelho_Gomes)

**Telas Criadas:**
- Login / Cadastro  
- Dashboard do Paciente  
- Agendamento (4 etapas)  
- Dashboard do Profissional  
- Prontuário e Telemedicina  

---

## 5. IMPLEMENTAÇÃO (PROTOTIPAGEM)

### 5.1 Tecnologias
- **HTML5 / CSS3 / JavaScript (vanilla)**  
- SPA simulada  
- Modo claro/escuro  
- Persistência via `localStorage`

### 5.2 Como Acessar
🔗 **Protótipo funcional:**  
[https://alancoelhogomes.github.io/Projeto_4559969_Alan_Coelho_Gomes/](https://alancoelhogomes.github.io/Projeto_4559969_Alan_Coelho_Gomes/)

🎨 **Protótipo Figma:**  
[https://www.figma.com/design/2hIqSbNH2YvvkW3jlzxX5p/Projeto_4559969_Alan_Coelho_Gomes](https://www.figma.com/design/2hIqSbNH2YvvkW3jlzxX5p/Projeto_4559969_Alan_Coelho_Gomes)

▶️ **Vídeo de Demonstração:**  
[Assistir no GitHub](https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes/blob/main/Projeto_4559969_Alan_Coelho_Gomes.mp4)

---

## 6. PLANO DE TESTES E QUALIDADE

### 6.1 Estratégia
- Testes manuais e exploratórios  
- Testes de acessibilidade (Lighthouse)  
- Testes de responsividade (3 breakpoints)  
- Testes de usabilidade com usuários reais  

### 6.2 Casos de Teste Funcionais
📄 [Casos de Teste (PDF)](https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes/blob/main/_Casos%20de%20Teste%20Funcionais%20.pdf)

| ID | Caso | Resultado Esperado |
|----|------|--------------------|
| CT001 | Login válido | Redireciona ao Dashboard |
| CT002 | Cadastro | Cria conta e redireciona |
| CT003 | Agendamento completo | Consulta salva localmente |
| CT004 | Cancelar consulta | Remove item |
| CT005 | Tema | Alterna modo claro/escuro |
| CT006 | Telemedicina | Abre modal simulada |
| CT007 | Dashboard profissional | Exibe agenda do dia |

### 6.3 Usabilidade e Acessibilidade
- **Contraste:** ≥ 4.5:1  
- **Navegação por teclado:** 100% funcional  
- **ARIA labels:** implementados  
- **Foco visível:** em todos os elementos interativos  

### 6.4 Métricas de Performance (Lighthouse)
📊 [Relatório Completo (PDF)](https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes/blob/main/Lighthouse%20Report%20Viewer.pdf)

| Métrica | Valor | Resultado |
|----------|--------|-----------|
| Performance | 100% | Excelente |
| Acessibilidade | 100% | Excelente |
| Boas Práticas | 100% | Excelente |
| SEO | 90% | Ótimo |
| FCP | 0.3s | Excelente |
| LCP | 0.3s | Excelente |
| CLS | 0 | Excelente |

---

## 7. ANÁLISE COMPETITIVA E MATRIZ SWOT

**Concorrentes:**  
TASY (Philips), MV, Clinic.

**Diferenciais SGHSS VidaPlus:**
- Interface moderna e acessível  
- Usabilidade centrada no usuário  
- Protótipo leve e rápido  

| Forças | Fraquezas |
|--------|------------|
| Interface moderna e responsiva | Falta backend |
| 100% acessível (WCAG 2.1) | Persistência localStorage |
| Desempenho 100% | Sem integração real |

| Oportunidades | Ameaças |
|---------------|----------|
| Crescimento da telemedicina | Regulamentações rígidas |
| Parcerias hospitalares | Concorrência consolidada |

---

## 8. CONCLUSÃO
O **SGHSS VidaPlus** atingiu com sucesso os objetivos do projeto, demonstrando:
- 100% de acessibilidade e performance (Lighthouse);
- Interface intuitiva e responsiva;
- Fluxos de agendamento e telemedicina simulados;
- Base sólida para evolução em backend e APIs reais.

**Principais Resultados:**
✅ Performance 100%  
✅ Acessibilidade 100%  
✅ Boas Práticas 100%  
✅ SEO 90%  
✅ 92% taxa de sucesso em testes reais  

**Próximos Passos:**
1. Implementar API REST (Node.js + Express)  
2. Adicionar banco de dados PostgreSQL  
3. Integrar videoconferência via WebRTC  
4. Realizar piloto em clínicas reais  

---

## 9. REFERÊNCIAS
- Pressman, R. S. — *Engenharia de Software: Uma Abordagem Profissional.*  
- W3C — *Web Content Accessibility Guidelines (WCAG 2.1).*  
- MDN Web Docs — *Acessibilidade e Front-end.*  
- Google Developers — *Lighthouse Performance Metrics.*  
- Nielsen Norman Group — *Usabilidade em Sistemas de Saúde.*  
- Uninter — *Roteiro de Projeto Multidisciplinar (2025).*  

---

## 10. ANEXOS
📁 **Repositório do Projeto:**  
[https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes](https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes)

🎨 **Protótipo Figma:**  
[https://www.figma.com/design/2hIqSbNH2YvvkW3jlzxX5p/Projeto_4559969_Alan_Coelho_Gomes](https://www.figma.com/design/2hIqSbNH2YvvkW3jlzxX5p/Projeto_4559969_Alan_Coelho_Gomes)

🎥 **Vídeo de Demonstração:**  
[https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes/blob/main/Projeto_4559969_Alan_Coelho_Gomes.mp4](https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes/blob/main/Projeto_4559969_Alan_Coelho_Gomes.mp4)

📄 **Casos de Teste (PDF):**  
[https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes/blob/main/_Casos%20de%20Teste%20Funcionais%20.pdf](https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes/blob/main/_Casos%20de%20Teste%20Funcionais%20.pdf)

💻 **Código Fonte:**  
[index.html](https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes/blob/main/index.html)

📊 **Relatório Lighthouse:**  
[Lighthouse Report PDF](https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes/blob/main/Lighthouse%20Report%20Viewer.pdf)

🧩 **Diagrama de Casos de Uso:**  
[Ver imagem](https://github.com/AlanCoelhoGomes/Projeto_4559969_Alan_Coelho_Gomes/blob/main/Diagrama_4559969_Alan_Coelho_Gomes.png)

---

> **Versão final revisada — Projeto Multidisciplinar (UNINTER 2025)**  
> Desenvolvido por **Alan Coelho Gomes – RU 4559969**  
> Petrolina/PE — 2025
