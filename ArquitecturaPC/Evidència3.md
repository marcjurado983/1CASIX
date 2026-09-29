
## Evidència 3

Emplena el següent en un Google Docs per als dos casos. Cal justificar el perquè de cada requeriment (per exemple: necessita tenir tants GB de Ram perquè ...). Cerca un ordinador que compleixi aquestes característiques mínimes i intenta ajustar el preu a que sigui el més barat possible.

1.Investiga quines necessitats tindria en quant a components un ordinador portàtil per a fer auditories de seguretat.

Per fer auditories de seguretat necessitaria un portàtil amb unes característiques bastant bones, ja que ha de poder executar diferents programes alhora, com Kali Linux, Wireshark, Nmap o Burp Suite.

### Característiques mínimes

| Component       | Necessitat         | Per què?                                                                           |
| --------------- | ------------------ | ---------------------------------------------------------------------------------- |
| **Processador** | 6 nuclis / 12 fils | Per poder executar diversos programes al mateix temps sense que vagi lent.         |
| **RAM**         | 16 GB              | Per utilitzar diverses eines i màquines virtuals sense quedar-nos sense memòria.   |
| **SSD**         | 512 GB             | Per instal·lar els programes i guardar captures i màquines virtuals.               |
| **GPU**         | Integrada          | No necessito una gràfica potent per fer auditories, així que puc estalviar diners. |
| **Pantalla**    | Full HD            | Per treballar millor amb terminals i diferents eines.                              |
| **Xarxa**       | Wi-Fi + Ethernet   | Per poder connectar-me a diferents xarxes durant les proves.                       |

### Ordinador escollit

He buscat un portàtil que compleixi aquestes característiques i que sigui el més barat possible. Una opció és un portàtil amb **Ryzen 5, 16 GB de RAM i 512 GB SSD**, que costa aproximadament **416 €**.

Crec que és suficient per fer auditories de seguretat sense haver de gastar diners en una targeta gràfica dedicada.

---

# 2. Servidor per a 1.000 usuaris

Per tenir un servidor web que pugui suportar uns **1.000 usuaris connectats al mateix temps**, necessitaria un ordinador més potent i preparat per estar funcionant les 24 hores.

### Característiques mínimes

| Component       | Necessitat         | Per què?                                                                                    |
| --------------- | ------------------ | ------------------------------------------------------------------------------------------- |
| **Processador** | 8 nuclis / 16 fils | Per poder gestionar moltes peticions al mateix temps.                                       |
| **RAM**         | 32 GB o més        | Perquè el servidor pugui mantenir molts processos funcionant sense quedar-se sense memòria. |
| **SSD**         | 2 × 512 GB NVMe    | Per tenir molta velocitat i poder fer una configuració RAID per tenir més seguretat.        |
| **GPU**         | No necessària      | Un servidor web no necessita una targeta gràfica potent.                                    |
| **Xarxa**       | 1 Gbit/s           | Per poder gestionar una gran quantitat de connexions.                                       |
| **Sistema**     | Ubuntu Server      | És gratuït i està pensat per utilitzar-se en servidors.                                     |

### Servidor escollit

He trobat el **Hetzner AX42**, que té:

* AMD Ryzen 7 PRO 8700GE
* 8 nuclis i 16 fils
* 64 GB de RAM ECC
* 2 × 512 GB NVMe
* Connexió d'1 Gbit/s

El preu és d'uns **97,30 € al mes + IVA**.

He escollit aquest servidor perquè compleix de sobres els requisits i està preparat per funcionar **24/7**.
