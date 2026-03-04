Ping

# C:\Users\Luis>ping 1.1.1.1

Disparando 1.1.1.1 com 32 bytes de dados:
Resposta de 1.1.1.1: bytes=32 tempo=14ms TTL=56
Resposta de 1.1.1.1: bytes=32 tempo=14ms TTL=56
Resposta de 1.1.1.1: bytes=32 tempo=15ms TTL=56
Resposta de 1.1.1.1: bytes=32 tempo=14ms TTL=56

Estatísticas do Ping para 1.1.1.1:
    Pacotes: Enviados = 4, Recebidos = 4, Perdidos = 0 (0% de
             perda),
Aproximar um número redondo de vezes em milissegundos:
    Mínimo = 14ms, Máximo = 15ms, Média = 14ms

# C:\Users\Luis>ping www.google.com -t

Disparando www.google.com [172.217.172.4] com 32 bytes de dados:
Resposta de 172.217.172.4: bytes=32 tempo=13ms TTL=115
Resposta de 172.217.172.4: bytes=32 tempo=15ms TTL=115
Resposta de 172.217.172.4: bytes=32 tempo=15ms TTL=115
Resposta de 172.217.172.4: bytes=32 tempo=13ms TTL=115
Resposta de 172.217.172.4: bytes=32 tempo=14ms TTL=115
Resposta de 172.217.172.4: bytes=32 tempo=19ms TTL=115
Resposta de 172.217.172.4: bytes=32 tempo=14ms TTL=115
Resposta de 172.217.172.4: bytes=32 tempo=13ms TTL=115
Resposta de 172.217.172.4: bytes=32 tempo=16ms TTL=115
Resposta de 172.217.172.4: bytes=32 tempo=14ms TTL=115
Resposta de 172.217.172.4: bytes=32 tempo=13ms TTL=115
Resposta de 172.217.172.4: bytes=32 tempo=13ms TTL=115
Resposta de 172.217.172.4: bytes=32 tempo=15ms TTL=115
Resposta de 172.217.172.4: bytes=32 tempo=14ms TTL=115
Resposta de 172.217.172.4: bytes=32 tempo=14ms TTL=115
Resposta de 172.217.172.4: bytes=32 tempo=14ms TTL=115

Estatísticas do Ping para 172.217.172.4:
    Pacotes: Enviados = 16, Recebidos = 16, Perdidos = 0 (0% de
             perda),
Aproximar um número redondo de vezes em milissegundos:
    Mínimo = 13ms, Máximo = 19ms, Média = 14ms

# C:\Users\Luis>ping 8.8.8.8 -t

Disparando 8.8.8.8 com 32 bytes de dados:
Resposta de 8.8.8.8: bytes=32 tempo=15ms TTL=115
Resposta de 8.8.8.8: bytes=32 tempo=14ms TTL=115
Resposta de 8.8.8.8: bytes=32 tempo=14ms TTL=115
Resposta de 8.8.8.8: bytes=32 tempo=15ms TTL=115
Resposta de 8.8.8.8: bytes=32 tempo=14ms TTL=115
Resposta de 8.8.8.8: bytes=32 tempo=15ms TTL=115
Resposta de 8.8.8.8: bytes=32 tempo=14ms TTL=115
Resposta de 8.8.8.8: bytes=32 tempo=13ms TTL=115
Resposta de 8.8.8.8: bytes=32 tempo=15ms TTL=115
Resposta de 8.8.8.8: bytes=32 tempo=13ms TTL=115
Resposta de 8.8.8.8: bytes=32 tempo=13ms TTL=115
Resposta de 8.8.8.8: bytes=32 tempo=15ms TTL=115
Resposta de 8.8.8.8: bytes=32 tempo=14ms TTL=115
Resposta de 8.8.8.8: bytes=32 tempo=17ms TTL=115

Estatísticas do Ping para 8.8.8.8:
    Pacotes: Enviados = 14, Recebidos = 14, Perdidos = 0 (0% de
             perda),
Aproximar um número redondo de vezes em milissegundos:
    Mínimo = 13ms, Máximo = 17ms, Média = 14ms

# C:\Users\Luis>tracert 1.1.1.1

Rastreando a rota para one.one.one.one [1.1.1.1]
com no máximo 30 saltos:

  1    <1 ms    <1 ms    <1 ms  192.168.0.1
  2     1 ms    <1 ms    <1 ms  192.168.2.1
  3     5 ms     1 ms     1 ms  10.100.255.1
  4     4 ms     2 ms     1 ms  10.10.100.1
  5    11 ms     9 ms     8 ms  10.200.203.33
  6    15 ms    14 ms    13 ms  ae1-3041.edge-gig-cr1.fortetelecom.com.br [186.237.48.244]
  7    17 ms    17 ms    15 ms  170-84-53-6.fortetelecom.com.br [170.84.53.6]
  8    14 ms    15 ms    14 ms  172.69.3.19
  9    16 ms    14 ms    14 ms  one.one.one.one [1.1.1.1]

Rastreamento concluído.

# C:\Users\Luis>tracert 8.8.8.8

Rastreando a rota para dns.google [8.8.8.8]
com no máximo 30 saltos:

  1    <1 ms    <1 ms    <1 ms  192.168.0.1
  2     1 ms    <1 ms    <1 ms  192.168.2.1
  3     4 ms     1 ms     1 ms  10.100.255.1
  4     3 ms     1 ms     1 ms  10.10.100.1
  5    11 ms     9 ms     8 ms  10.200.203.33
  6    14 ms    13 ms    12 ms  ae1-3041.edge-gig-cr1.fortetelecom.com.br [186.237.48.244]
  7    16 ms    15 ms    14 ms  74.125.50.192
  8    16 ms    17 ms    14 ms  142.250.228.65
  9    14 ms    14 ms    17 ms  142.251.48.155
 10    14 ms    14 ms    14 ms  dns.google [8.8.8.8]

Rastreamento concluído.

# C:\Users\Luis>tracert www.instagram.com

Rastreando a rota para z-p42-instagram.c10r.instagram.com [31.13.91.174]
com no máximo 30 saltos:

  1    <1 ms    <1 ms    <1 ms  192.168.0.1
  2     1 ms    <1 ms     1 ms  192.168.2.1
  3     4 ms     1 ms     1 ms  10.100.255.1
  4     4 ms     1 ms     2 ms  10.10.100.1
  5    11 ms    10 ms    11 ms  10.200.203.33
  6    22 ms    14 ms    13 ms  ae1-3041.edge-gig-cr1.fortetelecom.com.br [186.237.48.244]
  7    14 ms    15 ms    16 ms  186-237-53-86.fortetelecom.com.br [186.237.53.86]
  8    15 ms    15 ms    13 ms  po4004.asw04.gig4.tfbnw.net [129.134.51.250]
  9    16 ms    16 ms    16 ms  psw04.gig4.tfbnw.net [129.134.119.204]
 10    19 ms    19 ms    18 ms  msw1ag.02.gig4.tfbnw.net [129.134.119.97]
 11    16 ms    16 ms    16 ms  instagram-p42-shv-02-gig4.fbcdn.net [31.13.91.174]

Rastreamento concluído.