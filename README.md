# Projeto_4559969_Alan_Coelho_Gomes
PROJETO MULTIDISCIPLINAR  ÊNFASE: DESENVOLVIMENTO FRONT-END SISTEMA DE GESTÃO HOSPITALAR E DE SERVIÇOS DE SAÚDE (SGHSS)
link da pagina online: https://alancoelhogomes.github.io/Projeto_4559969_Alan_Coelho_Gomes/



















CENTRO UNIVERSITÁRIO INTERNACIONAL UNINTER
CURSO SUPERIOR DE TECNOLOGIA EM ANÁLISE E DESENVOLVIMENTO DE SISTEMAS (EaD) 
PROJETO MULTIDISCIPLINAR 
ÊNFASE: DESENVOLVIMENTO FRONT-END SISTEMA DE GESTÃO HOSPITALAR E DE SERVIÇOS DE SAÚDE (SGHSS)










Alan Coelho Gomes
RU: 4559969








Petrolina/PE

2025

SUMÁRIO
INTRODUÇÃO


ESTUDO DE CASO: SGHSS (VidaPlus)


ANÁLISE E REQUISITOS
  3.1 Requisitos Funcionais
  3.2 Requisitos Não Funcionais
  3.3 Diagrama de Casos de Uso (descrição)


MODELAGEM E ARQUITETURA (Ênfase: Front-end)
  4.1 Design System e Componentização
  4.2 Wireframes / Protótipos de Tela (descrição)


IMPLEMENTAÇÃO (PROTOTIPAGEM)
  5.1 Arquivo de Protótipo (index.html) — Instruções de Acesso


PLANO DE TESTES E QUALIDADE
  6.1 Estratégia de Testes
  6.2 Casos de Teste (tabela)
  6.3 Testes de Usabilidade e Acessibilidade


CONCLUSÃO


REFERÊNCIAS


ANEXOS (Modelos UML, prints, código)












1. INTRODUÇÃO
Este projeto apresenta a concepção, modelagem e prototipagem de um Sistema de Gestão Hospitalar e de Serviços de Saúde (SGHSS) para a instituição VidaPlus, com ênfase em Desenvolvimento Front-end. O objetivo é demonstrar um protótipo interativo que suporte os processos críticos de cadastro/atendimento de pacientes, gestão de profissionais e telemedicina, com foco em usabilidade, responsividade e conformidade com padrões de acessibilidade (WCAG) e privacidade (LGPD).
O trabalho integra práticas de engenharia de software, design centrado no usuário e testes de qualidade, gerando artefatos exigidos pelo roteiro da disciplina: documentação, protótipo funcional (único arquivo HTML simulando aplicação) e plano de testes.

2. ESTUDO DE CASO: SGHSS (VidaPlus)
Contexto: A VidaPlus opera unidades hospitalares, clínicas, laboratórios e serviços de home care. Necessita centralizar: cadastro/atendimento de pacientes, agenda de profissionais, administração hospitalar (leitos/estoques), telemedicina e o controle de segurança/compliance.
Principais atores:
Paciente (usuário final)


Profissional de Saúde (médico, enfermeiro)


Administrador (gestão e relatórios)


Sistema (serviços de autenticação, agendamento, teleconferência)


Escopo deste PM: prototipagem front-end dos fluxos de Paciente e Profissional (login, dashboard, agendamento, prontuário básico, teleconsulta placeholder), priorizando usabilidade e acessibilidade.

3. ANÁLISE E REQUISITOS
3.1 Requisitos Funcionais (seleção priorizada)
RF001 – Autenticação: Login e logout de Paciente e Profissional com validação de credenciais.


RF002 – Cadastro de Pacientes: Formulário para cadastro (nome, CPF, dob, e-mail, senha) com validação front-end.


RF003 – Agendamento: Fluxo de agendamento em três etapas (Especialidade → Profissional → Data/Hora) com confirmação.


RF004 – Acesso a Telemedicina: Link/sala virtual para teleconsulta (simulação no protótipo).


