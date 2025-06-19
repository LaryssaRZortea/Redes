# Trabalho: Integração de habilidades - 2025/1  
**Discipli74a:** Redes de Computadores  
**Curso:** Engenharia de Computação / Tecnologia em Análise e Desenvolvimento de Sistemas  

**Nome: Laryssa Rayane Zortea**  
**RA: 2037874**  

---

## Tarefa 1: Sub-Redes

|     Sub- Rede     |       IPv4 - Sub-Rede       |       IPv4 - Máscara      |             IPv6 - Sub-Rede/Prefixo            |
| :---------------: | :-------------------------: | :-----------------------: | :--------------------------------------------: |
|    Pato Branco    | 200.136.**74**.*00*          | 255.255.255.*192*         |    2001:DB8:CAFE:**74***00*::/64               |
| Francisco Beltrão | 200.136.**74**.*64*          | 255.255.255.*224*         |    2001:DB8:CAFE:**74***01*::/64               |
|   Dois Vizinhos   | 200.136.**74**.*96*          | 255.255.255.*224*         |    2001:DB8:CAFE:**74***02*::/64               |
|       Toledo      | 200.136.**74**.*128*         | 255.255.255.*224*         |    2001:DB8:CAFE:**74***03*::/64               |
|     Media74eira    | 200.136.**74**.*160*         | 255.255.255.*224*         |    2001:DB8:CAFE:**74***04*::/64               |
|    Sa74ta Hele74a   | 200.136.**74**.*192*         | 255.255.255.*224*         |    2001:DB8:CAFE:**74***05*::/64               |
|       pb-vit      | 200.136.**74**.*224*         | 255.255.255.*252*         |    2001:DB8:CAFE:**74**FF::/112                |
|       vit-fb      | 200.136.**74**.*228*         | 255.255.255.*252*         |    2001:DB8:CAFE:**74**FF::*1*:0/112           |
|       fb-ita      | 200.136.**74**.*232*         | 255.255.255.*252*         |    2001:DB8:CAFE:**74**FF::*2*:0/112          |
|       ita-pb      | 200.136.**74**.*236*         | 255.255.255.*252*         |    2001:DB8:CAFE:**74**FF::*3*:0/112          |
|       ita-dv      | 200.136.**74**.*240*         | 255.255.255.*252*         |    2001:DB8:CAFE:**74**FF::*4*:0/112          |



## Tarefa 2: Endereçamento de Dispositivos

