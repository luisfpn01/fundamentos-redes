# Fundamentos de Redes - Módulo 3

## Tipos de Redes
    Existem tipos de redes variados, diferentes quanto a tamanho ou meio de transmissão.

### WIRED
    Redes que transmitem informação (protocolos) utilizando cabeamento. Divididos em categorias como Cat5e (1 Gbps);Cat6 (10 Gbps) e Cat6a, Cat7/Cat7a e Cat8 (40Gbps) utilizando conectores RJ45.

### WIRELESS
    Redes que não necessitam de cabos para se comunicar entre pares. O meio de transmissão de pacotes é feito com ondas de rádio de frequências 2.4 GHz, 5 Ghz e as mais novas com 6 Ghz; ou ondas de infravermelho e até, a tecnologia mais atualizada, a luz (Li-Fi). Seguem o padrão Wireless-fidelity (Wi-Fi) e se baseiam no protocolo IEEE 802.11 que define como os dispositivos se comunicam através dos pacotes por meio de identificação na rede, normalmente usados em WLANs.

### PAN
    Personal Area Network: Uma rede pequena que envolve um raio de poucos metros e possui poucos dispositivos, como por exemplo: fones bluetooth conectados a celular, mouse bluetooth conectado a computador, celular conectado a computador por meio de cabo USB.

### LAN
    Local Area Network: Rede local que pode utilizar tanto conexões cabeadas como conexões sem fio. Definida por conectar dispositivos à rede em um raio de aproximadamente 100m, normalmente utilizada para uso doméstico, com roteador. Também por definição é usada corporativamente, como escritórios, departamento de uma empresa e edifícios.

### MAN
    Metropolitan Area Network: Infraestrutura de dados de alta velocidade que conecta redes LAN dentro de uma área geográfica do tamanho de uma cidade ou região metropolitana. Utiliza fibra ótica para conectar matrizes e filiais ou fornecedor interet.

### WAN
    Wide Area Network: Interconecta computadores e redes locais (LANs) geograficamente dispersas, cobrindo áreas amplas como cidades, países ou continentes. A Internet é o maior exemplo de WAN, utilizada para conectar filiais corporativas, compartilhar recursos e centralizar dados. Então, WAN é uma junção de LANs abrangendo longa distância.

### Wireless
- O que é: Transmissão de dados através de ondas de rádio. Seguem o padrão Wireless-Fidelity.
- Frequências (2.4GHz, 5GHz e 6GHz): São bandas de frequência de rádio utilizadas pelo roteador para compartilhar os dados com os outros       dispositivos da rede.
- Vantagens: Facilidade para ingressar na rede
- Desvantagens: Interferência de sinal por barreiras físicas
- Tipos de segurança (WPA2, WPA3): WPA2 (Wi-Fi Protected Access 2) é um protocolo de segurança criptografado que protege o tráfego da internet em redes sem fio. O WPA3 (Wi-Fi Protected Access 3) é o protocolo de segurança sem fio mais recente, lançado pela Wi-Fi Alliance em 2018 para substituir o WPA2. Ele oferece proteção robusta contra ataques de força bruta, criptografia mais forte (até 256 bits) e segurança aprimorada em redes públicas e domésticas.

## Protocolos Importantes
- TCP: O TCP (Transmission Control Protocol - Protocolo de Controle de Transmissão) é um padrão fundamental de rede que garante a entrega confiável, ordenada e sem erros de pacotes de dados entre aplicações.
- UDP: O User Datagram Protocol (UDP) é um protocolo de transporte rápido, simples e "sem conexão", ideal para aplicações que exigem baixa latência, como streaming de vídeo, VoIP e jogos online.
- IP: Um endereço IP (Internet Protocol) é um rótulo numérico único que identifica dispositivos (computadores, celulares, impressoras) em uma rede, permitindo a comunicação entre eles e o acesso à internet.
- DNS: O DNS (Domain Name System – Sistema de nome de domínio) converte nomes de domínio legíveis por humanos (por exemplo, www.amazon.com) em endereços IP legíveis por máquina (por exemplo, 192.0.2.44).

