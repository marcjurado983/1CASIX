---
description: Marc Jurado Valero
---

# Monitoratge i anàlisi del comportament d'un sistema

### PART 1. Establir el comportament habitual de Windows

1\. Arrencar el sistema

1. Inicia la màquina virtual de Windows 10.
2. Inicia sessió normalment.
3. No obris cap programa.
4. Espera entre 3 i 5 minuts perquè el sistema es carregui completament.

2\. Obrir el Gestor de tasques

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

3\. Analitzar la CPU

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

4.Analitzar la Memòria

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

5\. Analitzar el Disc

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

6\. Analitzar la Xarxa

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

7\. Identificar processos consumidors

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

8\. Ordenar per memòria

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

9\. Localitzar PID

![](<../.gitbook/assets/image (8).png>)<br>

Conclusió: El Monitor de recursos dona més detalls que el Gestor de tasques, que és un resum més simple&#x20;





### **PART 2. Monitor de Recursos**



1\. Obrir-lo

<figure><img src="../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

\
2\. Analitzar CPU

<figure><img src="../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

3\. Analitzar Memòria

<figure><img src="../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

4\. Analitzar Disc

<figure><img src="../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

5\. Analitzar Xarxa

<figure><img src="../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

6\. Registrar la línia base

<figure><img src="../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>



### **PART 3. Generar activitat**

1\. Obrir aplicacions

Obrir: bloc de notes, calculadora i Paint

<figure><img src="../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>



2\. Obrir navegador

Obre Edge.

Obre 5-10 pestanyes.

<figure><img src="../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>



3\. Analitzar recursos

CPU

Observa CPU i quin consumeix més: el que consumeix més és SHellExperienceHost.exe

<figure><img src="../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

#### Memòria

<figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

Consumeix més MsMpEng.exe

MsMpEng.exe és el procés principal de Microsoft Defender Antivirus

Analitzar fitxers en temps real.



4\. Prova de disc

Copia un fitxer gran (500 MB o més) i observes el disc

<figure><img src="../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

5\. Compressió

Instal·la o usa: 7-Zip

Observa: CPU, Memòria i Disc

<figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>



6\. Tornar a repòs

Tanca totes les aplicacions.

Espera 2-3 minuts.

<figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

* CPU: “Els que gasten més CPU són msedge.exe i SearchApp.exe.” (Treu la frase de ShellExperienceHost.)
* Memòria: “La memòria puja fins al 72-79%. L’antivirus (MsMpEng.exe) és el que en gasta més.”
* Disc: “Quan copio el fitxer, el disc treballa més.”
* Compressió: “Amb 7-Zip pugen la CPU, la memòria i el disc.”
* Tornar a repòs: “Quan tanco les aplicacions, tot torna a valors semblants als del principi.”





### **PART 4. Windows Event Viewer**

\
1\. Obrir-lo

<figure><img src="../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

2\. Accedir als registres

<figure><img src="../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>



### PART 5. Registre Application

1\. Entrar a Application

<figure><img src="../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

2\. Analitzar un esdeveniment

<figure><img src="../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

3\. Buscar nivells

Localitza:Informació,Advertiment,Error

<figure><img src="../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

PART 6. Registre System



busca esdeveniments relacionats amb:



Controlador de disc

<figure><img src="../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

Xarxa i DNS no he trobat



Serveis

<figure><img src="../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>

### **PART 7. Registre Security**

<figure><img src="../.gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>

### **PART 8. Filtrar registres**

<figure><img src="../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>

Filtrar per temps

<figure><img src="../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>

Eliminar filtre

<figure><img src="../.gitbook/assets/image (41).png" alt=""><figcaption></figcaption></figure>

### **PART 9. Generar un esdeveniment**

\
1\. Anotar hora

<figure><img src="../.gitbook/assets/image (42).png" alt=""><figcaption></figcaption></figure>

2\. Aturar un servei

<figure><img src="../.gitbook/assets/image (43).png" alt=""><figcaption></figcaption></figure>

3\. Tornar-lo a iniciar

<figure><img src="../.gitbook/assets/image (44).png" alt=""><figcaption></figcaption></figure>

4\. Buscar-lo al visor

Ves a System.

Ordena per data.

<figure><img src="../.gitbook/assets/image (46).png" alt=""><figcaption></figcaption></figure>



### **PART 10. Kali Linux - journalctl**

1\. Iniciar Kali

<figure><img src="../.gitbook/assets/image (47).png" alt=""><figcaption></figcaption></figure>

2\. Mostrar el journal

<figure><img src="../.gitbook/assets/image (48).png" alt=""><figcaption></figcaption></figure>

3\. Mostrar últimes entrades

<figure><img src="../.gitbook/assets/image (49).png" alt=""><figcaption></figcaption></figure>

4\. Últims 10 minuts

<figure><img src="../.gitbook/assets/image (50).png" alt=""><figcaption></figcaption></figure>

5\. Mostrar errors

<figure><img src="../.gitbook/assets/image (51).png" alt=""><figcaption></figcaption></figure>

6\. Veure serveis actius

<figure><img src="../.gitbook/assets/image (52).png" alt=""><figcaption></figcaption></figure>

7\. Consultar un servei

<figure><img src="../.gitbook/assets/image (53).png" alt=""><figcaption></figcaption></figure>

8\. Temps real

<figure><img src="../.gitbook/assets/image (54).png" alt=""><figcaption></figcaption></figure>

9\. Generar activitat

<figure><img src="../.gitbook/assets/image (55).png" alt=""><figcaption></figcaption></figure>

Torna a la finestra del journalctl -f.

<figure><img src="../.gitbook/assets/image (56).png" alt=""><figcaption></figcaption></figure>



### PART 11. Investigar /var/log

1\. Entrar al directori

![](<../.gitbook/assets/image (58).png>)<br>

2\. Veure fitxers

<figure><img src="../.gitbook/assets/image (59).png" alt=""><figcaption></figcaption></figure>

3\. Veure modificacions recents

<figure><img src="../.gitbook/assets/image (60).png" alt=""><figcaption></figcaption></figure>

4\. Consultar un registre

<figure><img src="../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure>

5\. Veure les últimes línies

<figure><img src="../.gitbook/assets/image (62).png" alt=""><figcaption></figcaption></figure>

6\. Seguiment en temps real

<figure><img src="../.gitbook/assets/image (63).png" alt=""><figcaption></figcaption></figure>

7\. Filtrar informació

<figure><img src="../.gitbook/assets/image (64).png" alt=""><figcaption></figcaption></figure>

### **PART 12. Correlació d'esdeveniments a Linux**



1\. Anotar hora

<figure><img src="../.gitbook/assets/image (65).png" alt=""><figcaption></figcaption></figure>

2\. Reiniciar servei

<figure><img src="../.gitbook/assets/image (66).png" alt=""><figcaption></figcaption></figure>

3\. Comprovar registres

<figure><img src="../.gitbook/assets/image (67).png" alt=""><figcaption></figcaption></figure>

4\. Buscar a /var/log

<figure><img src="../.gitbook/assets/image (68).png" alt=""><figcaption></figcaption></figure>
