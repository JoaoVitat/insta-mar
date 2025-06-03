# Documento de Requisitos

## Histórico de Revisões Deste Arquivo

| Data       | Versão | Descrição                | Autor          |
| ---------- | ------ | ------------------------ | ----------     |
| 03/06/2025 | 1.0    | Versão inicial           | Felipe Santos  |

## 1. Introdução

### 1.1 Propósito

Este documento tem como propósito descrever os requisitos funcionais e não funcionais do sistema Instamar, uma rede social exclusiva para alunos da faculdade e profissionais da saúde.

### 1.2 Escopo

O sistema Instamar permitirá a interação entre alunos e profissionais da saúde, oferecendo funcionalidades tradicionais de redes sociais, como criação de perfis e postagens, além de recursos específicos como solicitação de caronas e direcionamento de postagens para públicos-alvo (como veteranos da faculdade).

### 1.3 Definições, Acrônimos e Abreviações

- **Instamar**: Nome do sistema.
- **Veterano**: Usuário com tempo de matrícula superior ao mínimo necessário para orientar novatos.
- **RF**: Requisito Funcional.
- **RNF**: Requisito Não Funcional.
- **UC**: Caso de Uso.

## 2. Descrição Geral

### 2.1 Perspectiva do Produto

Instamar será desenvolvido como uma aplicação web responsiva, podendo futuramente ser convertida para aplicativos móveis. Ele não substitui sistemas acadêmicos, mas se integra a eles para obter dados como curso e período do usuário.

### 2.2 Funcionalidades do Produto

- Cadastro e autenticação de usuários com vínculo acadêmico/profissional validado
- Criação e visualização de postagens
- Direcionamento de posts para veteranos, turma específica ou público geral
- Solicitação e oferta de caronas entre usuários
- Notificações segmentadas
- Sistema de moderação básica e denúncia de conteúdo

### 2.3 Características dos Usuários

- **Alunos da faculdade**: Usuários ativos, com curso e semestre identificáveis.
- **Profissionais da saúde**: Ex-alunos ou convidados com cadastro especial.
- **Veteranos**: Subconjunto de alunos/profissionais com experiência reconhecida.

### 2.4 Restrições

- Apenas usuários autenticados pela faculdade terão acesso à plataforma
- O sistema precisa operar nos navegadores modernos (Chrome, Firefox, Safari)
- Integração com APIs internas da instituição deve respeitar política de segurança

## 3. Requisitos Específicos

### 3.1 Requisitos Funcionais

| ID   | Descrição                                                                 | Prioridade |
| ---- | ------------------------------------------------------------------------- | ---------- |
| RF01 | Permitir o cadastro e login de usuários com validação institucional       | Alta       |
| RF02 | Permitir criação de postagens com seleção de público (geral, turma, etc.) | Alta       |
| RF03 | Implementar filtro para visualização de posts apenas por veteranos        | Alta       |
| RF04 | Permitir solicitação e aceite de caronas entre usuários                   | Média      |
| RF05 | Notificar usuários sobre postagens relevantes                             | Média      |

### 3.2 Requisitos Não Funcionais

| ID    | Categoria   | Descrição                                                                 | Prioridade |
| ----- | ----------- | ------------------------------------------------------------------------- | ---------- |
| RNF01 | Usabilidade | Interface simples e acessível, adaptada para desktop e dispositivos móveis | Alta       |
| RNF02 | Performance | Tempo de resposta inferior a 2 segundos para ações comuns                 | Média      |
| RNF03 | Segurança   | Autenticação segura e proteção contra injeções e XSS                      | Alta       |

## 4. Visão Geral do Sistema

O sistema será dividido em três principais camadas:  
1. **Frontend (Web)**: interface em React ou similar  
2. **Backend (API REST)**: desenvolvido com FastAPI, responsável por regras de negócio  
3. **Banco de Dados**: armazenamento de usuários, postagens, caronas e preferências  

## 5. Casos de Uso

- UC01: Cadastro de usuário  
- UC02: Criação de post com público-alvo  
- UC03: Solicitação de carona  
- UC04: Visualização de feed segmentado  
- UC05: Recebimento de notificações  

(Diagramas visuais podem ser adicionados conforme necessário)

## 6. Priorização de Requisitos

Utilizou-se o método MoSCoW para priorização dos requisitos:

- **Must**: RF01, RF02, RF03  
- **Should**: RF04, RF05  
- **Could**: Integração com redes sociais externas  
- **Won’t**: Gamificação nesta versão inicial

## 7. Aprovação

| Nome       | Papel             | Assinatura | Data       |
| ---------- | ----------------- | ---------- | ---------- |
| gk_Santos  | Analista/Dev      |            | 03/06/2025 |
| [Coordenador] | Coordenador Acadêmico |            | DD/MM/AAAA |

> **Nota:** Este documento será atualizado incrementalmente ao longo do desenvolvimento do projeto.
