## Filen: lagerkartan.pcap
## Trafikbaslinje

## Trafikbaslinje – TCP

| Källa (IP) | Mål (IP) | Källport | Målport |
| ---------- | -------- | -------- | ------- |
|172.20.1.30|172.20.1.58|37520     |9000     |
|172.20.1.30|172.20.1.58|42800     |80       |
|172.20.1.30|172.20.1.58|47830     |9000     |
|172.20.1.30|172.20.1.58|50536     |9000     |
|172.20.1.30|172.20.1.58|51076     |9000     |
|172.20.1.30|172.20.1.58|53077     |80       | 
|172.20.1.30|172.20.1.58|54306     |8080     |
|172.20.1.30|172.20.1.58|31064     |53       |

port 53  DNS, uppslagning av domännamn
port 8080 alternativ HTTP-port, till exempel för en utvecklingsserver eller proxy.
9000 är målporten, men vi vet inte vad tjänsten gör bara utifrån portnumret.
## Trafikbaslinje – UDP

| Källa (IP) | Mål (IP)  | Källport | Målport |
| ---------- | --------- | -------- | ------- |
|172.20.1.30 |185.12.64.1|35303    |   53    |
|172.20.1.30 |185.12.64.1|39310    |   53    |
|172.20.1.30 |185.12.64.1|45432    |   53    |
|172.20.1.30 |185.12.64.1|47701    |   53    |
|172.20.1.30 |185.12.64.1|51889    |   53    |
|172.20.1.30 |185.12.64.1|53913    |   53    |
|172.20.1.30 |185.12.64.1|58034    |   53    |
|172.20.1.30 |185.12.64.1|59740    |   53    |
port 53  DNS, uppslagning av domännamn


## Filen: avvikelsen.pcap
## Trafikbaslinje – TCP

| Källa (IP) | Mål (IP) | Källport | Målport |
| ---------- | -------- | -------- | ------- |
|172.20.1.30 |172.20.1.58|37520    |9000     |

9000 är målporten, men vi vet inte vad tjänsten gör bara utifrån portnumret.