RF005 – Dashboard do Profissional: Visualização das consultas do dia, acesso a prontuários e emissão de prescrições (placeholder).


3.2 Requisitos Não Funcionais
RNF001 – Acessibilidade (WCAG/W3C): Uso de roles ARIA, contraste de cores, labels em inputs e navegação por teclado.


RNF002 – Responsividade: Layouts em três breakpoints (Desktop, Tablet, Mobile).


RNF003 – Segurança / LGPD (simulada no protótipo): mascaramento de dados sensíveis, não persistência de credenciais no protótipo, orientação para criptografia em implementação real.


RNF004 – Usabilidade: Fluxos reduzidos e feedbacks visuais (mensagens de erro/ sucesso).


RNF005 – Performance: páginas leves; protótipo em cliente único sem dependências externas pesadas.


3.3 Diagrama de Casos de Uso — descrição textual (obrigatório)
Atores: Paciente, Profissional, Administrador.
 Casos principais:
Paciente: Registrar → Login → Agendar Consulta → Acessar Teleconsulta → Visualizar Histórico.


Profissional: Login → Gerenciar Agenda → Abrir Prontuário → Emitir Prescrição → Registrar Atendimentos.


Administrador: Login Admin → Gerenciar Usuários → Gerar Relatórios.


(Gráfico do Diagrama de Casos de Uso deve ser incluído em anexo; você pode gerar com draw.io / Lucidchart e inserir como imagem no PDF.)

4. MODELAGEM E ARQUITETURA (Foco Front-end)
4.1 Arquitetura Front-end (proposta)
Single Page Application (SPA) simulada: Um único arquivo HTML com roteamento em client-side via JavaScript (simulação).


Organização por módulos (proposta para implementação real):


/components — Botões, Inputs, Cards, Modais, Header.


/pages — Login, Cadastro, DashboardPaciente, Agendamento, DashboardProfissional, Prontuário.


/styles — Tokens (CSS Variables), Design System.


Design System: variáveis CSS (tema claro/escuro), tokens de cores, tipografia e radius compartilhados.


Acessibilidade: uso de aria-*, labels, foco visível e contraste verificado.


4.2 Wireframes / Protótipos de Tela (descrição textual)
Tela Login (responsiva): campos CPF/E-mail, senha, botão Entrar, link para cadastro, botão alternar tema. Mensagens de erro mostradas abaixo do formulário com aria-live.


Dashboard do Paciente: Cards com atalhos (Agendar, Histórico, Telemedicina), cabeçalho com nome do usuário e botão para logout.


Tela de Agendamento (wizard): passo 1 (Escolher Especialidade), passo 2 (Escolher Profissional), passo 3 (Escolher Data/Hora) com validação e sugestão de horários alternativos.


Dashboard do Profissional: lista de consultas do dia em formato de cards/tabela, botão para abrir prontuário do paciente.


Prontuário (simplificado): resumo do paciente, histórico de atendimentos e campo para anotações.



5. IMPLEMENTAÇÃO (PROTOTIPAGEM)
5.1 Tecnologias usadas no protótipo
HTML / CSS / JavaScript (vanilla) — protótipo single-file (index.html) com navegação simulada, alternância de tema e validação front-end.


Arquivo pronto e funcional foi preparado localmente (código entregue em sessão anterior).


5.2 Como acessar o protótipo (instruções e placeholder)
IMPORTANTE: por exigência do roteiro, o link ao protótipo deve ser público e acessível aos corretores. Se você for subir no GitHub Pages, Netlify ou outro host, insira o URL final abaixo.
Endereço do protótipo (ENTREGA — substituir pelo link real):
 O protótipo interativo e os fluxos de navegação estão disponíveis para avaliação no seguinte endereço/link: [INSERIR LINK FUNCIONAL PARA index.html OU URL PÚBLICA]
