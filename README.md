# Endpoint Security Sistemas Distribuídos

## Sprint 1: Configuração Inicial e Definição de Padrões de Segurança

### Objetivo:
Estabelecer as bases do projeto com foco em segurança, incluindo:
- Configuração segura do repositório no GitHub.
- Definição de práticas seguras para os endpoints da API.

---

### 1. Configuração do Repositório

### Boas práticas aplicadas
- **Branches protegidas**: Foi configurada a proteção para a branch `main`, exigindo revisões de pull requests.
- **Revisão obrigatória**: Pull requests devem ser aprovados por pelo menos 1 integrante do time.
- **Commits verificados**: Habilitada a opção para permitir apenas commits assinados.

### Referência
- [Boas práticas do GitHub para repositórios](https://docs.github.com/pt/repositories/creating-and-managing-repositories/best-practices-for-repositories)

---

### 2. Padrões de Segurança da API

### Métodos HTTP utilizados
- `GET`: Leitura de dados.
- `POST`: Criação de novos recursos.
- `PUT`: Atualização completa de recursos.
- `DELETE`: Exclusão de recursos.

### Autenticação
- Definido o uso de **JWT (JSON Web Tokens)** como método principal de autenticação.

### Política de CORS
Implementado controle de CORS para prevenir acesso indevido à API:

```http
Access-Control-Allow-Origin: https://exemplo.com
Access-Control-Allow-Methods: GET, POST, PUT, DELETE
Access-Control-Allow-Headers: Content-Type, Authorization
