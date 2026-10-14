# Adressplan 
**Adressutrymme:** 10.40.0.0/16 (RFC 1918)
**Omfattning:** Endast IPv4. IPv6 är avstängt på labbservrarna och ingår inte.
**Plattform:** Oracle Cloud (OCI). Nätadress, gateway (.1 i subnätet) och broadcast reserveras per subnät.
**Antagande:** Serverzoner dimensionerade för 10–25 servrar inkl. tillväxt.
**Version / datum / ansvarig:** v02 / 2026-10-14 / <namn>

| Prefix | Syfte | Adressintervall (första–sista) | Ansvarig tjänst | Reserverat utrymme | Kommentar |
|---|---|---|---|---|---|
| 10.40.0.0/27 | Webb / DMZ | 10.40.0.2 – 10.40.0.30 | Webbserver | 10.40.0.25 – 10.40.0.30 | Exempel, .1 gateway |
| 10.40.0.32/27 | Applikation | 10.40.0.34 – 10.40.0.62 | Appserver | 10.40.0.57 – 10.40.0.62 | Exempel, .33 gateway |
| 10.40.0.64/28 | Databas | 10.40.0.66 – 10.40.0.78 | Databasserver | 10.40.0.75 – 10.40.0.78 | Exempel, .65 gateway |
| 10.40.0.80/28 | Logg / övervakning | 10.40.0.82 – 10.40.0.94 | Loggserver | 10.40.0.91 – 10.40.0.94 | Exempel, .81 gateway |
| 10.40.0.96/28 | Management / admin | 10.40.0.98 – 10.40.0.110 | Jump/SSH | 10.40.0.107 – 10.40.0.110 | Exempel, .97 gateway |
| 10.40.0.112 – 10.40.255.255 | Ej allokerat (tillväxt, klientnät) | 10.40.0.112 – 10.40.255.254 | – | Hela blocket | Får ej användas utan uppdatering av planen |