Observação: Se for entregar localmente, anexe o arquivo index.html ao ZIP e no PDF informe instruções para o avaliador abrir o arquivo no navegador. Recomendado: fazer deploy no GitHub Pages (https://<usuario>.github.io/<repo>/) e colocar esse link no PDF.

6. PLANO DE TESTES E QUALIDADE
6.1 Estratégia de Testes (Front-end)
Testes Manuais Funcionais: validar todos os fluxos críticos (login, cadastro, agendamento, navegação do profissional).


Testes de Usabilidade: teste com 3–5 usuários reais ou colegas, observando tempo para completar tarefa (ex.: agendar consulta) e pontos de confusão.


Testes de Acessibilidade: verificação com ferramentas (Lighthouse, Contrast Checker) e checagem manual de navegação por teclado e leitores de tela.


Testes de Responsividade: checagem em 3 breakpoints (desktop 1440, tablet 768, mobile 375).


Testes de Regressão: após modificações, reexecutar casos críticos.


Ferramentas sugeridas: Google Lighthouse, Cypress (automação de fluxos), axe-core (acessibilidade).
6.2 Casos de Teste Funcionais (tabela)
ID
Caso de Teste
Entrada
Comportamento Esperado
Resultado Esperado
CT001
Login válido
CPF/email + senha válidos
Sistema valida e redireciona para DashboardPaciente
Usuário visualiza DashboardPaciente
CT002
Login inválido (campo vazio)
CPF vazio ou senha vazia
Não permite login; exibe mensagem de erro
Mensagem "Preencha todos os campos" visível
CT003
Agendamento conflito
Escolher horário já ocupado
Sistema informa conflito e sugere horários alternativos
Alerta de conflito exibido; lista de horários atualizada
CT004
Alternância de tema
Usuário clica em alternar tema
Tema claro/escuro alterna persistindo preferência
Tema alternado e preferência salva (localStorage)
CT005
Navegação por teclado
Usuário usa TAB para navegar
Todos os controles focáveis e legíveis
Foco visível e acessível nos elementos

6.3 Testes de Usabilidade e Métricas
Roteiro de teste: tarefa principal "Agendar uma consulta" (tempo máximo aceitável: 3 minutos).


Métricas coletadas: taxa de sucesso (objetivo > 90%), tempo até completar tarefa, número de erros, feedback qualitativo.


Critérios de aceitação: usuário consegue agendar sem ajuda em ≤ 3 minutos e sem erros de validação não esclarecedores.



7. CONCLUSÃO
O protótipo SGHSS demonstrou a viabilidade dos fluxos críticos: autenticação, agendamento e visualização de dashboards para pacientes e profissionais, com atenção à usabilidade, acessibilidade e responsividade.
Desafios identificados: garantir conformidade completa com LGPD em implementação real (criptografia em trânsito/repouso, consentimentos) e integração com serviços de vídeo (telemedicina) de forma segura.
Próximas etapas recomendadas:
Implementação do backend (API REST) com autenticação JWT e criptografia.


Integração com serviço de video seguro (WebRTC + TURN/STUN).


Automação de testes com Cypress e integração contínua (CI/CD).


Validação de acessibilidade com usuários e correções iterativas.



8. REFERÊNCIAS
Pressman, R. S. — Engenharia de Software: Uma Abordagem Profissional. (Referência para processos de engenharia de software).


W3C — Web Content Accessibility Guidelines (WCAG) 2.1.


MDN Web Docs — Guia de Acessibilidade e Práticas de Front-end.


Cypress Docs — End-to-end testing for the modern web.


OWASP — Top 10 Security Risks and secure coding practices.


(Preencha as referências completas conforme o formato de citação exigido pela instituição.)

9. ANEXOS (Lista / Indicadores para inclusão)
Anexo A — Diagrama de Casos de Uso (imagem).


Anexo B — Wireframes (prints): Login, Dashboard Paciente, Agendamento, Dashboard Profissional.


Anexo C — Código fonte do protótipo (index.html) — incluir como arquivo ou link para repositório.


Anexo D — Resultados de testes: checklist de usabilidade e relatórios (ex.: Lighthouse).


Anexo E — Roteiro de Apresentação (slides/resumo para banca).

