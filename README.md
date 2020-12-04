# Apunts_UF1_1

## INTRODUCCIÓ

### Tipus de Software
  - De sistema
  - D'aplicació
  - De desenvolupament

### Relació Hardware-Software
  - Disc dur: emmagatzema de forma permanent els arxius executablesi els arxius de dades
  - Memòria RAM: emmagatzema de forma temporal els codis binàris dels arxius executables i els arxius de dades necessaris.
  - CPU: llegeix i executa instruccions emmagatzemades a la memòria RAM, així com les dades necessàries.
  - E/S: recull noves dades desde l'entrada, es mostren els resultats, es llegeixen/guarden al disc...

### Codi font, objecte i executable
  - Codi font: arxius de text llegible escrit en un llenguatge de programació.
  - Codi objecte: arxiu binari no executable.
  - Codi executable: arxiu binari executable.

## CICLE DE VIDA DEL SOFTWARE

### Enginyeria de Software (desenvolupament de software)
Què és? Disciplina que estudia els principis i metodologies per al desenvolupament i manteniment de sistemes software.
Enginyeria de sistemes: Especificació del sistema

### Desenvolupament de Software
#### Fases principals
###### 1. Anàlisis
Determinació i definició de les necessitats del client i s'especifiquen els requisits que ha de complir el software a desenvolupar.  La especificació i requisits han de ser:
- Completa i sense omisions
- Concisa i sense trivialitats
- Evitar ambigüetats
- Evitar detalls de disseny
- Entendible per al client
- Separació de requisits funcionals i no funcionals
- Dividir i jerarquitzar el model
- Fixar criteris de validació

Especificació de requisits del software.

