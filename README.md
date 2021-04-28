# proj-redes-tcpip
Projeto da disciplina de Arquitetura de Redes TCP-IP

A imagem abaixo exibe os IPs de interfaces configuradas e conectadas.
![alt text](<https://github.com/italomoraes/proj-redes-tcpip/blob/main/Resources/Topologia.png>)

Dentro do arquivo "Config Scripts.txt" - na raiz deste projeto - você encontrará as linhas utilizadas para efetuar as configurações em cada um dos roteadores.

Os roteadores R1, R2 e R3 estão contidos em uma rede fechada e têm acesso às redes uns de outros, porém, o único roteador com acesso externo a essa rede é R2 e somente ele consegue se comunicar para fora da rede.

O Roteador R6 (MikroTik) faz parte de seu próprio sistema e tem máscara de forma que apenas ele dispositivo e mais um sejam conectados às suas subredes ("/30").

Os roteadores R4 e R5 estão em outra rede fechada e apenas R4 pode acessar a rede externa.
