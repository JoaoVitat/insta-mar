# História de Usuário: US001

## Título

Publicar post direcionado para veteranos da faculdade

## Narrativa

**Como** aluno da faculdade  
**Eu quero** publicar postagens visíveis apenas para os veteranos do meu curso  
**Para que** eu possa obter conselhos e informações de quem já passou pelas etapas que estou enfrentando

## Critérios de Aceitação

1. O usuário pode escolher a visibilidade do post (público, apenas veteranos, apenas alunos do mesmo semestre etc.)
2. A funcionalidade verifica se o usuário é veterano com base em critérios definidos (semestre atual, tempo de matrícula, etc.)
3. Veteranos recebem notificações diferenciadas sobre esses posts

## Detalhes Técnicos

- Utilizar filtros de visibilidade no banco de dados (ex.: tags por grupo de usuários)
- Integração com sistema de autenticação da faculdade para validar status de veterano
- Endpoint específico para postagem com visibilidade direcionada
- Interface com dropdown de seleção de público-alvo

## Dependências

- Autenticação de usuário com vínculo validado pela faculdade
- Cadastro completo de curso, período e ano de ingresso de cada usuário

## Estimativa

5 Story Points

## Prioridade

Must

## Observações

Critério para definir “veterano” deve ser ajustável no painel administrativo da aplicação.
