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

## Configurações inicias git

### email 
Com o comando `git --config --global user.email "email"` definimos o e-mail padrão. Adicionando a flag `--unset` removemos esse padrão.


### username
Com o comando `git --config --global user.name "username"` definimos o e-username padrão

## Ciclo de vida dos arquivos no git 

### Untracked
São os arquivos que o git ainda não tem conhecimento, ou seja, não foram adicionados ao git.

### Unmodified
Arquivos que já estão no git, mas que ainda não sofreram modificação

### Modified 
Quando modificamos qualquer coisa em um arquivo Unmodified, ele se torna Modified.

### Staged
Quando executamos o comando `git add` e adicionamos os arquivos, seja *Untracked ou Modified*, eles ficam nesse estágio *Staged*. Estes, são arquivos que estão sendo preparados para o commit.

### Commit
Quando o comando de commit é executado, os arquivos que são *Modified* são envelopados em uma versão do repositório e voltam para o estágio *Unmodified*. E o código é salvo no git.

## Ambientes de desenvolvimento

### Working Directory
Diretório onde estão situados os arquivos que estamos modificando. 

### Stage Area
Região onde os arquivos *Staged* irão ficar.

### Local Repository
Onde os commits são armazenados.

## Verificar Status
Com o comando `git status` conseguimos verificar os estado de todos os arquivos do repositório.

## Primeiro comando no git
Sempre que queremos iniciar um repositório no git devemos usar o comando `git init`. A partir disso, será criada, no diretório atual, uma pasta *.git* que contem os arquivos necessários para o funcionamento do git.

## Adicionar à fila
Se quisermos adicionar arquivos que tenham sido alterados para a fila de envio, usamos o comando `git add [arquivo>]`. *arquivo* com o valor * adiciona todos os arquivos do diretório.

## Enviar modificações
O comando `git commit -m "nome"` envia as modificações e as salva no histórico com o nome que definimos.

## Flags interessantes para usar no terminal

* `-a` -> Mostra pastas ocultas