|         Dispositivo        | Interface | IPv4                | IPv4 - Máscara    | IPv4 - Gateway     | IPv6/Prefixo (GUA)                    | IPv6 (LLA) | IPv6-Gateway |
| :------------------------: | :-------: | ------------------- | ----------------- | ------------------ | ------------------------------------- | ---------- | ------------ |
|             PC1            |    74IC    | 200.136.**74**.*3*   | 255.255.255.*192* | 200.136.**74**.*1*  | 2001\:DB8\:CAFE:**74***00*::*3*/64    | EUI-64     | FE80::1      |
|             PC2            |    74IC    | 200.136.**74**.*4*   | 255.255.255.*192* | 200.136.**74**.*1*  | 2001\:DB8\:CAFE:**74***00*::*4*/64    | EUI-64     | FE80::1      |
|             PC3            |    74IC    | 200.136.**74**.*67*  | 255.255.255.*224* | 200.136.**74**.*65* | 2001\:DB8\:CAFE:**74***01*::*3*/64    | EUI-64     | FE80::1      |
|             PC4            |    74IC    | 200.136.**74**.*68*  | 255.255.255.*224* | 200.136.**74**.*65* | 2001\:DB8\:CAFE:**74***01*::*4*/64    | EUI-64     | FE80::1      |
|             PC5            |    74IC    | 200.136.**74**.*99*  | 255.255.255.*224* | 200.136.**74**.*97* | 2001\:DB8\:CAFE:**74***02*::*3*/64    | EUI-64     | FE80::1      |
|             PC6            |    74IC    | 200.136.**74**.*100* | 255.255.255.*224* | 200.136.**74**.*97* | 2001\:DB8\:CAFE:**74***02*::*4*/64    | EUI-64     | FE80::1      |
|     Switch-Pato Branco     |    SVI    | 200.136.**74**.*2*   | 255.255.255.*192* | 200.136.**74**.*1*  | -                                     | -          | -            |
|  Switch-Francisco Beltrão  |    SVI    | 200.136.**74**.*66*  | 255.255.255.*224* | 200.136.**74**.*65* | -                                     | -          | -            |
|    Switch-Dois Vizinhos    |    SVI    | 200.136.**74**.*98*  | 255.255.255.*224* | 200.136.**74**.*97* | -                                     | -          | -            |
|    Roteador-Pato Branco    |   Fa0/0   | 200.136.**74**.*1*   | 255.255.255.*192* | -                  | 2001\:DB8\:CAFE:**74**00::*1*/64      | FE80::1    | -            |
|    Roteador-Pato Branco    |  Se0/0/0  | 200.136.**74**.*225* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**74**FF::*0*:*1*/112 | EUI-64     | -            |
|    Roteador-Pato Branco    |  Se0/0/1  | 200.136.**74**.*238* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**74**FF::*3*:*2*/112 | EUI-64     | -            |
| Roteador-Francisco Beltrão |   Fa0/0   | 200.136.**74**.*65*  | 255.255.255.*224* | -                  | 2001\:DB8\:CAFE:**74***01*::*1*/64    | FE80::1    | -            |
| Roteador-Francisco Beltrão |  Se0/0/0  | 200.136.**74**.*233* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**74**FF::*2*:*1*/112 | EUI-64     | -            |
| Roteador-Francisco Beltrão |  Se0/0/1  | 200.136.**74**.*230* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**74**FF::*1*:*2*/112 | EUI-64     | -            |
|      Roteador-Vitorino     |  Se0/0/0  | 200.136.**74**.*229* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**74**FF::*1*:*1*/112 | EUI-64     | -            |
|      Roteador-Vitorino     |  Se0/0/1  | 200.136.**74**.*226* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**74**FF::*0*:*2*/112 | EUI-64     | -            |
|     Roteador-Itapejara     |  Se0/0/0  | 200.136.**74**.*237* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**74**FF::*3*:*1*/112 | EUI-64     | -            |
|     Roteador-Itapejara     |  Se0/0/1  | 200.136.**74**.*234* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**74**FF::*2*:*2*/112 | EUI-64     | -            |
|     Roteador-Itapejara     |   Fa0/1   | 200.136.**74**.*241* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**74**FF::*4*:*1*/112 | EUI-64     | -            |
|   Roteador-Dois Vizinhos   |   Fa0/0   | 200.136.**74**.*97*  | 255.255.255.*224* | -                  | 2001\:DB8\:CAFE:**74***02*::*1*/64    | FE80::1    | -            |
|   Roteador-Dois Vizinhos   |   Fa0/1   | 200.136.**74**.*242* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**74**FF::*4*:*2*/112 | EUI-64     | -            |


---

## Tarefa 3: Tabela de Roteamento
>Observação: inserir o número de linhas necessárias em cada tabela

### Roteador Pato Branco
#### IPv4
|  Rede de Destino |     Máscara     |   Próximo Salto   | Interface de Saída |  
|:----------------:|:---------------:|:-----------------:|:------------------:|  
| 200.136.**74**.64  | 255.255.255.224 | 200.136.**74**.226 | Se0/0/0            | 
| 200.136.**74**.96  | 255.255.255.224 | 200.136.**74**.226 | Se0/0/0            |
| 200.136.**74**.228 | 255.255.255.252 | 200.136.**74**.226 | Se0/0/0            |
| 200.136.**74**.232 | 255.255.255.252 | 200.136.**74**.226 | Se0/0/0            |
| 200.136.**74**.240 | 255.255.255.252 | 200.136.**74**.226 | Se0/0/0            |

#### IPv6
|  Rede de Destino /Prefixo         |         Próximo Salto           | Interface de Saída |  
|:---------------------------------:|:-------------------------------:|:------------------:| 
| 2001:DB8:CAFE:**74**_01_::/64     | 2001:DB8:CAFE:**74**FF::_0_:_2_ | Se0/0/0            |
| 2001:DB8:CAFE:**74**_02_::/64     | 2001:DB8:CAFE:**74**FF::_0_:_2_ | Se0/0/0            |
| 2001:DB8:CAFE:**74**FF::_1_:0/112 | 2001:DB8:CAFE:**74**FF::_0_:_2_ | Se0/0/0            |
| 2001:DB8:CAFE:**74**FF::_2_:0/112 | 2001:DB8:CAFE:**74**FF::_0_:_2_ | Se0/0/0            |
| 2001:DB8:CAFE:**74**FF::_4_:0/112 | 2001:DB8:CAFE:**74**FF::_0_:_2_ | Se0/0/0            |


