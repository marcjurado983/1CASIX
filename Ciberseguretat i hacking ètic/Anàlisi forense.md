---
nom: Marc Jurado
---

# Anàlisi forense

***

## Preparació: afegeix un disc d’auditoria

Amb la màquina virtual apagada, afegeix un segon disc virtual des de VirtualBox o VMware a la màquina Kali Linux.

Assigna-li prou capacitat per contenir una imatge completa del disc principal i els resultats de l’anàlisi. Per simplificar, conserva una única imatge i analitza-la sense modificar-la.

Afegeix els passos detallats de configuració

<figure><img src="../.gitbook/assets/Captura de pantalla 2026-10-21 110050.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Captura de pantalla 2026-10-21 110352.png" alt=""><figcaption></figcaption></figure>

***

Inicia Kali, identifica el disc nou amb lsblk, crea-hi una partició i formata-la. Comprova que és el disc nou abans de formatar-lo. Assigna-li l’etiqueta AUDITORIA i crea-hi aquestes carpetes: imatge/,registres/,resultats/

<figure><img src="../.gitbook/assets/Captura de pantalla 2026-10-21 110540.png" alt=""><figcaption></figcaption></figure>

***

FORMATAR EL DISC

<figure><img src="../.gitbook/assets/Captura de pantalla 2026-10-21 110626.png" alt=""><figcaption></figcaption></figure>



Crear punt de muntatge,Muntar

<figure><img src="../.gitbook/assets/Captura de pantalla 2026-10-21 110723.png" alt=""><figcaption></figcaption></figure>





Crear carpetes

<figure><img src="../.gitbook/assets/Captura de pantalla 2026-10-21 110726.png" alt=""><figcaption></figcaption></figure>

***
