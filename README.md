# 👤 Regras de Negócio – Usuário

## 🖼️ Tela de Login

<img width="675" height="375" alt="login png" src="https://github.com/user-attachments/assets/143204ef-aa40-450b-8d50-ae86fc86b256" />
*Figura 1 – Interface de login do sistema*

---

## 🔐 1. Acesso do Usuário (Login)

### 📌 Descrição

O usuário acessa o sistema informando suas credenciais.

### ⚙️ Regras de Negócio

```pseudo
REGRA: Acesso ao sistema

IF usuario NÃO informar nome OU senha
    THEN impedir acesso

IF usuario NÃO estiver cadastrado
    THEN impedir acesso

IF senha incorreta
    THEN registrar tentativa

IF tentativas >= 3
    THEN bloquear acesso do usuario

IF dados válidos
    THEN permitir acesso ao sistema
```

---

## 👤 2. Cadastro de Usuário

### 📌 Descrição

O usuário pode criar uma conta para acessar o sistema.

### ⚙️ Regras de Negócio

```pseudo
REGRA: Criação de conta

IF usuario NÃO informar nome OU senha
    THEN impedir cadastro

IF nome já estiver em uso
    THEN impedir cadastro

IF senha.length < 8
    THEN impedir cadastro

IF dados válidos
    THEN permitir criação da conta
```

---

## 🔄 3. Comportamento do Usuário no Sistema

### ⚙️ Regras de Negócio

```pseudo
REGRA: Sessão do usuário

IF usuario realizar login
    THEN iniciar sessão

IF sessão ativa
    THEN usuario pode acessar funcionalidades

IF usuario solicitar logout
    THEN encerrar sessão
```

---

## 🧠 4. Participação no Teste Socioemocional

### ⚙️ Regras de Negócio

```pseudo
REGRA: Responder questionário

IF usuario iniciar teste
    THEN deve responder todas as perguntas

IF usuario NÃO responder todas as perguntas
    THEN impedir finalização

IF teste concluído
    THEN calcular pontuação do usuario
```

```pseudo
REGRA: Cálculo da pontuação

pontuacao_total = soma das respostas

pontuacao_maxima = numero_perguntas * 10
```

---

## 🎮 5. Uso do Simulador

### ⚙️ Regras de Negócio

```pseudo
REGRA: Acesso ao simulador

IF usuario possuir pontuação baixa
    THEN acesso ao simulador é obrigatório

IF usuario possuir pontuação média
    THEN acesso ao simulador é opcional

IF usuario possuir pontuação alta
    THEN acesso ao simulador é opcional
```

---

## 📊 6. Evolução do Usuário

```pseudo
REGRA: Progresso do usuário

IF usuario melhorar desempenho
    THEN atualizar pontuação

IF usuario atingir pontuação >= 80
    THEN classificar como "APTO"
```

---

## ⚠️ 7. Validações do Usuário

```pseudo
REGRA: Validação de dados

IF campos obrigatórios vazios
    THEN impedir ações

IF nome duplicado
    THEN impedir cadastro

IF senha fora do padrão
    THEN impedir cadastro
```

---

## 🔒 8. Responsabilidade do Usuário

```pseudo
REGRA: Uso da conta

usuario é responsável por suas credenciais

usuario NÃO deve compartilhar acesso

usuario deve utilizar o sistema de forma adequada
```

---

## 🎯 9. Objetivo

Garantir que o usuário utilize o sistema de forma correta, segura e eficiente, promovendo o desenvolvimento de competências socioemocionais.