#### Roteador Francisco Beltrão
#### IPv4
|  Rede de Destino |     Máscara     |   Próximo Salto   | Interface de Saída |  
|:----------------:|:---------------:|:-----------------:|:------------------:| 
| 200.136.**74**.0   | 255.255.255.192 | 200.136.**74**.234 | Se0/0/0            |
| 200.136.**74**.96  | 255.255.255.224 | 200.136.**74**.234 | Se0/0/0            | 
| 200.136.**74**.224 | 255.255.255.252 | 200.136.**74**.234 | Se0/0/0            | 
| 200.136.**74**.236 | 255.255.255.252 | 200.136.**74**.234 | Se0/0/0            |
| 200.136.**74**.240 | 255.255.255.252 | 200.136.**74**.234 | Se0/0/0            |

#### IPv6
|  Rede de Destino /Prefixo         |         Próximo Salto           | Interface de Saída |  
|:---------------------------------:|:-------------------------------:|:------------------:| 
| 2001:DB8:CAFE:**74**_00_::/64     | 2001:DB8:CAFE:**74**FF::_2_:_2_ | Se0/0/0            |
| 2001:DB8:CAFE:**74**_02_::/64     | 2001:DB8:CAFE:**74**FF::_2_:_2_ | Se0/0/0            |
| 2001:DB8:CAFE:**74**FF::_0_:0/112 | 2001:DB8:CAFE:**74**FF::_2_:_2_ | Se0/0/0            |
| 2001:DB8:CAFE:**74**FF::_3_:0/112 | 2001:DB8:CAFE:**74**FF::_2_:_2_ | Se0/0/0            |
| 2001:DB8:CAFE:**74**FF::_4_:0/112 | 2001:DB8:CAFE:**74**FF::_2_:_2_ | Se0/0/0            |

#### Roteador Vitorino
#### IPv4
|  Rede de Destino |     Máscara     |   Próximo Salto   | Interface de Saída |  
|:----------------:|:---------------:|:-----------------:|:------------------:| 
| 200.136.**74**.0   | 255.255.255.192 | 200.136.**74**.230 | Se0/0/0            |
| 200.136.**74**.64  | 255.255.255.224 | 200.136.**74**.230 | Se0/0/0            |
| 200.136.**74**.96  | 255.255.255.224 | 200.136.**74**.230 | Se0/0/0            |
| 200.136.**74**.232 | 255.255.255.252 | 200.136.**74**.230 | Se0/0/0            |
| 200.136.**74**.236 | 255.255.255.252 | 200.136.**74**.230 | Se0/0/0            |
| 200.136.**74**.240 | 255.255.255.252 | 200.136.**74**.230 | Se0/0/0            |

#### IPv6
|  Rede de Destino /Prefixo         |         Próximo Salto           | Interface de Saída |  
|:---------------------------------:|:-------------------------------:|:------------------:| 
| 2001:DB8:CAFE:**74**_00_::/64     | 2001:DB8:CAFE:**74**FF::_1_:_2_ | Se0/0/0            |
| 2001:DB8:CAFE:**74**_01_::/64     | 2001:DB8:CAFE:**74**FF::_1_:_2_ | Se0/0/0            |
| 2001:DB8:CAFE:**74**_02_::/64     | 2001:DB8:CAFE:**74**FF::_1_:_2_ | Se0/0/0            |
| 2001:DB8:CAFE:**74**FF::_2_:0/112 | 2001:DB8:CAFE:**74**FF::_1_:_2_ | Se0/0/0            | 
| 2001:DB8:CAFE:**74**FF::_3_:0/112 | 2001:DB8:CAFE:**74**FF::_1_:_2_ | Se0/0/0            |
| 2001:DB8:CAFE:**74**FF::_4_:0/112 | 2001:DB8:CAFE:**74**FF::_1_:_2_ | Se0/0/0            |


