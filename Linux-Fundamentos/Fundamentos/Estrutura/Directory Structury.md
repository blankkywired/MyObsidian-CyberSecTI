https://www.geeksforgeeks.org/linux-directory-structure/
### Estrutura basica do Linux:

a estrutura básica dos diretorios linux se encontra em uma unica pasta, chamada de pasta raiz do sistema Linux , chamada de apenas "/ "


![[Pasted image 20241017191835.png]]
==No sistema operacional Linux/Unix tudo é considerado um arquivo(File) , até mesmo os próprios diretórios são considerados arquivos pelo sistema.==


## Tipos de arquivos no sistema Linux

##### Arquivos gerais: 
Chamados tambem de arquivos ordinários, pode ser uma imagem , video, programa ou um arquivo de texto como por exemplo uma anotação em um bloco de notas

##### Arquivos do Diretório / Arquivos Diretório:
São como containers para outros diretórios ou arquivos possuindo assim uma estrutura hierarquica

È considerado um tipo especial de arquivo, podendo ser acessado pelos comandos cd ( change directory) ou mkdir (make directory)


##### Arquivos de Dispositivo / Device Files:

arquivos de dispositivo são uma categoria especial de arquivos linux e são fundamentais para representar um dispositivo físico como mouse , impressora , teclados, placas de rede etc. 

	*Ficam alocados no diretório /dev*


Por que Tudo é considerado um arquivo no sistema Linux / Unix?

Flexibilidade : Possibilita criar dispositivos virtuais e expandir as possibilidades do sistema gerando inúmeras possibilidades

Segurança: Controle de acesso aos dispositivos internos e externos por meio de permissões de arquivo tradicionais

Facilita o processamento pelo Sistema Operacional para gerenciar o hardware de maneira homogenea 



### Hierarquia dos Diretórios do sistema Linux




| Categoria |                                                                   Descrição                                                                   |
| :-------: | :-------------------------------------------------------------------------------------------------------------------------------------------: |
|     /     | O mais alto nivel da hierarquia dos diretórios, chamada de pasta raiz, e contem todos os arquivos que possibilitam a inicialização do sistema |
|   /bin    |                                                 Contém todos os comandos binários essenciais                                                  |
|   /boot   |                                  Trata-se do conjuntos de arquivos necessários para inicialização do sistema                                  |
|   /dev    |              Armazena todos os arquivos de dispositivos para facilitar o acesso ao hardware e periféricos conectados ao sistema               |
|   /etc    |                                                                                                                                               |
|           |                                                                                                                                               |
|           |                                                                                                                                               |
|           |                                                                                                                                               |
|           |                                                                                                                                               |
|           |                                                                                                                                               |
|           |                                                                                                                                               |
|           |                                                                                                                                               |
|           |                                                                                                                                               |
|           |                                                                                                                                               |
|           |                                                                                                                                               |



