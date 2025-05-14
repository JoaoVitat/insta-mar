#  Instamar - Definição de Interfaces e Arquitetura do Sistema

## 1. Frontend para Backend (APIs RESTful)

- **Tecnologia**: React ou Flutter → Node.js  
- **Protocolo de Comunicação**: HTTP/HTTPS  
- **Formato de Dados**: JSON  
- **Métodos Utilizados**: `GET`, `POST`, `PUT`, `DELETE`  
- **Autenticação**: JWT (JSON Web Token)

**Exemplo de Endpoints**:
```http
POST /api/login
GET /api/posts
POST /api/messages
```

## 2. Backend para Banco de Dados (PostgreSQL)

- **Tecnologia**: Node.js → PostgreSQL  
- **Modo de Acesso**: SQL direto ou ORM (ex: Sequelize)  
- **Operações**:
  - Inserção de novos usuários, postagens e mensagens.
  - Consulta de feed, histórico de mensagens e dados de perfil.

**Exemplo de Tabela - posts**:
```sql
CREATE TABLE posts (
  id SERIAL PRIMARY KEY,
  user_id INTEGER REFERENCES users(id),
  content TEXT,
  created_at TIMESTAMP DEFAULT NOW()
);
```

## 3. Criptografia das Mensagens (Ponta a Ponta)

- **Tipo**: Criptografia de ponta a ponta (E2EE)
- **Tecnologia recomendada**:  
  - Criptografia assimétrica: RSA ou ECC  
  - Alternativa: biblioteca como **Libsodium** ou **OpenPGP.js**
- **Processo**:
  - A mensagem é criptografada no dispositivo do remetente com a **chave pública** do destinatário.
  - Só pode ser lida após descriptografada com a **chave privada** do destinatário.

## 4. Visão Geral da Arquitetura

**Estilo Arquitetural**: Cliente-Servidor

```plaintext
[Usuário - App (React/Flutter)]
           ⇅ (API REST)
[Back-end - Node.js]
           ⇅ (SQL)
[Banco de Dados - PostgreSQL]
           ⇅
[Serviço de Mensagens Criptografadas]
```

## 5. Componentes Principais

###  Front-end
- **Função**: Interface com o usuário
- **Tecnologias**: React ou Flutter
- **Responsabilidades**:
  - Exibir feed, mensagens, caronas, suporte etc.
  - Navegação fluida e responsiva

###  Back-end
- **Função**: Lógica de negócio
- **Tecnologia**: Node.js
- **Responsabilidades**:
  - Autenticação, postagens, mensagens, denúncias
  - Comunicação com banco de dados
  - Acionamento do módulo de criptografia

###  Banco de Dados
- **Tecnologia**: PostgreSQL
- **Função**: Armazenamento de:
  - Usuários, postagens, mensagens, caronas, denúncias, etc.

###  Módulo de Mensagens
- **Função**: Envio e recebimento de mensagens com segurança
- **Recurso**: Criptografia ponta a ponta

## 6. Justificativas das Escolhas

| Item | Justificativa |
|------|---------------|
| React/Flutter | Interface moderna, responsiva, multiplataforma |
| Node.js | Alta escalabilidade e desempenho |
| PostgreSQL | Confiável, robusto e escalável |
| API REST | Comunicação simples e padronizada |
| Criptografia E2EE | Proteção total da privacidade dos usuários |