#### Roteador Itapejara D'Oeste
#### IPv4
|  Rede de Destino |     Máscara     |   Próximo Salto   | Interface de Saída |  
|:----------------:|:---------------:|:-----------------:|:------------------:| 
| 200.136.**74**.0   | 255.255.255.192 | 200.136.**74**.238 | Se0/0/0           |
| 200.136.**74**.64  | 255.255.255.224 | 200.136.**74**.238 | Se0/0/0           | 
| 200.136.**74**.96  | 255.255.255.224 | 200.136.**74**.242 | Fa0/1             | 
| 200.136.**74**.224 | 255.255.255.252 | 200.136.**74**.238 | Se0/0/0           |
| 200.136.**74**.228 | 255.255.255.252 | 200.136.**74**.238 | Se0/0/0           |

#### IPv6
|  Rede de Destino /Prefixo         |         Próximo Salto           | Interface de Saída |  
|:---------------------------------:|:-------------------------------:|:------------------:|  
| 2001:DB8:CAFE:**74**_00_::/64     | 2001:DB8:CAFE:**74**FF::_3_:_2_ | Se0/0/0            |
| 2001:DB8:CAFE:**74**_01_::/64     | 2001:DB8:CAFE:**74**FF::_3_:_2_ | Se0/0/0            |
| 2001:DB8:CAFE:**74**_02_::/64     | 2001:DB8:CAFE:**74**FF::_4_:_2_ | Fa0/1              |
| 2001:DB8:CAFE:**74**FF::_0_:0/112 | 2001:DB8:CAFE:**74**FF::_3_:_2_ | Se0/0/0            |
| 2001:DB8:CAFE:**74**FF::_1_:0/112 | 2001:DB8:CAFE:**74**FF::_3_:_2_ | Se0/0/0            |


#### Roteador Dois Vizinhos
#### IPv4
|  Rede de Destino |     Máscara     |   Próximo Salto   | Interface de Saída |  
|:----------------:|:---------------:|:-----------------:|:------------------:| 
| 200.136.**74**.0   | 255.255.255.192 | 200.136.**74**.241 | Fa0/1             |
| 200.136.**74**.64  | 255.255.255.224 | 200.136.**74**.241 | Fa0/1             | 
| 200.136.**74**.224 | 255.255.255.252 | 200.136.**74**.241 | Fa0/1             |
| 200.136.**74**.228 | 255.255.255.252 | 200.136.**74**.241 | Fa0/1             |
| 200.136.**74**.232 | 255.255.255.252 | 200.136.**74**.241 | Fa0/1             | 
| 200.136.**74**.236 | 255.255.255.252 | 200.136.**74**.241 | Fa0/1             | 


#### IPv6
|  Rede de Destino /Prefixo         |         Próximo Salto           | Interface de Saída |  
|:---------------------------------:|:-------------------------------:|:------------------:|  
| 2001:DB8:CAFE:**74**_00_::/64     | 2001:DB8:CAFE:**74**FF::_4_:_1_ | Fa0/1              |
| 2001:DB8:CAFE:**74**_01_::/64     | 2001:DB8:CAFE:**74**FF::_4_:_1_ | Fa0/1              | 
| 2001:DB8:CAFE:**74**FF::_0_:0/112 | 2001:DB8:CAFE:**74**FF::_4_:_1_ | Fa0/1              |
| 2001:DB8:CAFE:**74**FF::_1_:0/112 | 2001:DB8:CAFE:**74**FF::_4_:_1_ | Fa0/1              | 
| 2001:DB8:CAFE:**74**FF::_2_:0/112 | 2001:DB8:CAFE:**74**FF::_4_:_1_ | Fa0/1              |
| 2001:DB8:CAFE:**74**FF::_3_:0/112 | 2001:DB8:CAFE:**74**FF::_4_:_1_ | Fa0/1              |


