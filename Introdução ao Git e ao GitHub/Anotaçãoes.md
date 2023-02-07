Link para download do Git: https://git-scm.com/downloads
O Git Bash é um terminal extendido para otimizar ouso do Git.

## Introdução ao Git e ao GitHub:

### Importância do Git:

​	O Git é um softaware de versionamento de código

### Comandos básicos para um bom desempenho no terminal:

- **Git GUI** = Interface Gráfica

- **Git CLI** = Command Line Interface

#### Comandos Windows

- **cd** = Navegar entre pastas --> cd .. retorna para a pasta anterior

- **dir** = Lista diretórios

- **mkdir** = Cria uma pasta

- **del** = deleta um diretório

- **cls** = Limpa um terminal

- **TAB** = Autocomplete

- **echo hello > (arquivo)** = Cria o arquivo caso não tenha na pasta

#### Comandos Linux

- **cd** = Navegar entre pastas --> cd .. retorna para a pasta anterior

- **ls** = Lista diretórios
  - **ls -a** = mostra arquivos ocultos

- **mkdir** = Cria uma pasta

- **rm -rf** = deleta um diretório

- **clear ou ctrl + L** = Limpa um terminal

- **TAB** = Autocomplete

- **echo hello > (arquivo)** = Cria o arquivo caso não tenha na pasta

- **mv “arquivo” ./“diretório”** = move arquivos em um diretório para outro diretório

### Como é o funcionamento do Git:

​	SHA1 (Secure Hash Algorithm) = algorítimo de encriptação que gera um conjunto de caracteres.

​	Identificador de 40 dígitos.

### Objetos internos do Git responsáveis pelo versionamento do código:

- **blobs** = bloco básico de composição (guarda o sha1 do arquivo, armazena metadados do Git (tipo de objeto, tamanho da string, etc.))

			echo 'conteudo' | git hash-object --stdin
			fc31e91b26cf85a55e072476de7f263c89260eb1

```
**passa os metadados para a string**
		echo -e 'blob 9\0conteudo' | openssl sha1
		(stdin)= fc31e91b26cf85a55e072476de7f263c89260eb1
```

- **trees (árvores)** = armazena nomes, armazenam blobs, podem apontar para um blob ou para outras árvores.

- **commits** = aponta para árvores, pra outros commits realizados anteriormente...

### Iniciando o Git e criando um commit:

**No git bash**

- **git init** = cria um repositório

  - **configura o git**

    - git config --global user.email “meu email”

    - git config --global user.name meu usuário

- **git add**
  - git add *

  - git add .

  - git add nome_arquivo

- **git commit**
  - git commit -m “adicionar comentários”


