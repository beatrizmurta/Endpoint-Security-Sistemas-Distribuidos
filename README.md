# Endpoint Security — Sistemas Distribuídos

## Sprint 1: Configuração Inicial e Definição de Padrões de Segurança

### Objetivo  
Estabelecer a base do projeto com foco em segurança, incluindo:

- Configuração segura do repositório no GitHub  
- Definição de padrões de segurança para os endpoints da API

---

## 1. Configuração do Repositório

### Boas práticas

- **Branches protegidas**  
  A branch `main` foi protegida para evitar alterações diretas. Alterações só são permitidas via pull request.

- **Revisão obrigatória**  
  Toda solicitação de pull request deve ser aprovada por pelo menos um membro da equipe antes de ser mesclada.

- **Commits verificados**  
  Foi habilitada a exigência de commits assinados digitalmente, garantindo a autoria e integridade das alterações.

**Referência:**  
[Boas práticas do GitHub para repositórios](https://docs.github.com/pt/repositories/creating-and-managing-repositories/best-practices-for-repositories)

---

## 2. Padrões de Segurança da API

### Métodos HTTP utilizados

| Método  | Descrição                           |
|---------|-------------------------------------|
| GET     | Leitura de dados                    |
| POST    | Criação de novos recursos           |
| PUT     | Atualização completa de recursos    |
| DELETE  | Exclusão de recursos                |

### Autenticação

- Utilização de **JWT (JSON Web Tokens)** como método principal de autenticação.
- Os tokens garantem sessões seguras e controlam o acesso aos recursos da API.

### Política de CORS

Foi implementada uma política de CORS restritiva para prevenir acessos indevidos:

```http
Access-Control-Allow-Origin: https://exemplo.com
Access-Control-Allow-Methods: GET, POST, PUT, DELETE
Access-Control-Allow-Headers: Content-Type, Authorization
```

---

## Apresentação das Sprints

Como parte da entrega das Sprints, foi elaborado um vídeo de apresentação contendo os seguintes destaques:

- Melhores práticas de segurança aplicadas na criação e configuração de um repositório GitHub.
- Definição dos padrões de segurança adotados para a implementação dos endpoints da API.
- Justificativas para o uso de autenticação via JWT e implementação de CORS.
- Organização da equipe no uso de branches e revisões para garantir integridade do código.

https://drive.google.com/drive/folders/1CAlzojKteYz55jF4AU3Geqklne7gxwF3?usp=sharing

O vídeo tem como objetivo apresentar de forma visual e didática o conteúdo técnico da sprint, reforçando a importância da segurança desde o início do desenvolvimento do sistema.

---

> Este documento faz parte do projeto da disciplina de Sistemas Distribuídos, com foco em segurança de endpoints desde a configuração inicial do ambiente de desenvolvimento.