---
## Tarefa 5: Testes de Conectividade (Opcional, mas recomeddado)
## Tabela 1
| Origem | Destino                                     | Tipo de Teste | Resultado       |
|:------:|:-------------------------------------------:|:-------------:|:---------------:|
| PC0    | 200.136.74.3 (PC1)                           | ping IPv4     | (4/0) |
| PC0    | 200.136.74.4 (PC2)                           | ping IPv4     | (4/0) |
| PC0    | 200.136.74.67 (PC3)                          | ping IPv4     | (4/0) |
| PC0    | 200.136.74.68 (PC4)                          | ping IPv4     | (4/0) |
| PC0    | 200.136.74.99 (PC5)                          | ping IPv4     | (4/0) |
| PC0    | 200.136.74.100 (PC6)                         | ping IPv4     | (4/0) |
| PC0    | 200.136.74.2 (Switch-Pato Branco)            | ping IPv4     | (4/0) |
| PC0    | 200.136.74.66 (Switch-Francisco Beltrão)     | ping IPv4     | (4/0) |
| PC0    | 200.136.74.98 (Switch-Dois Vizinhos)         | ping IPv4     | (4/0) |
| PC0    | 200.136.74.1 (Roteador-Pato Branco)          | ping IPv4     | (4/0) |
| PC0    | 200.136.74.225 (Roteador-Pato Branco)        | ping IPv4     | (4/0) |
| PC0    | 200.136.74.238 (Roteador-Pato Branco)        | ping IPv4     | (4/0) |
| PC0    | 200.136.74.65 (Roteador-Francisco Beltrão)   | ping IPv4     | (4/0) |
| PC0    | 200.136.74.233 (Roteador-Francisco Beltrão)  | ping IPv4     | (4/0) |
| PC0    | 200.136.74.230 (Roteador-Francisco Beltrão)  | ping IPv4     | (4/0) |
| PC0    | 200.136.74.229 (Roteador-Vitorino)           | ping IPv4     | (4/0) |
| PC0    | 200.136.74.226 (Roteador-Vitorino)           | ping IPv4     | (4/0) |
| PC0    | 200.136.74.237 (Roteador-Itapejara)          | ping IPv4     | (4/0) |
| PC0    | 200.136.74.234 (Roteador-Itapejara)          | ping IPv4     | (4/0) |
| PC0    | 200.136.74.241 (Roteador-Itapejara)          | ping IPv4     | (4/0) |
| PC0    | 200.136.74.97 (Roteador-Dois Vizinhos)       | ping IPv4     | (4/0) |
| PC0    | 200.136.74.242 (Roteador-Dois Vizinhos)      | ping IPv4     | (4/0) |
| PC0    | 2001:DB8:CAFE:7400::3 (PC1)                  | ping IPv6     | (4/0) |
| PC0    | 2001:DB8:CAFE:7400::4 (PC2)                  | ping IPv6     | (4/0) |
| PC3    | 2001:DB8:CAFE:7401::3 (PC3)                  | ping IPv6     | (4/0) |
| PC3    | 2001:DB8:CAFE:7401::4 (PC4)                  | ping IPv6     | (4/0) |
| PC5    | 2001:DB8:CAFE:7402::3 (PC5)                  | ping IPv6     | (4/0) |
| PC5    | 2001:DB8:CAFE:7402::4 (PC6)                  | ping IPv6     | (4/0) |
| PC0    | 2001:DB8:CAFE:7400::1 (Roteador-Pato Branco) | ping IPv6     | (4/0) |
| PC3    | 2001:DB8:CAFE:7401::1 (Roteador-Francisco Beltrão)| ping IPv6 | (4/0) |
| PC5    | 2001:DB8:CAFE:7402::1 (Roteador-Dois Vizinhos)| ping IPv6    | (4/0) |


---

## Checklist para Entrega
- [ ] Tarefa 1: Tabela de Sub-Redes preenchida corretamente 
- [ ] Tarefa 2: Tabela de Endereçamento preenchida corretamente para todos os dispositivos  
- [ ] Tarefa 3: Tabela de Roteamento completa para todos os roteadores  
- [ ] Tarefa 4: Topologia funcional no Packet Tracer
- [ ] Tarefa 5: Testes realizados e documentados (opcional)  
- [ ] Documento salvo no formato .md, conforme modelo disponibilizado, com nome no padrão: Trabalho_Redes_nome_RA.md

## LISTA DE CÓDIGOS UTILIZADOS NOS ROTEADORES TRABALHO

