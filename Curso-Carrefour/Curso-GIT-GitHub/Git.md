# Git
Programa feito para realizar versionamento de código, criado pelo **Linus Torval**

**OBS**: *Git* != *GitHub*

## Comandos de navegação

* `cd` -> navegar entre as pastas
* `ls` -> exibir o conteúdo da pasta atual
* `mkdir` -> criar uma pasta
* `del/rmdir`(Windows) ou `-rm/-rf`(Unix)

**DICA**: `Ctrl + L` no Linux limpa o terminal automaticamente

**OUTRA DICA**: `echo` é um comando de terminal que escreve. Se fizermos `echo [arquivo1] > [arquivo2]`. Escrevemos o conteúdo do primeiro no segundo

## Funcionamento

### SHA
Funções hash que realizam criptografia gerando segurança ao git. É gerado um conjunto de caracteres de 40 dígitos único.

### Objetos internos

#### Blobs
Os **blobs** são metadados que guardam o tamanho do arquivo. Nele temos uma string *blob* indicando que é um blob e, antes do conteúdo, temos a string *\0*

#### Tree
Tem uma indicação para os blobs e para os **commits* ou outras trees. Além de ter, também, o nome do arquivo.

#### Commits
Aponta para uma tree, para um parente(um commit anterior a ela), para o autor e para uma mensagem. E o **timestamp** que é o horário que foi criado.

## Chaves SSH e Tokens

### Chave SSH
Forma de estabelecer uma conexão criptografada confiável entre duas máquinas

#### Como gerar uma chave SSH 

*empty for no passphrase*

Faça `ssh-keygen -t ed25519 -C email`. E automatizamos o processo fazendo `eval $(ssh-agent -s)` e fazer `ssh-add id_ed25519` 
