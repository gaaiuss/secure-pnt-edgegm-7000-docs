### VIAVI SecurePNT EdgeGM 7000

É um relógio mestre voltado para redes que precisam distribuir tempo extremamente
preciso e confiável. Ele recebe uma referência de tempo e distribui para outros
equipamentos na rede usando os protocolos PTP e NTP.

---

#### Conceito PNT — Position, Navigation and Timing

Para o caso do EdgeGM 7000, o componente mais importante é o tempo. O GNSS
normalmente fornece uma referência de tempo boa porém, não confiável o tempo
todo.

Pode sofrer:

- Jamming: interferência intencional externa.
- Spoofing: envio de sinais falsos de atacantes fingindo ser uma referêcia GNSS
  legítima.
- Meaconing: um sinal legítimo é capturado, atrasado e retransmitido.

A VIAVI utiliza a tecnologia TrustedPNT que combina, autentica e qualifica
multiplas fontes de timing.

Ou seja, na hierarquia, o EdgeGM atua como esse maestro na orquestração das
diversas referências de tempo (GNSS / GEO / LEO).

---

#### NTP vs PTP

#### Network Time Protocol:

Quando temos um servidor NTP que será usado para sincronizar dispositivos na rede
em geral e não há necessidade de precisão extrema.

Normalmente utilizado para sincronizar:

- servidores
- PCs
- aplicações
- equipamentos de rede
- sistemas operacionais

---

#### Precision Time Protocol:

É utilizado quando precisamos de uma sincronização muito mais precisa e aí entra
o orquestrador EdgeGM no topo da hierarquia e age como filtro entre os demais
equipamentos na rede.

---