**ROTEADOR PATO BRANCO**
```
enable
configure terminal
hostname r-pb-lrz

interface fa0/0
description LAN Pato Branco
ip address 200.136.74.1 255.255.255.192
ipv6 address 2001:DB8:CAFE:7400::1/64
ipv6 address FE80::1 link-local 
no shutdown

interface Se0/0/0 
description Enlace pb-vit
ip address 200.136.74.225 255.255.255.252
ipv6 address 2001:DB8:CAFE:74FF::1/112 
clock rate 56000
no shutdown

interface Se0/0/1 
description Enlace pb-ita
ip address 200.136.74.238 255.255.255.252
ipv6 address 2001:DB8:CAFE:74FF::3:2/112
no shutdown

end
write

--------------
   IP ROUTE   
--------------
enable
configure terminal
ipv6 unicast-routing

ip route 200.136.74.64 255.255.255.224 200.136.74.226
ip route 200.136.74.96 255.255.255.224 200.136.74.226
ip route 200.136.74.228 255.255.255.252 200.136.74.226
ip route 200.136.74.232 255.255.255.252 200.136.74.226
ip route 200.136.74.240 255.255.255.252 200.136.74.226

ipv6 route 2001:DB8:CAFE:7401::/64 2001:DB8:CAFE:74FF::0:2
ipv6 route 2001:DB8:CAFE:7402::/64 2001:DB8:CAFE:74FF::0:2
ipv6 route 2001:DB8:CAFE:74FF::1:0/112 2001:DB8:CAFE:74FF::0:2
ipv6 route 2001:DB8:CAFE:74FF::2:0/112 2001:DB8:CAFE:74FF::0:2
ipv6 route 2001:DB8:CAFE:74FF::4:0/112 2001:DB8:CAFE:74FF::0:2
```

**ROTEADOR FRANCISCO BELTRÃO**
```
enable
configure terminal
hostname r-fb-lrz

interface fa0/0
description LAN Francisco Beltrao
ip address 200.136.74.65 255.255.255.224
ipv6 address 2001:DB8:CAFE:7401::1/64
ipv6 address FE80::1 link-local
no shutdown

interface Se0/0/0 
description Enlace fb-ita
ip address 200.136.74.233 255.255.255.252
ipv6 address 2001:DB8:CAFE:74FF::2:1/112
clock rate 56000
no shutdown

interface Se0/0/1 
description Enlace fb-vit
ip address 200.136.74.230 255.255.255.252
ipv6 address 2001:DB8:CAFE:74FF::1:2/112
no shutdown

end
write

--------------------------------
   IP ROUTE FRANCISCO BELTRÃO   
--------------------------------
enable
configure terminal
ipv6 unicast-routing

ip route 200.136.74.0 255.255.255.192 200.136.74.234
ip route 200.136.74.96 255.255.255.224 200.136.74.234
ip route 200.136.74.224 255.255.255.252 200.136.74.234
ip route 200.136.74.236 255.255.255.252 200.136.74.234
ip route 200.136.74.240 255.255.255.252 200.136.74.234

ipv6 route 2001:DB8:CAFE:7400::/64 2001:DB8:CAFE:74FF::2:2
ipv6 route 2001:DB8:CAFE:7402::/64 2001:DB8:CAFE:74FF::2:2
ipv6 route 2001:DB8:CAFE:74FF::0:0/112 2001:DB8:CAFE:74FF::2:2
ipv6 route 2001:DB8:CAFE:74FF::3:0/112 2001:DB8:CAFE:74FF::2:2
ipv6 route 2001:DB8:CAFE:74FF::4:0/112 2001:DB8:CAFE:74FF::2:2
```
**ROTEADOR VITORINO**
```
enable
configure terminal
hostname r-vit-lrz

interface Se0/0/0 
description Enlace vit-fb
ip address 200.136.74.229 255.255.255.252
ipv6 address 2001:DB8:CAFE:74FF::1:1/112
clock rate 56000
no shutdown

interface Se0/0/1 
description Enlace vit-pb
ip address 200.136.74.226 255.255.255.252
ipv6 address 2001:DB8:CAFE:74FF::0:2/112
no shutdown

end
write

--------------
   IP ROUTE   
--------------
enable
configure terminal
ipv6 unicast-routing

ip route 200.136.74.0 255.255.255.192 200.136.74.230
ip route 200.136.74.64 255.255.255.224 200.136.74.230
ip route 200.136.74.96 255.255.255.224 200.136.74.230
ip route 200.136.74.232 255.255.255.252 200.136.74.230
ip route 200.136.74.236 255.255.255.252 200.136.74.230
ip route 200.136.74.240 255.255.255.252 200.136.74.230

ipv6 route 2001:DB8:CAFE:7400::/64 2001:DB8:CAFE:74FF::1:2
ipv6 route 2001:DB8:CAFE:7401::/64 2001:DB8:CAFE:74FF::1:2
ipv6 route 2001:DB8:CAFE:7402::/64 2001:DB8:CAFE:74FF::1:2
ipv6 route 2001:DB8:CAFE:74FF::2:0/112 2001:DB8:CAFE:74FF::1:2
ipv6 route 2001:DB8:CAFE:74FF::3:0/112 2001:DB8:CAFE:74FF::1:2
ipv6 route 2001:DB8:CAFE:74FF::4:0/112 2001:DB8:CAFE:74FF::1:2
```

