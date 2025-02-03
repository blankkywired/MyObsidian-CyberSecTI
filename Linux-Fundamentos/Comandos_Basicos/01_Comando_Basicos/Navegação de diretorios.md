

## cd - change directory ( Mudar de diretorio)
```shell-session
blankky@blankky-Inspiron-15-3520:~$ cd Downloads
blankky@blankky-Inspiron-15-3520:~/Downloads$ 

```
*entra dentro da pasta Downloads*
###### Dica: é possivel entrar dentro de uma pasta apenas informando o caminho do diretorio que deseja entrar:
```shell-session
blankky@blankky-Inspiron-15-3520:~$ cd Documents/CyberSec/Linux/
blankky@blankky-Inspiron-15-3520:~/Documents/CyberSec/Linux$ 
```




## cd ..
Voltar um nivel da hierarquia:
```shell-session
blankky@blankky-Inspiron-15-3520:~/Documents/CyberSec/Linux$ cd ..
blankky@blankky-Inspiron-15-3520:~/Documents/CyberSec$ 
```
Voltou uma 'casa' do diretorio

## Propriedades do comando ls 

## ls -a / ls -all
Lista todos os itens visiveis de um diretorio
```shell-session
cry0l1t3@htb[~]$ ls -l

total 32
drwxr-xr-x 2 cry0l1t3 htbacademy 4096 Nov 13 17:37 Desktop
drwxr-xr-x 2 cry0l1t3 htbacademy 4096 Nov 13 17:34 Documents
drwxr-xr-x 3 cry0l1t3 htbacademy 4096 Nov 15 03:26 Downloads
drwxr-xr-x 2 cry0l1t3 htbacademy 4096 Nov 13 17:34 Music
drwxr-xr-x 2 cry0l1t3 htbacademy 4096 Nov 13 17:34 Pictures
drwxr-xr-x 2 cry0l1t3 htbacademy 4096 Nov 13 17:34 Public
drwxr-xr-x 2 cry0l1t3 htbacademy 4096 Nov 13 17:34 Templates
drwxr-xr-x 2 cry0l1t3 htbacademy 4096 Nov 13 17:34 Videos
```
Conteudos de cada colunado comando ls -l

| Tipo de conteudo | Significado                                  |
| ---------------- | -------------------------------------------- |
| drwxr-xr-x       | tipos e permissões                           |
| 2                | Número de hard links ao ficheiro/diretório   |
| `cry0l1t3`       | Dono/Usuario responsável pelo arquivo        |
| htbacademy       | grupo dono do arquivo/diretório              |
| Nov 13 17:37     | Data e hora da ultima modificação do arquivo |
| Desktop          | Nome  do Diretorio/Arquivo                   |
| 4096             | Tamanho do arquivo                           |
#### Dicas:
Não é necessario ir ate determinado diretorio para poder listar o conteudo dos arquivos dentro dele


pode-se usar por exemplo:
**ls pasta1/pasta2/pasta3/pasta4/diretoriofinal** 

mostrando o conteudo do diretorio chamado diretoro final sem precisar se locomover ate ele


## ls -i / inode number - index number
a opção -i do comando ls fornece o numero indexo de um arquivo no diretório. 
```shell-session
blankky@blankky-Inspiron-15-3520:~/Documents/Programação$ ls -i
15867933  HTML_CSS  
15863630 'Python '
```


## ls -a / all 
Lista todos os diretorios e arquivos (visiveis e invisiveis para o usuario)
Os arquivos invisiveis são aqueles que começam com "." tambem chamados de dots files 