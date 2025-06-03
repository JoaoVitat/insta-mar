# Matriz de Rastreabilidade de Requisitos

## Histórico de Revisões deste Arquivo

| Data       | Versão | Descrição                | Autor     |
| ---------- | ------ | ------------------------ | --------- |
| 03/06/2025 | 1.0    | Versão inicial           | gk_Santos |

## 1. Introdução

Este documento apresenta a matriz de rastreabilidade dos requisitos do sistema, permitindo visualizar as relações entre requisitos, casos de uso, componentes do sistema e casos de teste.

## 2. Matriz de Rastreabilidade

### 2.1 Requisitos x Casos de Uso

| Requisito | UC01 | UC02 | UC03 | UC04 | UC05 |
| --------- | ---- | ---- | ---- | ---- | ---- |
| RF01      | X    |      |      |      |      |
| RF02      |      | X    |      | X    |      |
| RF03      |      | X    |      | X    |      |
| RF04      |      |      | X    |      |      |
| RF05      |      |      |      |      | X    |

### 2.2 Requisitos x Componentes do Sistema

| Requisito | Frontend | Backend/API | Banco de Dados | Notificações |
| --------- | -------- | ----------- | -------------- | ------------ |
| RF01      | X        | X           | X              |              |
| RF02      | X        | X           | X              |              |
| RF03      | X        | X           | X              |              |
| RF04      | X        | X           | X              |              |
| RF05      | X        | X           |                | X            |

### 2.3 Requisitos x Casos de Teste

| Requisito | CT01 | CT02 | CT03 | CT04 | CT05 |
| --------- | ---- | ---- | ---- | ---- | ---- |
| RF01      | X    |      |      |      |      |
| RF02      |      | X    |      |      |      |
| RF03      |      |      | X    |      |      |
| RF04      |      |      |      | X    |      |
| RF05      |      |      |      |      | X    |

### 2.4 Requisitos x Requisitos (Dependências)

| Requisito | RF01 | RF02 | RF03 | RF04 | RF05 |
| --------- | ---- | ---- | ---- | ---- | ---- |
| RF01      | -    | X    | X    |      |      |
| RF02      |      | -    |      |      |      |
| RF03      | X    |      | -    |      |      |
| RF04      |      |      |      | -    |      |
| RF05      |      |      | X    |      | -    |

## 3. Análise de Impacto

Esta seção descreve o processo para análise de impacto de mudanças nos requisitos:

1. Identificar o requisito a ser alterado  
2. Consultar a matriz para verificar todos os elementos relacionados  
3. Avaliar o impacto da mudança em cada elemento relacionado  
4. Documentar a análise de impacto  
5. Obter aprovação para a mudança  
6. Atualizar todos os artefatos afetados

> [!IMPORTANT]
> A matriz de rastreabilidade deve ser mantida atualizada durante todo o ciclo de desenvolvimento para garantir a integridade do sistema.

