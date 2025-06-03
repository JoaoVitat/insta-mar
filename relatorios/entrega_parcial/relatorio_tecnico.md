# Relatório Técnico - Entrega Parcial

**Data:** 11/04/2025  
**Versão:** 1.0  
**Equipe:** Grupo I

- Felipe Santos Rocha - Scrum Master
- Luis Lima - Desenvolvedor
- Felipe Rodrigues - Desenvolvedor
- João Vitor Amaro Tavares - Desenvolvedor
- Otavio Augusto Zampronio Marquini - Product Owner
- Heitor Vinicios Giovane Baraveli - QA
- José Eduardo Vigidio da Silva - Desenvolvedor
---


## 1. Resumo Executivo

O projeto *Instamar* tem como objetivo o desenvolvimento de uma rede social exclusiva para estudantes da área da saúde e profissionais da mesma área, permitindo maior integração, suporte e comunicação entre os usuários. Até o momento, foram elaborados os documentos iniciais de requisitos, prototipagem, visão geral do sistema e metodologia de desenvolvimento. O foco atual é o planejamento detalhado da arquitetura, definição das funcionalidades e organização do backlog para iniciar a fase de codificação.

---

## 2. Introdução

### 2.1 Objetivo do Projeto

Desenvolver uma aplicação móvel que sirva como rede social restrita para alunos da área da saúde, com funcionalidades diferenciadas como solicitação de caronas, direcionamento de publicações para veteranos, além das funcionalidades sociais tradicionais como postagens, curtidas e comentários.

### 2.2 Escopo

O sistema prevê funcionalidades como:
- Cadastro e login autenticado
- Perfil de usuário acadêmico
- Postagens públicas e direcionadas
- Interação por curtidas e comentários
- Solicitação e oferta de caronas
- Moderação básica de conteúdo

### 2.3 Metodologia

A metodologia utilizada é o Scrum, com sprints quinzenais e entregas incrementais. A equipe se organiza em reuniões semanais para planejamento, revisão e acompanhamento das tarefas.

---

## 3. Análise de Requisitos

### 3.1 Requisitos Funcionais

- RF01: O sistema deve permitir o cadastro de novos usuários autenticados via e-mail institucional.
- RF02: O usuário deve conseguir publicar postagens visíveis para todos ou direcionadas a grupos específicos.
- RF03: O sistema deve permitir interação com postagens (curtir/comentar).
- RF04: O usuário deve poder solicitar ou oferecer carona.
- RF05: O sistema deve permitir atualização de perfil com informações acadêmicas.

### 3.2 Requisitos Não Funcionais

- RNF01: A interface deve ser responsiva e intuitiva.
- RNF02: A aplicação deve estar disponível 99% do tempo (alta disponibilidade).
- RNF03: Os dados dos usuários devem ser armazenados com segurança.

### 3.3 Matriz de Rastreabilidade

Será vinculada posteriormente ao detalhamento de casos de uso, testes e componentes após o início da codificação.

---

## 4. Arquitetura e Design

### 4.1 Visão Geral da Arquitetura

A arquitetura escolhida é baseada em Flutter (para desenvolvimento multiplataforma) com backend e autenticação via Firebase, aproveitando seus serviços de banco de dados (Firestore), autenticação e storage.

### 4.2 Diagramas

Foram elaborados:
- Diagrama de casos de uso preliminar
- Diagrama de classes de alto nível
- Fluxograma de navegação entre telas

### 4.3 Decisões de Design

- Utilização do Firebase como BaaS para reduzir tempo de desenvolvimento inicial.
- Uso de Flutter para disponibilizar o app tanto para Android quanto para iOS.
- Priorização da UX para estudantes com pouca familiaridade técnica.

### 4.4 Protótipos

Protótipos de telas foram desenvolvidos com foco em usabilidade e navegação intuitiva. As ferramentas utilizadas foram Figma e Canva.

---

## 5. Implementação Atual

Ainda não iniciada. O planejamento da implementação está em andamento e será iniciado após o fechamento dos requisitos e revisão dos protótipos.

---

## 6. Testes

### 6.1 Abordagem de Teste

Serão utilizados testes exploratórios, testes unitários com Flutter e testes de integração com Firebase, planejados para etapas futuras.

### 6.2 Testes Realizados

Ainda não realizados.

### 6.3 Resultados

Não aplicável neste momento.

---

## 7. Progresso do Projeto

### 7.1 Cronograma

O cronograma segue dentro do planejado para a fase de análise e projeto.

### 7.2 Sprints Concluídas

Duas sprints concluídas com foco em documentação, levantamento de requisitos e prototipação.

### 7.3 Métricas

- Documentação inicial: 100%
- Protótipos de alta fidelidade: 80%
- Planejamento de sprints: 100%
- Implementação: 0%

---

## 8. Desafios e Soluções

### 8.1 Principais Desafios

- Definir escopo inicial viável para MVP
- Equilibrar funcionalidades sociais com privacidade e moderação
- Escolher a melhor abordagem para autenticação institucional

### 8.2 Soluções Adotadas

- Definição de um MVP com funcionalidades essenciais
- Utilização dos recursos nativos do Firebase para autenticação e regras de segurança

---

## 9. Próximos Passos

### 9.1 Funcionalidades Planejadas

- Implementar autenticação
- Criar estrutura de usuários e perfis
- Desenvolver o feed de postagens

### 9.2 Melhorias Previstas

- Melhorar a navegação nos protótipos com base em feedbacks
- Refinar casos de uso e fluxos críticos

### 9.3 Cronograma Atualizado

Mantido conforme planejamento inicial, com previsão de início da implementação na próxima sprint.

---

## 10. Lições Aprendidas

- A prototipação inicial é fundamental para alinhar visão entre os membros da equipe.
- A escolha de tecnologias deve considerar o domínio técnico da equipe.
- A documentação contínua evita retrabalho e desalinhamento.

---

## 11. Conclusão

O projeto encontra-se bem estruturado na fase de planejamento. A equipe está preparada para iniciar a fase de desenvolvimento, com base nos requisitos validados e protótipos consolidados.

---

## 12. Anexos

- Protótipos no Figma
- Diagrama de Casos de Uso
- Documento de Requisitos

> [!NOTE]
> Este relatório representa o estado atual do projeto antes do início da implementação. As próximas etapas serão conduzidas com base nas definições aqui estabelecidas.
