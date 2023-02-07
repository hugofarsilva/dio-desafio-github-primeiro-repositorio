Link para download do Git: https://git-scm.com/downloads
O Git Bash é um terminal extendido para otimizar ouso do Git.

## Introdução ao Git e ao GitHub:

### Importância do Git:

​	O Git é um softaware de versionamento de código distribuído.

### Comandos básicos para um bom desempenho no terminal:

- **Git GUI** :arrow_right: Interface Gráfica

- **Git CLI** :arrow_right: Command Line Interface

#### Comandos Windows

- **cd** :arrow_right: Navegar entre pastas --> cd .. retorna para a pasta anterior

- **dir** :arrow_right: Lista diretórios

- **mkdir** :arrow_right: Cria uma pasta

- **del** :arrow_right: deleta um diretório

- **cls** :arrow_right: Limpa um terminal

- **TAB** :arrow_right: Autocomplete

- **echo hello > (arquivo)** :arrow_right: Cria o arquivo caso não tenha na pasta

#### Comandos Linux

- **cd** :arrow_right: Navegar entre pastas --> cd .. retorna para a pasta anterior

- **ls** :arrow_right: Lista diretórios
  - **ls -a** :arrow_right: mostra arquivos ocultos

- **mkdir** :arrow_right: Cria uma pasta

- **rm -rf** :arrow_right: deleta um diretório

- **clear ou ctrl + L** :arrow_right: Limpa um terminal

- **TAB** = Autocomplete

- **echo hello > (arquivo)** :arrow_right: Cria o arquivo caso não tenha na pasta

- **mv “arquivo” ./“diretório”** :arrow_right: move arquivos em um diretório para outro diretório

### Como é o funcionamento do Git:

​	SHA1 (Secure Hash Algorithm) = algorítimo de encriptação que gera um conjunto de caracteres.

​	Identificador de 40 dígitos.

### Objetos internos do Git responsáveis pelo versionamento do código:

- **blobs** :arrow_right: bloco básico de composição (guarda o sha1 do arquivo, armazena metadados do Git (tipo de objeto, tamanho da string, etc.))

			echo 'conteudo' | git hash-object --stdin
		fc31e91b26cf85a55e072476de7f263c89260eb1

```
**passa os metadados para a string**
echo -e 'blob 9\0conteudo' | openssl sha1
(stdin)= fc31e91b26cf85a55e072476de7f263c89260eb1
```

- **trees (árvores)** :arrow_right: armazena nomes, armazenam blobs, podem apontar para um blob ou para outras árvores.

- **commits** :arrow_right: aponta para árvores, pra outros commits realizados anteriormente (parent)... 

### Iniciando o Git e criando um commit:

**No git bash**

- **git init** :arrow_right: cria um repositório
  - **configura o git** :arrow_right: sempre usar e-mail e usuários utilizados no GitHub
  - git config --global user.email “meu e-mail”
    
  - git config --global user.name “meu usuário”
  
- **git add** :arrow_right: adiciona alterações no arquivo pra ser feito o commit
  - git add *

  - git add .

  - git add nome_arquivo

- **git commit** :arrow_right: confirma as alterações no arquivo pra serem empurradas para o repositório remoto no GitHub
  - git commit -m “adicionar comentários”

- **git remote** :arrow_right: adiciona meu repositório remoto à minha máquina local
  - git remote add origin “url do repositório no GitHub”

- **git push** :arrow_right: manda o repositório da minha máquina local para o GitHub
  - git push origin master

- **git pull** :arrow_right: pega o repositório modificado no GitHub pra mesclar com o repositório alterado na minha máquina local.

- **git clone** :arrow_right: faz um clone de um repositório remoto no repositório local
  - git clone “url do repositório remoto”


