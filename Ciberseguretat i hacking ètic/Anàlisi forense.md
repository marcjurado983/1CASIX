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

Evidència 1: Simulació, adquisició i anàlisi




### PAS 1: Crea, modifica i elimina fitxers

\
Crea la carpeta i els fitxers

<figure><img src="../.gitbook/assets/Captura de pantalla 2026-10-21 111040.png" alt=""><figcaption></figcaption></figure>



Desa una imatge JPEG de prova (descarrega’n una o copia’n una) com a \~/cas\_forense/imatge.jpg

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

Registra els hashes abans d’eliminar res:

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

Eliminar secret\_atac.txt

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

Modificar document.txt

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

Cambiar permisos

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

Eliminar la imagen&#x20;

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

Comprobar

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

## Pas 2: manipulació temporal



Crea el fitxer i desa les metadades d’abans

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

Canvia les dates&#x20;

<figure><img src="../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

Desa les metadades de després

<figure><img src="../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>



## Pas 3: Desa els registres disponibles

\
Data i hora de la recollida&#x20;

<figure><img src="../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

timedatectl

<figure><img src="../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

Registres amb journalctl

<figure><img src="../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

Historial d’ordres&#x20;

<figure><img src="../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

Comprova que s’ha desat tot

<figure><img src="../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

Abans d’apagar Kali

<figure><img src="../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

<br>

## Pas 4: adquireix el disc principal amb dd

\
Apaga Kali i inicia la màquina virtual amb una ISO de Kali en mode Live.

<figure><img src="../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>



Obre un terminal i identifica els discos&#x20;

<figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

muntar només AUDITORIA

<figure><img src="../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

Executa el dd

<figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

Comprova el resultat&#x20;

<figure><img src="../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

\
Pas 5: hash i anàlisi de la imatge
----------------------------------

Calcula el hash SHA-256 de kali.dd

<figure><img src="../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

No modifica el contingut, així que el hash no canvia.

<br>

Torna a iniciar Kali des del disc principal

<figure><img src="../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

Identifica i munta AUDITORIA

![](<../.gitbook/assets/image (25).png>)



Comprova si ja tens el hash

<figure><img src="../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

Calcula el hash

<figure><img src="../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

Protegeix la imatge contra escriptura

<figure><img src="../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

Buscar document.txt

<figure><img src="../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

Recuperar el contingut de document.txt

<figure><img src="../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

Metadades de prova\_temps.txt

<figure><img src="../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

Buscar entrades eliminades

<figure><img src="../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

cercar INCIDENT\_AULA\_2026

<figure><img src="../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

Recuperar la JPEG amb PhotoRec

<figure><img src="../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>

calculat correctament el SHA-256 de la JPEG recuperada&#x20;

i comparacio amb inicial

<figure><img src="../.gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>

A la teva captura, el hash original de imatge.jpg és: d82354edc07776dcf3b76da3db275bd00897b6dd071ce13f8fb24e2d2aae655129

El hash de la JPEG recuperada és: bb4478bec97ee18e405e6a8b75f8491323221f1f891c9c53fa9cbc379e83503

Comparació del hash de la imatge recuperada

Després de recuperar una imatge JPEG amb PhotoRec, he calculat el seu hash SHA-256 amb l'ordre `sha256sum` i l'he comparat amb el hash original registrat abans d'eliminar el fitxer.

Els dos hashes són diferents. Per tant, no es pot confirmar que el fitxer recuperat sigui idèntic a la imatge original. Aquesta comparació permet comprovar la integritat del fitxer recuperat.



STRINGS I GREPS

<figure><img src="../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>
