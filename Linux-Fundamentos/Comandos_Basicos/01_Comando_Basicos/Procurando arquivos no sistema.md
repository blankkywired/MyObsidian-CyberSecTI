Uma das possibilidades do Linux é sua alta eficiencia e velocdade para fazer pesquisas de aquivos no sistema que na qual o usuário tem acesso.

### find   
Usamos o [[Linux-Fundamentos/Comandos_Basicos/02_Comandos_Basicos/Procurando arquivos e diretorios.md|find]] quando se pressupõe que o usuário sabe o nome do arquivo porem a localização no diretório em que se encontra é desconhecida. 

```shell-session
tryhackme@linux1:~$ find -name passwords.txt
./folder1/passwords.txt
tryhackme@linux1:~$
```

```shell-session
blankky@blankky-Inspiron-15-3520:~$ find -name ativ5.6.py
./Documents/Programação/Python Introducao_Logica_Programacao/Cap5/ativ5.6.py
blankky@blankky-Inspiron-15-3520:~$
```


Como no exemplo acima, o arquivo password.txt se encontra dentro da pasta folder1

###### Dica 
caso o usuário não saiba exatamente o nome do arquivo porem saiba a extensão do arquivo, como por exemplo (.pdf / .xsl / .txt / .py / . mp4)

é possivel fazer um scaneamento no sistema filtrando arquivos com a mesma extensão usando ( * )

```shell-session
tryhackme@linux:~$ find -name  *.txt 
./folder1/passwords.txt` 
./Documents/todo.txt
```
o asterico fica junto com o .txt 


tambem pode usar o comando  finde seguido de ( / ) para procurar o arquivo no diretório todo, assim, fazendo um scanneamento completo na pasta


### grep

Serve para filtrar por padrões em arquivos  em uma busca em arquivos de texto.

O `grep` é ideal para analisar arquivos de log e encontrar mensagens de erro, avisos ou informações relevantes

`grep "padrão" arquivo`
- **"padrão":** A palavra ou expressão que você está procurando.
- **arquivo:** O arquivo onde a busca será realizada.


Ex:
```shell-session
tryhackme@linux:~$ grep "THM" access.log
procurando pelo prefixo "THM" dentro do arquivo access.log
```


