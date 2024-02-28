# Projeto Integrador: Pequena Loja de Materiais Esportivos

## Sumário

1. [Resumo](#resumo)
2. [Planejamento](#planejamento)
    - [Planejamento da Rede Local](#planejamento-da-rede-local)
    - [Cabeamento Interno e Externo](#cabeamento-interno-e-externo)
    - [Crimpagem e Certificação de Rede](#crimpagem-e-certificação-de-rede)
    - [Avaliação de Custo-Benefício](#avaliação-de-custo-benefício)
    - [Projeto Físico da Rede LAN](#projeto-físico-da-rede-lan)
    - [Projeto Lógico da Rede LAN](#projeto-lógico-da-rede-lan)
    - [Detalhes do Projeto Utilizando o Packet Tracer](#detalhes-do-projeto-utilizando-o-packet-tracer)
3. [Conclusão](#conclusão)

---

## Resumo

Este projeto tem como objetivo configurar uma rede no Packet Tracer para atender às necessidades de uma pequena loja de materiais esportivos, proporcionando conectividade segura para funcionários, uma solução de vendas, vigilância por câmera e acesso Wi-Fi para clientes.

## Planejamento

### Planejamento da Rede Local

Na fase de planejamento, foi feita uma análise das necessidades da rede local, considerando fatores como tamanho da área a ser coberta, número de dispositivos, largura de banda necessária e orçamento disponível. O plano detalhado incluirá a escolha dos equipamentos, como desktops, switches e cabos.

### Cabeamento Interno e Externo

Na fase de cabeamento, serão realizados o estudo e a instalação do cabeamento interno e externo da rede local. Isso inclui a escolha adequada de cabos, conectores e dispositivos de proteção. O cabeamento será instalado de acordo com as normas técnicas relevantes.

### Crimpagem e Certificação de Rede

Na fase de crimpagem e certificação, será realizado o teste de conformidade do cabeamento instalado. O teste de certificação é uma medida essencial para garantir a qualidade do cabeamento e o desempenho da rede.

### Avaliação de Custo-Benefício

Na fase de avaliação de custo-benefício, será analisada a relação entre o custo total do projeto e os benefícios obtidos. A avaliação incluirá fatores como economia de tempo, melhoria na eficiência da rede e redução de problemas de conectividade.

### Projeto Físico da Rede LAN

O projeto físico da rede LAN será baseado nos seguintes requisitos:

* A rede deve cobrir toda a área da loja.
* A rede deve suportar no mínimo 16 hosts fixos incluindo câmeras de segurança.
* A rede deve fornecer largura de banda de pelo menos 100 Mbps.

Com base nesses requisitos, o projeto físico da rede LAN será o seguinte:

* A rede será baseada em uma topologia estrela.
* O switch principal será instalado no centro da loja.
* Será instalado um roteador Wi-Fi para gerar uma rede para clientes e funcionários.
* O cabeamento será feito com cabos Cat 5e.

### Projeto Lógico da Rede LAN

O projeto lógico da rede LAN será baseado nos seguintes requisitos:

* A rede principal da loja deve seguir o seguinte padrão: 192.168.0.0/24
* A máscara da rede será: 255.255.255.0
* Uma segunda rede criada usando um roteador Wi-Fi.
* A rede Wi-Fi terá o seguinte endereço de IP: 192.168.20.0/24 e máscara padrão: 255.255.255.0, evitando que ela se comunique e interfira com a rede principal da loja.
* O Wi-Fi será transmitido nas frequências de 2,4 GHz e 5 GHz, e será separado uma transmissão exclusiva para clientes terem acesso à rede como “convidado”.

Com base nesses requisitos, o projeto lógico da rede LAN será o seguinte:

* A rede principal da loja utilizará endereços IPs fixos em seus hosts, para melhor controle dos mesmos.
* A rede Wi-Fi, devido à rotatividade de clientes/convidados, utilizará IPs dinâmicos providos pelo sistema DHCP do próprio roteador Wi-Fi.
* A rede convidado (guest), que será provida aos clientes, terá acesso total à internet, mas por questões de segurança não será capaz de ver ou comunicar com os outros dispositivos que também estarão usando a rede.

### Detalhes do Projeto Utilizando o Packet Tracer

#### Topologia da Rede:

* Topologia estrela, usando o Switch como elemento central.

#### Computadores e Dispositivos:

* 1 Switch central para fazer a conexão dos dispositivos.
* 1 modem e roteador para fazer a conexão com o provedor de internet. Rede escolhida de classe C (192.168.0.0/24).
* 1 Gateway (roteador) para criar uma segunda rede, sendo esta uma rede Wi-Fi destinada a clientes e funcionários. Foi utilizada uma segunda rede de classe C (192.168.20.0/24).

#### Área de Escritório:

* 2 desktops para Administração e Recursos Humanos.
* 1 desktop para marketing e divulgações em redes sociais e afins.
* 1 desktop para gerenciamento de estoque.
* 1 desktop servidor (menor custo que um servidor convencional) para gerenciar funcionários.
* 1 impressora multifuncional jato de tinta, equipada com scanner para uso de funcionários do escritório.

#### Área de Vendas:

* 2 desktops para frente de caixa.
* 2 desktops para consultas ao estoque e assistência a clientes.
* 1 impressora laser monocromática para uso na área de vendas.

#### Área de Segurança:

* 1 desktop para monitoramento do feed de câmeras e monitoramento da rede.

#### Cabeamento:

Foi utilizado o cabo Cat5e (UTP), o tipo mais comum de cabo Ethernet, amplamente utilizado em redes domésticas e de pequenas empresas. É econômico e atende à maioria das necessidades.

#### Gestão de Estoque em Nuvem:

Essas soluções podem ajudar a melhorar a eficiência operacional, simplificar processos e permitir que os proprietários se concentrem em expandir seus negócios.
* Acessibilidade Remota: Acesso fácil aos dados de estoque e vend

as de qualquer lugar com conexão à internet.
* Atualizações Automáticas: Recebimento automático de atualizações de software sem a necessidade de instalações manuais.
* Escalabilidade: Capacidade de expandir o sistema conforme a loja cresce, adicionando usuários ou funcionalidades conforme necessárias.
* Redução de Custos: Evita custos iniciais de hardware e oferece modelos de assinatura mensal.
* Integração com Outras Ferramentas: Facilidade de integração com outras ferramentas úteis para negócios, como contabilidade e análise de dados.
* Segurança de Dados: Proteção adicional dos dados dos clientes com medidas de segurança avançadas, como criptografia e backups regulares.

## Conclusão

Este projeto foi desenvolvido com o objetivo de fornecer uma rede local eficiente e econômica para uma pequena loja esportiva. O projeto atende aos requisitos do cliente e está em conformidade com as normas técnicas relevantes.
