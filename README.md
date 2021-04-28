# proj-redes-tcpip
Projeto da disciplina de Arquitetura de Redes TCP-IP

A imagem abaixo exibe os IPs de interfaces configuradas e conectadas.
![alt text](<https://github.com/italomoraes/proj-redes-tcpip/blob/main/Resources/Topologia.png>)

Dentro do arquivo "Config Scripts.txt" - na raiz deste projeto - você encontrará as linhas utilizadas para efetuar as configurações em cada um dos roteadores.

Os roteadores R1, R2 e R3 estão contidos em uma rede fechada e têm acesso às redes uns de outros, porém, o único roteador com acesso externo a essa rede é R2 e somente ele consegue se comunicar para fora da rede.

O Roteador R6 (MikroTik) faz parte de seu próprio sistema e tem máscara de forma que apenas ele e mais um dispositivo sejam conectados às suas subredes ("/30").

Os roteadores R4 e R5 estão em outra rede fechada e apenas R4 pode acessar a rede externa.

A seguir há um resumo da configuração efetuada em cada interface utilizada dos roteadores.


## R1

### fastEthernet 0/0:
**Subrede:** 10.0.1.0/26<br>
**IP:** 10.0.1.1<br>
**Máscara:** 255.255.255.192<br>

### fastEthernet 1/0:
**Subrede:** 10.0.1.64/26<br>
**IP:** 10.0.1.65<br>
**Máscara:** 255.255.255.192<br>


## R2

### fastEthernet 0/0:
**Subrede:** 10.0.1.0/26<br>
**IP:** 10.0.1.2<br>
**Máscara:** 255.255.255.192<br>

### fastEthernet 1/0:
**Subrede:** 10.0.1.128/26<br>
**IP:** 10.0.1.129<br>
**Máscara:** 255.255.255.192<br>

### gigabitEthernet 2/0:
**Subrede:** 10.0.3.0/30<br>
**IP:** 10.0.3.1<br>
**Máscara:** 255.255.255.252<br>


## R3

### fastEthernet 0/0:
**Subrede:** 10.0.1.128/26<br>
**IP:** 10.0.1.130<br>
**Máscara:** 255.255.255.192<br>

### fastEthernet 1/0:
**Subrede:** 10.0.1.64/26<br>
**IP:** 10.0.1.66<br>
**Máscara:** 255.255.255.192<br>


## R4

### fastEthernet 0/0:
**Subrede:** 10.0.2.0/24<br>
**IP:** 10.0.2.1<br>
**Máscara:** 255.255.255.0<br>

### gigabitEthernet 2/0:
**Subrede:** 10.0.3.4/30<br>
**IP:** 10.0.3.6<br>
**Máscara:** 255.255.255.252<br>


## R5

### fastEthernet 0/0:
**Subrede:** 10.0.2.0/24<br>
**IP:** 10.0.2.2<br>
**Máscara:** 255.255.255.0<br>


## R6 (Mikrotik)

### ether1
**Subrede:** 10.0.3.0/30<br>
**IP:** 10.0.3.2<br>
**Máscara:** 255.255.255.252<br>

### ether2
**Subrede:** 10.0.3.4/30<br>
**IP:** 10.0.3.5<br>
**Máscara:** 255.255.255.252<br>
