# Evidència 1: Connectant màquines virtuals
Marc Jurado

He configurat les màquines virtuals de **Windows i Kali** perquè comparteixin una xarxa i es puguin comunicar entre elles. He provat dues configuracions diferents d'adaptador: **adaptador pont**, que permet que les màquines estiguin connectades a la mateixa xarxa física i tinguin Internet, i **xarxa interna**, que crea una xarxa privada només entre les màquines virtuals. Per aïllar la xarxa, utilitzaria la **xarxa interna**, ja que Windows i Kali es poden comunicar entre elles però queden separades de la xarxa externa i d'Internet.

Configuració 1: les dues màquines en NAT comunicació més internet
Totes dues màquines tenen IP del rang NAT (normalment 10.0.2.x) 

<img src="img/cap1.png" alt="Sistemes Operatius" width="500">
---
<img src="img/cap2.png" alt="Sistemes Operatius" width="500">

Configuració 2: Xarxa interna les dues no tenen conexio a internet pero es comuniquen aïllant la xarxa

<img src="img/cap3.png" alt="Sistemes Operatius" width="500">

<img src="img/cap4.png" alt="Sistemes Operatius" width="500">


---

Identificar IP, màscara, gateway, DNS i MAC de la màquina Windows i de la màquina Kali.

## Màquina Windows
<img src="img/cap5.png" alt="Sistemes Operatius" width="500">

<img src="img/cap6.png" alt="Sistemes Operatius" width="500">

## Màquina Kali

<img src="img/cap7.png" alt="Sistemes Operatius" width="500">

<img src="img/cap8.png" alt="Sistemes Operatius" width="500">

---

Comprovar la comunicació Windows → Kali amb la comanda ping per als dos tipus 

<img src="img/cap9.png" alt="Sistemes Operatius" width="500">

---

Comprovar la comunicació Kali → Windows amb la comanda ping per als dos tipus d'adaptador.

<img src="img/cap10.png" alt="Sistemes Operatius" width="500">

---

Investigar qualsevol ping que no funcioni i determinar si el problema és de xarxa o de tallafoc (Windows per defecte bloqueja els pings des del tallafocs).

<img src="img/cap11.png" alt="Sistemes Operatius" width="500">

He detectat que el problema és de Xarxa, ja que la connexio ping al 8.8.8.8, de google no funciona al desactivar internet


---
