### Criando Arquivos




#### Comando touch
Serve para criar um arquivo vazio:

```shell-session
blankky@htb[/htb]$ touch <name>
```
Exemplo:
```shell-session
blankky@htb[/htb]~$ touch helloWorld.py
```
Criando um arquivo de linguagem de programação python


#### Comando mkdir (make directory)
usado para construir novos diretórios dentro do sistema

```shell-session
blankky@htb[/htb]$ mkdir nome_do_diretorio
```

==*Para criar multiplos diretorios pode-se usar o comando mkdir seguido dos nomes dos diretorios separados por espaço*==

```shell-session
blankky@htb[/htb]$ mkdir diretorio1 diretorio2 diretorio3
```

### Diretórios Pais/Parentes
Diretorios pais/parentes são diretorios que possuem outros diretorios dentro deles, como se fosse as raizes de uma arvore:

```shell-session
blankky@htb[/htb]$ mkdir -p Storage/local/user/documents
```
*No comando acima pede-se para o computador criar um diretorio chamado documents dentro do diretorio user que esse estara dentro do diretorio local que por fim estará dentro do diretorio Storage*

==*O diretorio Storage é o diretorio pai de /local *==
==*O diretorio /local é diretorio pai do diretorio /user*==

##### Criando diretorios pais/parentes
Para construir diretorios parentes utiliza-se o comando mkdir -p ou --parents
para construir multiplos diretorios em hierarquia, se um diretorio ja existir não ira gerar erro.

```shell-session
blankky@htb[/htb]$ mkdir -p Diretorio1/Diretorio2/Diretorio/Diretorio4
```




### Movendo Arquivos

#### Comando mv (Move)
para mover um arquivo de um local para outro lugar basta usar o comando mv seguido do nome do arquivo seguido do novo destino

```shell-session
blankky@htb~$ mv info.txt novoDestino
```

### Renomeando um arquivo
#### comando mv
Para renomear um arquivo basta usar o comando mv seguido do arquivo que deseja renomear e o novo nome do arquivo

```shell-session
blankky@htb~$ mv <file/directory> <renamed file/directory>
```
Exemplo:

Renomeando um arquivo
```shell-session
blankky@htb~$ mv info.txt information.txt
```

Renomeando um diretório:
```shell-session
blankky@htb~$ mv diretorio diretorioRenomeado
```
agora, o diretorio sera renomeado para diretorioRenomeado


### Copiando arquivos 

Comando cp (copy)
Usa-se o comando cp para copiar um arquivo para um novo destino 

```shell-session
blankky@htb~$ cp arquivo novo/diretorio/destino
```

Exemplo
```shell-session
blankky@htb~$ cp info.txt ./Documents/CyberSec/Linux/NovoDestino
```


##### Copiar e Renomear um arquivo 
```shell-session
blankky@htb~$ cp arquivo.txt /home/usuario/documentos/novo_arquivo.txt
```
- **Descrição**: Copia `arquivo.txt` para `documentos` e o renomeia para `novo_arquivo.txt`.
##### Copiar um diretorio recursivamente

```shell-session
blankky@htb~$ cp -r pasta_origem/ /home/usuario/pasta_destino/
```

**Descrição**: Copia a pasta `pasta_origem` e todo seu conteúdo (subpastas e arquivos) para `pasta_destino`


##### Copiar multiplos arquivos para um diretorio 

```shell-session
blankky@htb~$ arquivo1.txt arquivo2.txt /home/usuario/documentos/
```

**Descrição**: Copia `arquivo1.txt` e `arquivo2.txt` para o diretório `documentos`.

### Removendo arquivos 
#### Comando rm (remove)
remove arquivos ou diretórios 
```shell-session
3520:~/Documents/CyberSec/Linux/vimtest$ ls
vim1.txt
blankky@blankky-Inspiron-15-3520:~/Documents/CyberSec/Linux/vimtest$ rm vim1.txt
blankky@blankky-Inspiron-15-3520:~/Documents/CyberSec/Linux/vimtest$ ls
blankky@blankky-Inspiron-15-3520:~/Documents/CyberSec/Linux/vimtest$ 
```
*removendo o arquivo vim1.txt do diretorio chamado vimtest*