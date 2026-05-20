# Simulações de Redes com Mininet

Este repositório contém os relatórios, comandos e scripts de simulação de redes de computadores utilizando a ferramenta **Mininet**. Estes experimentos fazem parte das atividades acadêmicas voltadas ao estudo de infraestrutura de redes e Internet das Coisas (IoT).

## Estrutura do Repositório

O projeto está organizado em diretórios, cada um contendo o relatório detalhado e as imagens comprobatórias das simulações:

*   📁 [**Trabalho 1**](./Trabalho_1/): 
    *   Simulação de uma topologia em **Árvore (Tree)** com 3 níveis de profundidade e ramificação 2 (8 hosts e 7 switches).
    *   Inspeções de portas, testes com `pingall` e análises de vazão com servidor/cliente TCP usando `iperf`.

*   📁 [**Trabalho 2**](./Trabalho_2/): 
    *   **Questão 1:** Simulação de uma topologia **Linear** com 8 switches, aplicando limitação de banda de 20, 30 e 40 Mbps e validando o impacto no throughput.
    *   **Questão 2:** Criação de uma **Topologia Customizada em Python** operando com um controlador manual. Inclui a programação direta de regras em switches OpenFlow (via `ovs-ofctl`) para controlar a comunicação baseando-se especificamente nos endereços MAC dos hosts.

## Tecnologias Utilizadas

*   **Mininet:** Plataforma principal para a emulação rápida da rede.
*   **Python:** Para criação programática de bibliotecas de topologias customizadas.
*   **Open vSwitch (OVS):** Switch virtual subjacente, configurado através de comandos `ovs-ofctl` para simulação manual de fluxos (SDN na prática).
*   **Análise de Tráfego:** `ping`, `iperf` para taxa de transferência (throughput) e `tcpdump` para inspeção avançada dos pacotes ICMP/ARP nas interfaces.
