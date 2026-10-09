# Activitat: Usuaris, perfils i seguretat del sistema

## Apartat 1. Usuaris existents

### WINDOWS 10

1. **Identificar l'usuari actual:** comprovar amb quin usuari he iniciat sessió a Windows.
   
   <img src="../../.gitbook/assets/cap50.png" alt="Sistemes Operatius" width="500">

2. **Llistar els usuaris locals:** obtenir una llista de tots els comptes d'usuari que hi ha a l'ordinador.
   
   <img src="../../.gitbook/assets/cap51.png" alt="Sistemes Operatius" width="500">
  
3. **Consultar els usuaris gràficament:** trobar els mateixos comptes mitjançant les eines d'administració de Windows.
   
   <img src="../../.gitbook/assets/cap52.png" alt="Sistemes Operatius" width="500">
   
4. **Diferenciar els comptes:** identificar quins usuaris he creat jo i quins han estat creats automàticament pel sistema.
   
     <img src="../../.gitbook/assets/cap53.png" alt="Sistemes Operatius" width="500">
     
5. **Comprovar els comptes desactivats:** revisar si hi ha usuaris que no poden iniciar sessió perquè estan desactivats.
    
   <img src="../../.gitbook/assets/cap54.png" alt="Sistemes Operatius" width="500">
   
6. **Consultar el SID:** trobar l'identificador únic (SID) del meu usuari.
    
   <img src="../../.gitbook/assets/cap55.png" alt="Sistemes Operatius" width="500">
  
7. **Identificar els comptes predeterminats:** indicar quins comptes venen creats per defecte amb Windows.
    
   <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">


### KALI LINUX

1. **Identifica l'usuari amb què has iniciat sessió.**
   
  <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

2. **Consulta el seu UID.**

   <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

3. **Identifica els grups als quals pertany.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

4. **Consulta la llista d'usuaris existents al sistema.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

5. **Localitza el compte root.**

      <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

6. **Identifica alguns comptes que no corresponen a persones que utilitzen l'ordinador.**

      <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">


## Apartat 2. Investiga els grups predeterminats

### Windows 10

1. **Consulta tots els grups locals existents.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

2. **Localitza el grup d'administradors.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

3. **Comprova quins usuaris en formen part.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

4. **Localitza el grup d'usuaris estàndard.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

5. **Localitza el grup relacionat amb l'accés mitjançant Escriptori Remot.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

6. **Identifica els grups als quals pertany el teu usuari actual.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

7. **Comprova si el teu usuari té privilegis administratius.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">


### Kali Linux

1. **Consulta els grups existents.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

2. **Identifica els grups als quals pertany el teu usuari.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

3. **Localitza el grup que permet als usuaris obtenir temporalment privilegis administratius.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

4. **Comprova quins usuaris pertanyen a aquest grup.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

5. **Identifica almenys tres grups del sistema que no hagis creat tu.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">


---

## Apartat 3. Crea un usuari de treball

> Crearem un compte que utilitzarem com a usuari de treball sense privilegis. L’usuari client serà el teu nom + client, per exemple `isaacclient`.

### Windows 10

1. **Crea l'usuari local client.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

2. **Assigna-li una contrasenya.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

3. **Comprova que el compte està habilitat.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

4. **Verifica que no disposa de privilegis administratius.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

5. **Identifica el SID assignat al nou compte.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

6. **Comprova a quins grups pertany.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">


### Kali Linux

1. **Crea també l'usuari client.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

2. **Assigna-li una contrasenya.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

3. **Comprova que disposa d'un directori personal.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

4. **Identifica el seu UID.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

5. **Identifica el seu grup principal.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

6. **Comprova els altres grups als quals pertany.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

7. **Verifica que inicialment no disposa de privilegis administratius.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">


---

## Apartat 4. Crea un grup local

### Windows 10

1. **Crea un grup local anomenat GrupClients.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

2. **Afegeix-hi l'usuari client.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">


### Kali Linux

1. **Crea un grup anomenat ClientsLinux.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

2. **Afegeix-hi client.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

3. **Comprova que l'usuari apareix com a membre del grup.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

4. **Inicia una nova sessió amb client i verifica que la nova pertinença al grup s'ha aplicat.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">


---

## Apartat 5. Separa el compte de treball del compte d'administració

