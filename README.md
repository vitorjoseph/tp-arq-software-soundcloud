 
# Sound Cloud

## Resumo

<div align="justify">
 
As aplicações da SoundCloud reutilizam sua API pública; o uso de uma camada de serviços RESTful parecia uma decisão sólida, mas cada cliente tem suas próprias
necessidades. A SoundCloud está migrando para um modelo onde clientes mantêm suas próprias APIs. Foram necessárias mudanças em arquitetura, tecnologias e processo. Nesta
apresentação vamos explorar os desafios enfrentados e decisões tomadas.<br>

 
O presente trabalho buscará demonstrar a evolução da arquitetura de serviços na SoundCloud nos últimos anos, bem como abordará os desafios que foram encontrados e as
soluções adotadas. Em específico, será abordo a arquitetura Backends for Frontends (BFF), descrevendo seus prós e contras e os principais tópicos relacionados a essa
abordagem.

<div align="center">
  <b>Backends for Frontends no SoundCloud em 2021</b><br><br>
  <img src="./Imagens/bff-2021.png" alt="Arquitetura Backends for Frontends"></b><br>
   <b>Figura 1. Arquitetura BFF.<br>
</div> 

A SoundCloud pioneirou o padrão arquitetônico Backends for Frontends em 2013, enquanto se afastava de um modelo datado de abordagem eat-your-own-dog-food que envolvia o uso de uma única API (a API pública) tanto para aplicativos oficiais quanto para integrações de terceiros, porém a necessidade de escalar operacional e
organizacionalmente levou a uma migração de uma arquitetura baseada em monólito para uma arquitetura de microsserviços. A proliferação de novos microsserviços, aliada à
introdução de uma API privada/interna para o monólito (transformando efetivamente o monólito em outro microsserviço), abriu a porta para novas e inovadoras APIs
dedicadas para alimentar nossas interfaces, nascendo assim a BFF, sendo um momento emocionante para a empresa, pois permitiu autonomia para equipes, juntamente com
muitas outras vantagens que serão discutidas em breve. 
 


</div>
