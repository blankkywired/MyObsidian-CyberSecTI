### Comandos basicos

#### echo
Mostra na tela do terminal qualquer texto que digitarmos
```shell-session
tryhackme@linux1:~$ echo Hello World
Hello World
```

#### whoami
Exibe o nome do usuário que está logado no momento na máquina
```shell-session
tryhackme@linux1:~$ whoami
tryhackme
```
#### ls - List Files in current directory
Lista os arquivos do atual diretório em que o usuário se encontra no sistema


```shell-session
tryhackme@linux1:~$ ls
'Important Files' 'My Documents' 'Notes Pictures'
```
Não é necessário estar necessariamente dentro de um diretório para poder lista-lo

È possivel listar um diretorio especifico sem se locomover ate ele , usando ls nome do diretorio

Ex: ls Downloads

#### cd - Change Directory (Mudar diretório)

serve para navegar entre os diretórios do sistema, podendo entrar em outras pastas 

Ex:
```shell-session
tryhackme@linux1:~$ cd Downloads
```
entra na pasta Downloads


#### cat - Concatenate

Função: Exibir o conteudo de um arquivo

```shell-session
tryhackme@linux1:~$ cat teste.txt`
Mensagem dentro do arquivo teste.txt
```
Dica: é possivel mostrar o conteudo de texto dentro de um arquivo sem navegar ate o arquivo, apenas usando o endereçamento do arquivo como por exemplo:

```shell-session
tryhackme@linux1:~$ cat /home/ubuntu/Documents/teste.txt
```


