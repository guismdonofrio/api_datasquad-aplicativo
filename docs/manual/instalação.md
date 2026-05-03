# Manual de Instalação (JavaFX + MaterialFX)

## Pré-requisitos

---

### 2. Instalando o "Cérebro" (Java JDK)
Para o sistema rodar, o computador precisa entender a linguagem Java.

1.  Acesse o site da [Oracle](https://www.oracle.com/java/technologies/downloads/) e baixe o **JDK 17** ou superior (versão "Windows x64 Installer").
2.  Abra o arquivo baixado e clique em **Next** (Próximo) em todas as telas até aparecer **Finish** (Finalizar).

---

---

### 3. Instalando o Banco de Dados (MySQL)
É aqui que as informações do sistema ficam guardadas.

1.  Baixe o [MySQL Installer](https://dev.mysql.com/downloads/installer/).
2.  Escolha a instalação **"Developer Default"**.
3.  **Atenção na Senha:** Durante a instalação, ele pedirá para você criar uma senha de "Root". **Anote essa senha no papel.** Você precisará dela para o sistema conectar ao banco.
4.  Siga clicando em **Next** e **Execute** até o fim.

---


### 4. Preparando o IntelliJ (Onde o sistema mora)
Como as pastas já estão no repositório, vamos trazê-las para o seu computador.

1.  **Baixar o Projeto:** Vá ao link do repositório que te enviaram. Clique no botão verde escrito **"Code"** e depois em **"Download ZIP"**.
2.  **Extrair:** Vá na sua pasta de "Downloads", clique com o botão direito no arquivo baixado e escolha **"Extrair Tudo"**.
3.  **Abrir o IntelliJ:**
    *   Abra o programa IntelliJ IDEA (ícone roxo e preto).
    *   Clique em **Open** (Abrir).
    *   Navegue até a pasta que você extraiu no passo anterior e clique em **OK**.

---

### 5. Configurando o JavaFX (O Visual)
O JavaFX é o que faz as janelas e botões aparecerem.

1.  No IntelliJ, vá em **File** -> **Project Structure**.
2.  Em **SDK**, verifique se o Java que instalamos no Passo 2 está selecionado.
3.  Se o projeto usar bibliotecas externas, o IntelliJ mostrará uma pequena notificação no canto inferior direito dizendo "Maven scripts found". Clique em **Load Maven Changes**.

---

## Clonar o Projeto

Clone o repositório [backend](https://github.com/rubensvnc/BD_2S_backend) com o Git:

```bash
git clone https://github.com/guismdonofrio/api_datasquad-aplicativo.git
```

Ou baixe o ZIP direto pelo GitHub.

---

## Abrindo no IntelliJ

1. Abra o **IntelliJ IDEA**
2. Clique em **"Open"**
3. Selecione a pasta do projeto clonado
4. Aguarde o IntelliJ importar as dependências automaticamente

---

## Execução do Projeto

1. Vá até a classe principal (ex: `Main.java`)
2. Clique com botão direito
3. Clique em **Run**

Ou use:

```
Shift + F10
```

---

## Possíveis Problemas

### ❌ Erro de JavaFX não encontrado

* Verifique se o **module-path** está correto

### ❌ Tela não abre

* Confirme se o `FXMLLoader` está apontando pro caminho certo

---

## Observações

* O projeto utiliza **JavaFX para interface gráfica**
* Recomenda-se usar **IntelliJ atualizado**
