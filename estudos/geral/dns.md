# DNS

## Registrant
  Registrante - o Dono do dominio (eu)

## Registrar
  Registrador - entidade que registra o dominio no banco de dados Registry. 
  Ex: Registro.br, hostgator, uol host, locaweb ..;

## Registry
  Registro, banco de dados dos dominios principais, cada Registry tem um dominio principal e a lista dos subdomios dele. 
  O dominio .br fica no NIC.br, todos os  subdominios brasileiros ficam nesse servidor.

## Root Server
  Mantes as definições de DNS os endereços fisicos ips. esse é o DNS


## TDL
  É um banco de dados  onde é registrado os endereços e os ips, como se fosse uma lista telefonica.
  Também é gerenciado pelo NIC.br para o dominio .br

## Authoritative Server
  É um banco de dados que tem todos os endereços da internet no mundo. 



## Caminho
  REGISTRANT busca o  nome do site e do dominio, no REGISTRAR,
  REGISTRAR busca o dominio na lista do REGISTRY,
  REGISTRY confirma o dominio e o sub dominio e retorna o endereço para o REGISTRAR que informa o REGISTRANT que o dominio está disponivel ou não. Em caso do dominios estar livre o REGISTRY passa para o TDL o endereço.
  TDL armazena o endereço recebido no banco de dados dele e disponibiliza para todos os AUTHORITATIVE SERVER ao  longo do mundo.
  AUTHORITATIVE SERVER disponibiliza online os endereços para qualquer pessoa no mundo acessar atravez dos servidores ao redor do mundo.
 

![Diagrama do DNS](/estudos/img/dns.png)



