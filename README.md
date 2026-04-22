# 👤 Regras de Negócio – Usuário

---

## 🖼️ Tela de Login

<img width="675" height="375" alt="login png" src="https://github.com/user-attachments/assets/143204ef-aa40-450b-8d50-ae86fc86b256" />
*Figura 1 – Interface de login do sistema*

---

## 🔐 1. Acesso do Usuário (Login)

### 📌 Descrição
O usuário acessa o sistema informando suas credenciais.

### 📋 Regras de Negócio

- O usuário deve informar nome e senha para acessar o sistema  
- Não é permitido acessar o sistema com campos vazios  
- O usuário deve estar previamente cadastrado  
- Caso a senha esteja incorreta, uma tentativa de acesso deve ser registrada  
- Após 3 tentativas inválidas, o acesso do usuário deve ser bloqueado temporariamente  
- Caso os dados estejam corretos, o acesso deve ser permitido  

---

## 👤 2. Cadastro de Usuário

### 📌 Descrição
O usuário pode criar uma conta para acessar o sistema.

### 📋 Regras de Negócio

- O usuário deve informar nome e senha para se cadastrar  
- Não é permitido cadastro com campos vazios  
- O nome do usuário deve ser único no sistema  
- A senha deve possuir no mínimo 8 caracteres  
- Caso os dados estejam válidos, o cadastro deve ser realizado com sucesso  

---

## 🔄 3. Comportamento do Usuário no Sistema

### 📋 Regras de Negócio

- Ao realizar login com sucesso, a sessão do usuário deve ser iniciada  
- Enquanto a sessão estiver ativa, o usuário pode acessar as funcionalidades do sistema  
- O usuário pode encerrar a sessão a qualquer momento (logout)  

---

## 🧠 4. Participação no Teste Socioemocional

### 📋 Regras de Negócio

- O usuário pode iniciar o teste socioemocional  
- Todas as perguntas devem ser respondidas para concluir o teste  
- Não é permitido finalizar o teste com perguntas em branco  
- Ao finalizar o teste, a pontuação do usuário deve ser calculada  
- A pontuação é baseada na soma das respostas selecionadas  

---

## 🎮 5. Uso do Simulador

### 📋 Regras de Negócio

- O acesso ao simulador depende do desempenho do usuário no teste  
- Usuários com pontuação baixa devem obrigatoriamente utilizar o simulador  
- Usuários com pontuação média podem utilizar o simulador opcionalmente  
- Usuários com pontuação alta também podem acessar o simulador de forma opcional  

---

## 📊 6. Evolução do Usuário

### 📋 Regras de Negócio

- O desempenho do usuário deve ser atualizado conforme suas interações  
- O usuário pode melhorar sua pontuação ao utilizar o simulador  
- Caso atinja uma pontuação alta, o usuário deve ser classificado como apto  

---

## ⚠️ 7. Validações do Usuário

### 📋 Regras de Negócio

- Campos obrigatórios não podem estar vazios  
- Não é permitido cadastro com nome duplicado  
- A senha deve seguir critérios mínimos de segurança  

---

## 🔒 8. Responsabilidade do Usuário

### 📋 Regras de Negócio

- O usuário é responsável por suas credenciais de acesso  
- Não deve compartilhar login e senha com terceiros  
- Deve utilizar o sistema de forma adequada e ética  

---

## 🎯 9. Objetivo

Garantir que o usuário utilize o sistema de forma correta, segura e eficiente, promovendo o desenvolvimento de competências socioemocionais.
