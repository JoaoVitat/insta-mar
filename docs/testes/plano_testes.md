# Plano de Testes

## Histórico de Revisões

| Data       | Versão | Descrição                     | Autor       |
|------------|--------|-------------------------------|-------------|
| 28/08/2025 | 1.0    | Versão inicial                | João Vitor  |
| 23/09/2025 | 1.1    | Inclusão de testes de performance | Felipe |

---

## 1. Introdução

### 1.1 Objetivos  
Este plano de testes tem como objetivo garantir que as funcionalidades do sistema sejam validadas conforme os requisitos especificados, assegurando qualidade e estabilidade do produto antes do lançamento.

### 1.2 Escopo  
Testar as funcionalidades principais do sistema, incluindo cadastro, login, comentários, e sistema de curtidas, bem como desempenho e segurança.

### 1.3 Definições, Acrônimos e Abreviações  
- **CT**: Caso de Teste  
- **QA**: Garantia de Qualidade (Quality Assurance)  
- **API**: Interface de Programação de Aplicações  
- **UI**: Interface do Usuário  

---

## 2. Estratégia de Teste

### 2.1 Níveis de Teste

#### 2.1.1 Testes Unitários  
Realizados pelos desenvolvedores para validar componentes individuais utilizando frameworks.

#### 2.1.2 Testes de Integração  
Verificam a comunicação entre módulos, focando em APIs e serviços integrados.

#### 2.1.3 Testes de Sistema  
Avaliam o sistema como um todo em ambiente semelhante à produção, testando fluxos completos.

#### 2.1.4 Testes de Aceitação  
Executados por usuários finais ou clientes para validar se o sistema atende aos requisitos.

### 2.2 Tipos de Teste

#### 2.2.1 Testes Funcionais  
Verificam se cada funcionalidade atende aos requisitos especificados.

#### 2.2.2 Testes de Desempenho  
Avaliam a resposta e estabilidade do sistema.

#### 2.2.3 Testes de Segurança  
Identificam vulnerabilidades e asseguram proteção dos dados.

#### 2.2.4 Testes de Usabilidade  
Avaliam a facilidade de uso da interface e experiência do usuário.

#### 2.2.5 Testes de Regressão  
Garantem que funcionalidades antigas continuam funcionando após alterações.

---

## 3. Recursos

### 3.1 Ambientes de Teste  
- Ambiente de desenvolvimento local  
- Ambiente de homologação (servidor de testes)

### 3.2 Ferramentas  
- Jira (gerenciamento de bugs)

### 3.3 Equipe  
- Analista de Testes: responsável por criar e executar casos de teste  
- Desenvolvedores: corrigir bugs encontrados  
- Gerente de QA: supervisão e aprovação

---

## 4. Cronograma

| Atividade              | Início    | Término   |
|------------------------|-----------|-----------|
| Preparação do ambiente | 28/08/2025| 29/08/2025|
| Execução dos testes    | 30/08/2025| 05/09/2025|
| Análise de resultados  | 06/09/2025| 15/09/2025|
| Reporte final          | 16/09/2025| 23/09/2025|

---

## 5. Critérios

### 5.1 Critérios de Entrada  
- Ambiente de teste configurado  
- Casos de teste aprovados  
- Build estável disponível

### 5.2 Critérios de Saída  
- Todos os casos críticos executados  
- Bugs críticos corrigidos  
- Aprovação do gerente de QA

### 5.3 Critérios de Suspensão e Retomada  
- Suspensão: falhas críticas no ambiente de teste  
- Retomada: ambiente estabilizado e bugs corrigidos

---

## 6. Matriz de Risco e Contingência

| Risco                         | Probabilidade | Impacto | Estratégia de Mitigação                      |
|-------------------------------|---------------|---------|---------------------------------------------|
| Falha no ambiente de homologação | Média         | Alto    | Manter backups e ambiente alternativo       |
| Recursos insuficientes         | Baixa         | Médio   | Treinamento e alocação de mais profissionais |
| Atraso no desenvolvimento      | Média         | Alto    | Replanejamento e priorização de tarefas     |

---

## 7. Casos de Teste

| ID | Descrição                   | Requisito | Pré-condições         | Passos                                              | Resultado Esperado                               | Prioridade |
|-------|-----------------------------|-----------|----------------------|-----------------------------------------------------|-------------------------------------------------|------------|
| CT01  | Enviar comentário em post   | REQ-005   | Usuário autenticado  | 1. Acessar post<br>2. Digitar comentário<br>3. Enviar | Comentário aparece imediatamente abaixo do post | Alta       |
| CT02  | Login com credenciais válidas | REQ-001   | Usuário não autenticado | 1. Abrir tela de login<br>2. Inserir usuário e senha<br>3. Confirmar | Usuário é redirecionado para dashboard          | Alta       |

---

## 8. Métricas

- Percentual de casos de teste executados  
- Taxa de defeitos encontrados por tipo  
- Tempo médio para correção de bugs críticos

---

## 9. Relatórios

- Relatório diário de status dos testes  
- Relatório final de execução com indicadores de qualidade  
- Relatório de defeitos com status atualizado

---

## 10. Aprovação

| Nome        | Papel             | Assinatura | Data       |
|-------------|-------------------|------------|------------|
| Felipe  | Gerente de QA     |            | 23/09/2025 |
| Otávio | Analista de Testes|            | 23/09/2025 |


>[!WARNING]
>A execução completa do plano de testes é essencial para garantir a qualidade do software. Qualquer desvio do plano deve ser documentado e justificado.
