
#### Operador &

Permite que o usuário rode comandos em segundo plano no terminal , como por exemplo uma tarefa que demanda tempo como a extração de um arquivo ou fazer a cópia de um arquivo.

#### Operador &&

Responsável por possibilitar que mais de um comando seja executado de uma unica vez, exemplo `comando1 && comando2` , porem so irá funcionar se o primeiro comando for executado com sucesso.

```shell-session
tryhackme@linux1:~$ sudo apt install update && upgrade
```


#### Operador >

Serve como um redirecionador de saída de dados, podendo ser usado para encaminhar uma sáida de dados de um arquivo para outro local, como uma pasta
Ex:
```shell-session
 tryhackme@linux1:~$ echo hey > welcome
tryhackme@linux1:~$ cat welcome
hey
```

###### Tambem serve para substituir um arquivo de texto 
como por exemplo substituir o nome password por password123:
```shell-session
tryhackme@linux1:~$ echo password123 > password
tryhackme@linux1:~$ cat password
password123
```



#### Operador >>

Tambem é um redirecionador de saída de dados como o operador > , porem ele redireciona uma saída de dado para um caminho desejado e o sobreescreve o colocando no final do arquivo que desejamos, sem substituir o arquivo.
```shell-session
tryhackme@linux1:~$ echo hello >> welcome
tryhackme@linux1:~$ cat welcome
hey
hello
```

##### Serve tambem para acrescentar uma informação a um arquivo existente sem substituilo

```shell-session
tryhackme@linux1:~$ echo tryhackme >> password
tryhackme@linux1:~$ cat password
password123tryhackme

```

## Resumo 

| Operador / Simbolo |                                                               Descrição                                                                |
| :----------------: | :------------------------------------------------------------------------------------------------------------------------------------: |
|         &          |                                    Permite que o usuário rode comandos em segundo plano no terminal                                    |
|         &&         |                       fornece a possibilidade de combinar vários comandos de uma única vez para serem executados                       |
|         >          |                                                    Redireciona saida de dados para                                                     |
|         >>         | mesma função que o operador > porem não substitue o arquivo, porem sobrescreve o arquivo com as novas informações que o usuário coloca |