> Treballar habitualment amb privilegis administratius no és una bona pràctica. Crearem un segon compte destinat a tasques d'administració. Vull que igual que a l’altre li afegeixis el teu nom al principi, per exemple: `isaacadmin`.

### Windows 10

1. **Crea l'usuari admin.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

2. **Assigna-li una contrasenya diferent de la de client.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

3. **Concedeix-li privilegis administratius.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

4. **Comprova a quins grups pertany.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">


### Kali Linux

1. **Crea l'usuari admin.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

2. **Concedeix-li la possibilitat de realitzar tasques administratives mitjançant el mecanisme d'elevació de privilegis de Linux.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

3. **Comprova els seus grups.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">


---

## Apartat 6. Comprova el principi de mínim privilegi

> Ara comprovaràs pràcticament que els dos comptes no tenen les mateixes capacitats.

### Windows 10

1. **Inicia sessió amb client.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

2. **Intenta modificar una configuració del sistema que requereixi privilegis administratius.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

3. **Intenta obrir una eina del sistema amb privilegis d'administrador i cancela l'elevació de privilegis.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

4. **Comprova que pots continuar fent tasques normals amb client.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

5. **Repeteix l'operació utilitzant admin i compara el comportament dels dos comptes.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">


### Kali Linux

1. **Inicia sessió amb client.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

2. **Intenta realitzar una operació que requereixi privilegis de root.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

3. **Comprova que l'operació no es pot completar amb els privilegis actuals.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

4. **Inicia sessió amb admin.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

5. **Repeteix l'operació utilitzant el mecanisme d'elevació de privilegis.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

6. **Verifica que admin pot executar temporalment una operació com a root.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">


---

## Apartat 7. Investiga els perfils locals de Windows

> Treballarem ara amb la diferència entre compte d'usuari i perfil d'usuari.

1. **Inicia sessió a Windows amb client.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

2. **Localitza el directori corresponent al seu perfil.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

3. **Identifica les carpetes Escriptori, Documents, Descàrregues i Imatges.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

4. **Activa la visualització dels elements ocults.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

5. **Localitza AppData.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

6. **Tanca la sessió.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

7. **Inicia sessió com a admin.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

8. **Comprova que disposa del seu propi Escriptori, Documents i altres directoris de perfil.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

9. **Localitza el perfil de client des del compte admin.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">


---

## Apartat 8. Investiga els directoris personals de Kali Linux

1. **Inicia sessió amb client.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

2. **Identifica quin és el seu directori personal.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

3. **Mostra també els fitxers i directoris ocults.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

4. **Localitza els directoris personals dels altres usuaris.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

5. **Inicia sessió amb admin.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

6. **Identifica el seu directori personal.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

7. **Compara'l amb el de client.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">


---

## Apartat 9. Protegeix informació del perfil

### Windows 10

1. **Inicia sessió amb client.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

2. **Crea una carpeta anomenada Privat.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

3. **Crea-hi un document.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

4. **Consulta les propietats de seguretat de la carpeta.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

5. **Identifica el propietari.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

6. **Identifica quins usuaris i grups disposen de permisos.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

7. **Observa els permisos de client.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

8. **Comprova si els permisos provenen de la carpeta superior.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">


### Kali Linux

1. **Inicia sessió amb client.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

2. **Crea una carpeta anomenada privat.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

3. **Crea-hi un document.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

4. **Consulta el propietari, el grup i els permisos de la carpeta.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

5. **Configura-la perquè només el propietari pugui accedir-hi.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

6. **Inicia sessió amb un altre usuari estàndard.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

7. **Intenta accedir al contingut de la carpeta.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

8. **Torna a client i comprova que continua tenint-hi accés.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">


---

## Apartat 10. Configura la seguretat dels comptes de Windows

1. **Obre l'eina de Windows destinada a configurar les directives de seguretat local.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

2. **Localitza les directives de compte.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

3. **Accedeix a la política de contrasenyes.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

4. **Consulta la longitud mínima configurada.**

    <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

5. **Consulta l'historial de contrasenyes.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

6. **Consulta els requisits de complexitat.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

7. **Localitza la política de bloqueig de comptes.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

8. **Comprova que la configuració ha quedat aplicada.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">

9. **Revisa els comptes client i admin per assegurar-te que tots dos compleixen la nova política.**

     <img src="../../.gitbook/assets/cap56.png" alt="Sistemes Operatius" width="500">
   