### Observações Pessoais ###

## O que eu entendi:
    Que existem diversos tipos de redes e que cada um desse tipo vai exigir de mim, como profissional de tecnologia e segurança, um conhecimento específico para solucionar os erros e problemas que possam vir a acometer as redes, sejam elas corporativas ou pessoais. Aprendi qu existe um estudo para transmitir dados pela luz e isso me despertou curiosidade. Agora estou aprendendo a base dos protocolos.

## Dificuldades:
    A maior dificuldade que enfreitei foi os tipos de segurança Wireless
    
## O que quero aprofundar:
    Pretendo me aprofundar em protocolos, para entender melhor como as redes funcionam.

### Parte Prática - Testes no Windows ###

## 1. Descobrindo IP da máquina
Comando utilizado:
    ipconfig

Resultado:
   Endereço IPv6 de link local . . . . . . . . : fe80::8fc8:e9b5:2730:e43e%9
   Endereço IPv4. . . . . . . .  . . . . . . . : 192.168.0.100
   Máscara de Sub-rede . . . . . . . . . . . . : 255.255.255.0
   Gateway Padrão. . . . . . . . . . . . . . . : 192.168.0.1

Explicação:
    Endereço IPv4 (Internet Protocol version 4) é o protocolo que identifica cada dispositivo dentro de uma rede. Ele faz o endereçamento dos dispositivos utilizando uma numeração em 32 bits, representado em quatro números separados por "ponto", divididos em 4 octetos (8 bits cada). Cada dispositivo na rede deve ter seu IP distinto para transmitir e receber dados.
    
    Trabalha na Camada 3 do Modelo OSI;
    Responsável por Endereçamento, Roteamento (Direcionar pacotes entre redes diferentes) e Entrega de pacotes entre redes;

    Pode ser:
        Público (acessível na internet)
        Privado (Usado em redes privadas)
            Faixas privadas:
                10.0.0.0 – 10.255.255.255
                172.16.0.0 – 172.31.255.255
                192.168.0.0 – 192.168.255.255
            
    Em resumo, como o meu ip está dentro da faixa de endereçamento privado, minha máquina não está diretamente exposta à internet, entretanto, pode se comunicar com outros dispositivos dentro da LAN.

### 2. Teste de Conectividade
Comando:
ping 8.8.8.8

O que observei:

Disparando 8.8.8.8 com 32 bytes de dados:
Resposta de 8.8.8.8: bytes=32 tempo=19ms TTL=115
Resposta de 8.8.8.8: bytes=32 tempo=17ms TTL=115
Resposta de 8.8.8.8: bytes=32 tempo=13ms TTL=115
Resposta de 8.8.8.8: bytes=32 tempo=15ms TTL=115

Estatísticas do Ping para 8.8.8.8:
    Pacotes: Enviados = 4, Recebidos = 4, Perdidos = 0 (0% de
             perda),
Aproximar um número redondo de vezes em milissegundos:
    Mínimo = 13ms, Máximo = 19ms, Média = 16ms

- Tempo de resposta: Média de 16ms
- TTL: Média de 115

Análise:
    O ICMP (Internet Control Message Protocol) é um protocolo usado para enviar mensagens de controle e diagnóstico de rede, ele não serve para transportar dados utilizáveis e sim para informar se o destino está acessível, se o pacote chegou ao destino e quanto tempo demorou para resposta chegar.
        O ICMP funciona na Camada 3 do OSI junto com o IPv4 (Ele depende do IP para funcionar).
        Tipos de Mensagens ICMP:
            Echo Request (ping)
            Echo Reply
            Destination Unreachable
            Time Exceeded (usado no tracert)

    O ping funciona e manda resposta porque:
        Cabo de Rede está conectado;
        Tenho um endereço MAC;
        Conexão com o roteador que me fornece um endereço IPv4;
        Portas configuradas;
        Rota à internet;