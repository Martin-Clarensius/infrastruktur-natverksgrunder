# Avvikande trafik i capture.pcap

> Automatiska heuristiker. Träffar är **indikationer som ska verifieras**, inte bevis.

## Sammanfattning

| Kontroll | Antal träffar |
|---|---|
| Misstänkt portskanning | 0 |
| Ovanliga portar | 25 |
| Okrypterade eller riskfyllda tjänster | 1 |
| Protokoll på oväntad port | 16 |
| Många TCP RST | 0 |
| Misstänkt DNS-trafik | 0 |
| Största dataflöden | 10 |

## Misstänkt portskanning

Källor som skickar SYN (utan ACK) mot minst 20 olika portar.

_Inga avvikelser hittades._

## Ovanliga portar

Portar som inte finns i listan över vanliga tjänster.

| Transport   |   Port | Protokoll   |   Antal paket |
|:------------|-------:|:------------|--------------:|
| TCP         |   4444 | TCP         |             5 |
| TCP         |  43827 | TCP         |             3 |
| TCP         |  58773 | TCP         |             3 |
| TCP         |  59521 | TCP         |             3 |
| TCP         |  57786 | TCP         |             3 |
| TCP         |  57416 | TCP         |             3 |
| TCP         |  53865 | TCP         |             3 |
| TCP         |  53604 | TCP         |             3 |
| TCP         |  53076 | TCP         |             3 |
| TCP         |  52928 | TCP         |             3 |
| TCP         |  52911 | TCP         |             3 |
| TCP         |  51202 | TCP         |             3 |
| TCP         |  59419 | TCP         |             3 |
| TCP         |  48931 | TCP         |             3 |
| TCP         |  50777 | TCP         |             3 |
| TCP         |  30295 | TCP         |             3 |
| TCP         |  42703 | TCP         |             3 |
| TCP         |  32077 | TCP         |             3 |
| TCP         |  42134 | TCP         |             3 |
| TCP         |  42001 | TCP         |             3 |
| TCP         |  37639 | TCP         |             3 |
| UDP         |  45919 | DNS         |             1 |
| UDP         |  31805 | DNS         |             1 |
| UDP         |  58910 | DNS         |             1 |
| UDP         |  30609 | DNS         |             1 |

## Okrypterade eller riskfyllda tjänster

Protokoll som ofta skickar data i klartext eller är vanliga attackmål.

|   Port | Tjänst   | Källa        | Destination    |   Antal paket |
|-------:|:---------|:-------------|:---------------|--------------:|
|     80 | HTTP     | 172.20.1.133 | 46.224.108.117 |            96 |

## Protokoll på oväntad port

Kan vara tunnling eller en tjänst som försöker gömma sig.

| Protokoll   |   Port |   Antal paket |
|:------------|-------:|--------------:|
| DNS         |  30609 |             1 |
| DNS         |  30667 |             1 |
| DNS         |  31805 |             1 |
| DNS         |  33255 |             1 |
| DNS         |  33636 |             1 |
| DNS         |  35330 |             1 |
| DNS         |  35738 |             1 |
| DNS         |  38443 |             1 |
| DNS         |  45919 |             1 |
| DNS         |  47329 |             1 |
| DNS         |  51922 |             1 |
| DNS         |  52894 |             1 |
| DNS         |  55052 |             1 |
| DNS         |  57047 |             1 |
| DNS         |  58910 |             1 |
| DNS         |  59689 |             1 |

## Många TCP RST

Återställda anslutningar kan tyda på stängda portar, skanning eller blockering.

_Inga avvikelser hittades._

## Misstänkt DNS-trafik

Domäner med namn på 50+ tecken eller många unika subdomäner (möjlig DNS-tunnling).

_Inga avvikelser hittades._

## Största dataflöden

Toppkonversationer sett till datamängd.

| Källa          | Destination    |   KiB |
|:---------------|:---------------|------:|
| 172.20.1.133   | 46.224.108.117 |   6.3 |
| 46.224.108.117 | 172.20.1.133   |   5.5 |
| 172.20.1.2     | 172.20.1.133   |   2.6 |
| 172.20.1.133   | 172.20.1.2     |   2.3 |
| 185.12.64.1    | 172.20.1.133   |   1.8 |
| 172.20.1.133   | 185.12.64.1    |   1.2 |
| 172.20.1.133   | 185.12.64.2    |   0.4 |
| 185.12.64.2    | 172.20.1.133   |   0.4 |
| 172.20.1.133   | 203.0.113.235  |   0.3 |
| 203.0.113.235  | 172.20.1.133   |   0.2 |