**ROTEADOR ITAPEJARA**
```
enable
configure terminal
hostname r-ita-lrz

interface Se0/0/0 
description Enlace ita-pb
ip address 200.136.74.237 255.255.255.252
ipv6 address 2001:DB8:CAFE:74FF::3:1/112
clock rate 56000
no shutdown

interface Se0/0/1 
description Enlace ita-fb
ip address 200.136.74.234 255.255.255.252
ipv6 address 2001:DB8:CAFE:74FF::2:2/112
no shutdown

interface fa0/1
description Enlace ita-dv
ip address 200.136.74.241 255.255.255.252
ipv6 address 2001:DB8:CAFE:74FF::/112
ipv6 address FE80::1 link-local
no shutdown

end
write

--------------
   IP ROUTE   
--------------
enable
configure terminal
ipv6 unicast-routing

ip route 200.136.74.0 255.255.255.192 200.136.74.238
ip route 200.136.74.64 255.255.255.224 200.136.74.238
ip route 200.136.74.96 255.255.255.224 200.136.74.242
ip route 200.136.74.224 255.255.255.252 200.136.74.238
ip route 200.136.74.228 255.255.255.252 200.136.74.238

ipv6 route 2001:DB8:CAFE:7400::/64 2001:DB8:CAFE:74FF::3:2
ipv6 route 2001:DB8:CAFE:7401::/64 2001:DB8:CAFE:74FF::3:2
ipv6 route 2001:DB8:CAFE:7402::/64 2001:DB8:CAFE:74FF::4:2
ipv6 route 2001:DB8:CAFE:74FF::0:0/112 2001:DB8:CAFE:74FF::3:2
ipv6 route 2001:DB8:CAFE:74FF::1:0/112 2001:DB8:CAFE:74FF::3:2
```

**ROTEADOR DOIS VIZINHOS**
```
enable
configure terminal
hostname r-dv-lrz

interface fa0/0
description LAN Dois Vizinhos
ip address 200.136.74.97 255.255.255.224
ipv6 address 2001:DB8:CAFE:7402::1/64
ipv6 address FE80::1 link-local 
no shutdown

interface fa0/1
description Enlace nn-nn
ip address 200.136.74.242 255.255.255.252
ipv6 address 2001:DB8:CAFE:74FF::4:2/112
ipv6 address FE80::1 link-local
no shutdown

end
write

--------------
   IP ROUTE   
--------------
enable
configure terminal
ipv6 unicast-routing

ip route 200.136.74.0 255.255.255.192 200.136.74.241
ip route 200.136.74.64 255.255.255.224 200.136.74.241
ip route 200.136.74.224 255.255.255.252 200.136.74.241
ip route 200.136.74.228 255.255.255.252 200.136.74.241
ip route 200.136.74.232 255.255.255.252 200.136.74.241
ip route 200.136.74.236 255.255.255.252 200.136.74.241

ipv6 route 2001:DB8:CAFE:7400::/64 2001:DB8:CAFE:74FF::4:1
ipv6 route 2001:DB8:CAFE:7401::/64 2001:DB8:CAFE:74FF::4:1
ipv6 route 2001:DB8:CAFE:74FF::0:0/112 2001:DB8:CAFE:74FF::4:1
ipv6 route 2001:DB8:CAFE:74FF::1:0/112 2001:DB8:CAFE:74FF::4:1
ipv6 route 2001:DB8:CAFE:74FF::2:0/112 2001:DB8:CAFE:74FF::4:1
ipv6 route 2001:DB8:CAFE:74FF::3:0/112 2001:DB8:CAFE:74FF::4:1
```
