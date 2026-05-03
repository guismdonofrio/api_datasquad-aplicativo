# Manual de Usuário - Sistema de Gestão Acadêmica

## Sumário

Este manual orienta o uso do Sistema de Gestão Acadêmica, desenvolvido para facilitar o processo de produção do cronograma de professores da Fatec - São José dos Campos.

---

## 1. Introdução

### 1.1 Pré-requisitos

- Instalar o sistema usando o manual disponível em: [Manual de Instalação](instalação.md)

### 1.2 Perfis de Usuário

O sistema possui três perfis de usuário, cada um com responsabilidades específicas:

**Administrador**
- Inserir informações de início e fim de semestres letivos
- Cadastrar datas restritas (quando não podem ser inseridas aulas)
- Inserir dados das sprints do semestre
- Cadastrar coordenadores (criar usuário e senha para login)

**Coordenador**
- Gerenciar um curso específico
- Cadastrar professores (criar usuário e senha para login)

**Professor**
- Gerenciar os temas de cada disciplina ao qual está vinculado
- Gerar cronograma de aulas

---

## 2. Instruções para Administrador

### 2.1 Primeiro Acesso

1. Acessar o banco de dados e inserir manualmente um administrador, conforme imagem abaixo.
   [IMAGEM AQUI]

2. Executar o arquivo .jar gerado no passo "Pré-requisitos"

3. Realizar o login com os dados do ADM criado no passo 1, conforme imagem abaixo.
   [IMAGEM AQUI]

### 2.2 Cadastrar Coordenador

1. Pressionar o botão conforme imagem abaixo
   [IMAGEM AQUI]

2. Inserir os dados de cadastro do coordenador e pressionar "Salvar", conforme imagem abaixo.
   [IMAGEM AQUI]

### 2.3 Inserir Dados do Sistema

Se necessário, inserir dados do semestre, sprints e datas restritas, conforme as imagens abaixo:

[IMAGEM AQUI]
[IMAGEM AQUI]
[IMAGEM AQUI]

### 2.4 Corrigir Cadastros

Em caso de cadastro incorreto:

1. Clique no botão conforme imagem abaixo:
   [IMAGEM AQUI]

2. Selecione o registro que deseja excluir, conforme imagem abaixo
   [IMAGEM AQUI]

3. Confirmada a seleção, pressione o botão "Excluir", conforme imagem abaixo
   [IMAGEM AQUI]

---

## 3. Instruções para Coordenador

### 3.1 Primeiro Acesso

1. Executar o arquivo .jar enviado pelo Administrador

2. Inserir os dados de login enviados pelo Administrador

### 3.2 Cadastrar Professor

1. Acessar o botão conforme imagem abaixo
   [IMAGEM AQUI]

2. Inserir os dados de cadastro do professor, conforme imagem abaixo
   [IMAGEM AQUI]

### 3.3 Visualizar Informações de Professores

**Para visualizar as disciplinas de um professor:**

- Pressione o botão conforme imagem abaixo
  [IMAGEM AQUI]

**Para visualizar o cronograma de um professor:**

- Pressione o botão conforme imagem abaixo
  [IMAGEM AQUI]

### 3.4 Corrigir Cadastros

Em caso de cadastro incorreto:

1. Clique no botão conforme imagem abaixo:
   [IMAGEM AQUI]

2. Selecione o registro que deseja alterar ou excluir, conforme imagem abaixo
   [IMAGEM AQUI]

3. Confirmada a seleção, insira os dados para alteração ou exclusão, conforme imagem abaixo
   [IMAGEM AQUI]

4. Pressione o botão "Alterar" para modificar ou "Excluir" para remover, conforme imagem abaixo
   [IMAGEM AQUI]

---

## 4. Instruções para Professor

### 4.1 Primeiro Acesso

1. Executar o arquivo .jar enviado pelo Administrador

2. Inserir os dados de login enviados pelo Coordenador

### 4.2 Cadastrar Temas

1. Acessar o botão para inserir os temas de uma disciplina, conforme imagem abaixo
   [IMAGEM AQUI]

2. Preencher as informações do tema, conforme imagem abaixo
   [IMAGEM AQUI]

   **Observação:** Para preencher as dependências, consulte a seção 4.5 deste manual.

3. Finalizado o preenchimento, pressione o botão "Salvar", conforme imagem abaixo
   [IMAGEM AQUI]

### 4.3 Visualizar Temas Cadastrados

1. Pressione o combobox "Selecione o curso" e escolha o curso desejado, conforme imagem abaixo
   [IMAGEM AQUI]

2. Selecione o combobox "Selecione o semestre" e escolha o semestre correspondente, conforme imagem abaixo
   [IMAGEM AQUI]

### 4.4 Gerar Cronograma

1. Pressione o botão "Gerar cronograma", conforme imagem abaixo
   [IMAGEM AQUI]

O sistema selecionará todos os temas criados para a disciplina e preencherá os dias letivos do semestre, conforme imagem abaixo.

[IMAGEM AQUI]

### 4.5 Configurar Dependências de Temas

Se um tema depende de outro para ser lecionado:

1. Selecione o combobox "Selecione um tema" e pressione o botão "Adicionar", conforme imagem abaixo
   [IMAGEM AQUI]

2. Finalizadas as inserções de dependências, pressione o botão "Salvar", conforme imagem abaixo
   [IMAGEM AQUI]

O sistema entenderá que, para lecionar o tema A, é necessário ter inserido as datas de lecionamento dos temas B, C e D (selecionados ao clicar no botão "Adicionar").

### 4.6 Alterar ou Excluir Temas

**Para alterar um tema:**

1. Selecione um tema dentro da tabela, conforme imagem abaixo
   [IMAGEM AQUI]

2. Os dados, antes bloqueados, estarão visíveis, conforme imagem abaixo
   [IMAGEM AQUI]

3. Altere a informação desejada e pressione o botão "Alterar", conforme imagem abaixo
   [IMAGEM AQUI]

**Para excluir um tema:**

1. Selecione um tema dentro da tabela, conforme imagem abaixo
   [IMAGEM AQUI]

2. Os dados, antes bloqueados, estarão visíveis, conforme imagem abaixo
   [IMAGEM AQUI]

3. Selecione o botão "Excluir", conforme imagem abaixo
   [IMAGEM AQUI]

### 4.7 Alterar ou Cancelar Aulas do Cronograma

**Para alterar uma aula:**

1. Selecione uma linha da tabela cronograma, conforme imagem abaixo
   [IMAGEM AQUI]

2. Os dados, antes bloqueados, estarão visíveis, conforme imagem abaixo
   [IMAGEM AQUI]

3. Altere as informações desejadas e pressione o botão "Alterar", conforme imagem abaixo
   [IMAGEM AQUI]

**Para cancelar uma aula:**

1. Selecione uma linha da tabela cronograma, conforme imagem abaixo
   [IMAGEM AQUI]

2. Os dados, antes bloqueados, estarão visíveis, conforme imagem abaixo
   [IMAGEM AQUI]

3. Insira a informação "Motivo cancelamento" e pressione o botão "Cancelar", conforme imagem abaixo
   [IMAGEM AQUI]

---

**Fim do Manual**
