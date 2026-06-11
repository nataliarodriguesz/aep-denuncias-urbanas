# 🌱 Cidade Sustentável – Sistema de Denúncias Urbanas

O projeto tem como objetivo facilitar a comunicação entre moradores e administradores responsáveis pela manutenção da cidade, permitindo o registro, acompanhamento e gerenciamento de denúncias relacionadas a problemas urbanos, como buracos em vias públicas, iluminação defeituosa, descarte irregular de lixo e outros incidentes que impactam a qualidade de vida da população.

---

## 📋 Objetivos do Projeto

O sistema foi idealizado para:

- Centralizar denúncias urbanas em um único ambiente;
- Permitir que moradores acompanhem o andamento de suas solicitações;
- Auxiliar administradores no gerenciamento e priorização de ocorrências;
- Aplicar conceitos de Engenharia de Software, Programação Orientada a Objetos e Estruturas de Dados.

---

## 👥 Perfis de Usuário

### Morador

O morador pode:

- Registrar denúncias;
- Consultar denúncias registradas;
- Acompanhar o status das solicitações.

### Administrador

O administrador pode:

- Visualizar denúncias recebidas;
- Alterar o status das denúncias;
- Consultar o histórico de ações;
- Priorizar ocorrências.

---

# 🏗️ Modelagem do Sistema

O desenvolvimento foi iniciado através da modelagem dos requisitos utilizando diagramas UML.

## 📌 Diagrama de Casos de Uso

Representa os atores do sistema e suas respectivas funcionalidades.

Principais atores:

- Morador
- Administrador

Principais casos de uso:

- Registrar denúncia
- Consultar denúncias
- Acompanhar status
- Visualizar denúncias
- Alterar status
- Consultar histórico
- Priorizar denúncia

---

## 📌 Diagrama de Classes de Alto Nível

Define as principais entidades do sistema e seus relacionamentos.

Classes principais:

- Usuario
- Morador
- Administrador
- Denuncia
- Historico
- FilaDenuncias

---

## 📌 Diagrama de Classes de Baixo Nível

Detalha atributos, métodos e relacionamentos entre as classes.

Foram aplicados conceitos como:

- Herança
- Encapsulamento
- Abstração
- Associação entre objetos

---

# ☕ Implementação Orientada a Objetos (Java)

A modelagem foi implementada em Java para demonstrar a aplicação dos conceitos de Programação Orientada a Objetos.

## Classe Abstrata Usuario

Classe base do sistema.

```java
Usuario
├── Morador
└── Administrador
```

Responsável por atributos e comportamentos comuns:

- id
- nome
- email
- senha

Métodos:

- login()
- logout()
- alterarSenha()

---

## Classe Morador

Especialização da classe Usuario.

Funcionalidades:

- registrarDenuncia()
- consultarDenuncias()
- acompanharStatus()

---

## Classe Administrador

Especialização da classe Usuario.

Funcionalidades:

- visualizarDenuncias()
- alterarStatus()
- priorizarDenuncia()
- consultarHistorico()

---

## Classe Denuncia

Representa uma ocorrência registrada no sistema.

Atributos principais:

- id
- titulo
- descricao
- bairro
- urgencia
- status

Funcionalidades:

- atualizarStatus()
- registrarAcao()
- exibirHistorico()

---

# 📚 Estruturas de Dados

Um dos requisitos do projeto era a utilização de estruturas de dados implementadas manualmente.

Foram desenvolvidas:

## 🔄 Fila de Denúncias (FIFO)

Implementada através das classes:

- FilaDenuncias
- NoFila

A fila segue o princípio:

**First In, First Out**

A primeira denúncia registrada é a primeira a ser processada.

Operações implementadas:

- enfileirar()
- desenfileirar()
- imprimir()

Representação:

```text
[Denúncia 1] -> [Denúncia 2] -> [Denúncia 3]
```

---

## 📌 Pilha de Histórico (LIFO)

Implementada através das classes:

- Historico
- NoPilha

A pilha segue o princípio:

**Last In, First Out**

A última ação registrada é exibida primeiro.

Operações implementadas:

- push()
- pop()
- imprimir()

Representação:

```text
Topo
 ↓
[Ação 3]
[Ação 2]
[Ação 1]
```

---

# 🌐 Interface Web

Além da modelagem em Java, foi desenvolvida uma interface web para simular o funcionamento do sistema.

Tecnologias utilizadas:

- HTML5
- CSS3
- JavaScript

A interface possui:

### Área do Morador

- Cadastro de denúncias
- Consulta de denúncias
- Acompanhamento de status

### Área do Administrador

- Visualização das denúncias
- Alteração de status
- Consulta do histórico

---

## Fluxo de Funcionamento

```text
Morador
   ↓
Registra denúncia
   ↓
Fila de denúncias
   ↓
Administrador visualiza
   ↓
Atualiza status
   ↓
Histórico registra ação
```

---

# 📁 Estrutura do Projeto

```text
CidadeSustentavel/

├── diagramas/
│   ├── CasoDeUso.png
│   ├── ClasseAltoNivel.png
│   └── ClasseBaixoNivel.png
│
├── java/
│   ├── Usuario.java
│   ├── Morador.java
│   ├── Administrador.java
│   ├── Denuncia.java
│   ├── Historico.java
│   ├── NoPilha.java
│   ├── FilaDenuncias.java
│   ├── NoFila.java
│   └── Main.java
│
├── web/
│   ├── css/
│   ├── js/
│   └── imagens/
│
├── index.html
└── README.md
```

---

# 🎓 Conceitos Aplicados

Durante o desenvolvimento foram aplicados conceitos de:

- Engenharia de Software
- UML
- Programação Orientada a Objetos
- Herança
- Encapsulamento
- Abstração
- Estruturas de Dados
- Desenvolvimento Web
- Organização de Projetos

---

# 🚀 Autor

Desenvolvido como atividade da disciplina de Engenharia de Software.

**Cidade Sustentável – Sistema de Denúncias Urbanas**