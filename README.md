# ACC202302_A3

## 💻 Sobre o Projeto

Trabalho de Criação de Rede Corporativa desenvolvido no Segundo Semestre de 2023 na Primeira fase do Técnologo de Análise e Desenvolvimento de Sistemas.

## 🧶 Elementos

Rede corporativa contendo um total de 512 endereços separados em **2 Filiais** em uma mesma região metropolitana.

<!-- prettier-ignore -->
|Detalhes| |
|-------- | - |
|IPv4 Rede| 192.168.0.0/23 255.255.254.0|
|Filial A | 10.10.0.0/24|
|Filial B | 10.10.1.0/24|




## 📰 LOGs

### ✅ 18/11/23:
 *`234bc97:`*
Inicialização do projeto. Foi definida a topologia, sendo separada em Filial A, contendo um Switch-PT para a centralização com 8 portas GigabitEthernet, sendo:
-  1 dedicada a comunicação com o roteador
- 4 destinadas aos servidores DNS, HTTP, DHCP e SMTP
- e 3 para os Switchs 2960-24TT dos setores de 
    - SAC
    - Desenvolvimento 
    - e Comercial.

### ✅ 19/11/23:
*`fb2509c:`*
Configuração dos switchs da Filial A com a separação das VLANs utilizando um IP genérico. Será definida o IP de cada Sub-rede futuramente.

|VLAN | Numero |
|------- | - |
|SPD - Setor de Processamento de Dados | 10 |
|SAC - Suporte ao Cliente | 20 |
|DEV - Desenvolvimento | 30 |
|CMC - Setor Comercial | 40 |

### 22/11/23:
*`2a70136:`*
Configuração do switch da Filial B com a criação da VLAN do setor ADM - Administrativo.

|VLAN | Numero |
|------- | - |
|ADM - Setor Administrativo | 10 |
|WIFI - Access Point | 20 |

Adicionado notas com os detalhes dos elementos.

### 23/11/23:
*`3974ca6:`*
Merge das alterações do commit anterior