###### 2. Disseny
El sistema es descompon i s'organitza en elements components que poden ser desenvolupats per separat. També s'especifica la interrelació i funcionalitat dels elements components. Les activitats habituals en disseny són: arquitectònic (documentació d'aquitectura del software), detallat(especificació de mòduls i funcions), de dades i d'interfície.

###### 3. Codificació
S'escriu el codi font de cada component. S'utilitzen diferents llenguatges informàtics:
- Lenguajes de programació: C, C++, Java, Javascript,..
- Altres: HTML, XML, JSON...

Codi font.

###### 4. Proves
El principal objectiu de les proves és aconseguir que el programa funcioni correctament i descobrir els defectes que tingui. S'ha d'intentar sotmetre el programa al màxim de situacions diferents possibles.

- Unitats: mòduls utilitzables
- Integració: sistema utilitzable
- Sistema: sistema acceptat

###### 5. Manteniment
Durant l'explotació del sistema del software és necessari realitzar canvis ocasionals. Refer les fases prèvies si és necessari. Els tipus de manteniment són:
- Correctiu: correcció de defectes
- Perfectiu: millora de la funcionalitat
- Evolutiu: afegir funcionalitats noves
- Adaptatiu: adaptació a nous entorns

Obtenim informes d'errors i control de canvis.

### Models de desenvolupament de Software
- Models clàssics (predictius)##### Metodologies àgils
Mètodes d'enginyeria de software basats en el desenvolupament iteratiu i incremental.
Les metodologies més conegudes són:
- Kanban: control segons demanda, sistema de targetes
- Scrum: incremental, se organiza por sprints
- XP (eXtreme Programming): per parelles, el client s'intrega a l'equip de desenvolupament

## LLENGUATGES DE PROGRAMACIÓ
### Obtenció del codi executable
Per obtenir codi binàri executable existeixen dos opcions:
- Compilar
- Interpretar

### Procés de compilació/interpretació
Es du a terme dos fases:
1. Anàlisis lèxic
2. Anàlisis sintàctic
Si no existeixen errors, es genera el codi objecte corresponent.

### Procés de compilació/interpretació
Exemple: C, C++,
Avantatges: execució molt eficient
Desavantatges: s'ha de compilar després de qualsevol modificació

### Llenguatges interpretats
Exemple: PHP, Javascript
Avantatges: el codi font s'interpreta directament
Desavantatges: execució menys eficient

### Java
Llenguatge compilat i interpretat. Java es compila i s'obté un codi binari intermedi anomenat bytecode. Aquest bytecode s'interpreta per executar-lo.
Avantatges: estructurat i orientat a objectes, fàcil d'aprendre, bona documentació i base d'usuaris
Desaventatges: menys eficient que els llenguatges compilats

### Tipus
- declaratius: indiquem el resultat sense especificar els passos. Normalment son llenguatges interpretats.
    - lògics: utilitzen regles (Prolog)
    - funcionals: utilitzen funcions (Lisp, Haskell)
    - algebraicos: utilitzen sentències(SQL)
- imperatius: indiquem els passos a seguir per obtenir un resultat. Els llenguatges orientats a objectes són també llenguatges estructurats. Molts són compilats.
    - estructurats: C
    - orientets a objectes: java
    - multiparadigma: C++, Javascript
- Segons abstracció:
    - Baix nivell: ensamblador
    - Nivell mitjà: C
    - Alt nivell: C++, Java

### Evolució
1. Codi binàri
2. Ensamblador
3. Llenguatges estructurats
4. Llenguatges orientats a objectes

### Criteris per a la selecció d'un llenguatge
- Camp s'aplicació
- Experiència prèvia
- Eines de desenvolupament
- Documentació disponible
- Base d'usuaris
- Reutilització
- Portabilitat
- Imposició client
    - Model en cascada
    - Model en V
- Models de construcció de prototips
- Models evolutius o incrementals
    - Model en espiral (iteratius)
    - Metodologies àgils (adaptatius)

##### Model en cascada
Model més antic. Identifica les fases principals del desenvolupament software i les fases es realitzen en ordre:
```sh
Anàlisis > Disseny > Codificació > Proves > Manteniment
```
És un model rígid que no s'adapta bé quan hi ha canvis d'especificació. Existeixen diferents variants amb major o menos quantitat d'activitats.

##### Model en V
Model similar al de cascada en la que hi ha una jerarquía en diferents nivells. Els nivells superiors indiquen major abstracció i els inferiors més detall. El resultat d'una fase és l'entrada de la següent. Existeixen diferents variants amb major o menos quantitat d'activitats.
```sh
Preanàlisis > Anàlisis > Disseny > Desenvolupament > Implantació > Proves unitat > Proves integració > Operació > Manteniment
```
Hi ha verificació i validació entre els nivells.

#### Models de construcció de prototips
Requisits no especificats amb claritat (per falta d'experiència prèvia i per falta de concreció del client/usuari). Consisteixen en la creació d'un prototip durant la fase d'anàlisi i probat de cara a ajustar els requisits del software.

##### Tipus de prototips
- Prototips ràpids: pot utilitzar un altre llenguatge/eina i és descartat finalment.
- Prototip evolutiu: utilitza el mateix llenguatge/eina del projecte i s'utilitzar com a base per al desenvolupament de tot el projecte.

##### Model en Espiral
El model en espiral es retroalimenta ja que el projecte passa varies vegades per cada fase de l'espiral.

Les fases de cada cicle:
1. Comunicació amb el client: procés d'investigació per plantejar el projecte.
2. Planificació: es determinen els objectius i con comença i acaba el cicle.
3. Anàlisis de risc: s'analitza tot el que pot afectar al projecte.
4. Implementació: es desenvolupa i valida el software.
5. Evaluació: evaluar el cicle que acabem de completar i com avançarem el projecte en el següent cicle.

##### Metodologies àgils
Mètodes d'enginyeria de software basats en el desenvolupament iteratiu i incremental.
Les metodologies més conegudes són:
- Kanban: control segons demanda, sistema de targetes
- Scrum: incremental, se organiza por sprints
- XP (eXtreme Programming): per parelles, el client s'intrega a l'equip de desenvolupament

## LLENGUATGES DE PROGRAMACIÓ
### Obtenció del codi executable
Per obtenir codi binàri executable existeixen dos opcions:
- Compilar
- Interpretar

### Procés de compilació/interpretació
Es du a terme dos fases:
1. Anàlisis lèxic
2. Anàlisis sintàctic
Si no existeixen errors, es genera el codi objecte corresponent.

### Procés de compilació/interpretació
Exemple: C, C++,
Avantatges: execució molt eficient
Desavantatges: s'ha de compilar després de qualsevol modificació

### Llenguatges interpretats
Exemple: PHP, Javascript
Avantatges: el codi font s'interpreta directament
Desavantatges: execució menys eficient

### Java
Llenguatge compilat i interpretat. Java es compila i s'obté un codi binari intermedi anomenat bytecode. Aquest bytecode s'interpreta per executar-lo.
Avantatges: estructurat i orientat a objectes, fàcil d'aprendre, bona documentació i base d'usuaris
Desaventatges: menys eficient que els llenguatges compilats

### Tipus
- declaratius: indiquem el resultat sense especificar els passos. Normalment son llenguatges interpretats.
    - lògics: utilitzen regles (Prolog)
    - funcionals: utilitzen funcions (Lisp, Haskell)
    - algebraicos: utilitzen sentències(SQL)
- imperatius: indiquem els passos a seguir per obtenir un resultat. Els llenguatges orientats a objectes són també llenguatges estructurats. Molts són compilats.
    - estructurats: C
    - orientets a objectes: java
    - multiparadigma: C++, Javascript
- Segons abstracció:
    - Baix nivell: ensamblador
    - Nivell mitjà: C
    - Alt nivell: C++, Java

### Evolució
1. Codi binàri
2. Ensamblador
3. Llenguatges estructurats
4. Llenguatges orientats a objectes

### Criteris per a la selecció d'un llenguatge
- Camp s'aplicació
- Experiència prèvia
- Eines de desenvolupament
- Documentació disponible
- Base d'usuaris
- Reutilització
- Portabilitat
- Imposició client
