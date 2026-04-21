# **T09: Estimació temporal de projecte (Diagrama de Gantt professional)**

## **Breu descripció**

Un dels errors més habituals en equips tècnics novells és confondre *fer feina* amb *gestionar un projecte*.

Començar a configurar servidors, desenvolupar una web o desplegar serveis sense una planificació rigorosa acostuma a provocar:

*   Retards
*   Colls d’ampolla
*   Solucions improvisades

En aquest punt del projecte, la direcció de **FoodLogístics S.A.** no vol només una proposta tècnica, sinó **garanties**.

Vol saber:

*   Quan estaran les solucions operatives
*   Quin ordre se seguirà
*   Què passarà si alguna tasca es retarda
*   Si l’equip és capaç de treballar de manera professional

Per tant, l’objectiu **no és fer un Gantt**, sinó demostrar que sabeu **planificar un projecte real** amb criteri tècnic i organitzatiu.

***

## **Objectius específics / Finalitat de la tasca**

Treballareu com a **equip de projecte** per construir una planificació completa i realista del desplegament de la solució per a FoodLogístics S.A., utilitzant un **diagrama de Gantt** generat amb:

*   **PlantUML (UMLTree)**  
    <https://plantuml.com/es/>
*   **Editor per visualitzar codi UMLTree**  
    <https://www.planttext.com/>

L’activitat es divideix en diverses fases.

***

## **Fase 1: Anàlisi real del projecte (pensament estructural)**

### **1.1 Identificació de tasques i dependències**

A partir de les tasques reals del projecte (**T01–T08**), heu d’identificar:

*   L’ordre lògic d’execució
*   Les tasques que es poden executar en paral·lel
*   Les tasques bloquejants

Heu de respondre preguntes com:

*   Quines tasques no poden començar sense haver-ne acabat una altra?
*   On poden aparèixer colls d’ampolla?
*   Quines tasques són més crítiques per al projecte?

***

### **1.2 Identificació del camí crític**

Heu de determinar:

*   Quines tasques, si es retarden, afecten tot el projecte.
*   Quines tasques tenen marge (*slack*).

No es tracta només d’identificar el camí crític, sinó d’**entendre’l**.

***

## **Fase 2: Estimació d’esforç amb criteri (ús d’IA guiat)**

Heu d’estimar la durada de cada tasca en hores, **no de forma arbitrària**.

### **Factors obligatoris d’estimació**

Per a cada tasca, cal tenir en compte com a mínim:

*   Temps de comprensió (lectura i anàlisi)
*   Temps de recerca (si cal)
*   Temps d’implementació tècnica
*   Temps de proves i correcció d’errors
*   Temps de documentació
*   Coordinació amb l’equip
*   Possibles interrupcions (classes, exàmens, altres tasques)
*   Temps de marge per a imprevistos

***

### **Ús d’IA (obligatori i guiat)**

Cal utilitzar la IA com a **assistència**, però sempre amb criteri tècnic i justificació raonada.

***

## **Fase 3: Assignació de recursos (treball en equip real)**

Distribuïu les tasques entre els membres de l’equip indicant:

*   Qui fa què
*   Quines tasques són compartides
*   Dependències entre membres de l’equip

Cal evitar:

*   La sobrecàrrega d’una sola persona
*   Temps morts a la resta de l’equip

***

## **Fase 4: Construcció del diagrama de Gantt (UMLTree)**

Utilitzant **PlantUML (UMLTree)**, el diagrama ha de mostrar:

*   Tasques del projecte (**T01–T08**)
*   Durada de cada tasca
*   Dependències entre tasques
*   Execució en paral·lel
*   Visió temporal del projecte (3–4 setmanes)

El diagrama **no és només visual**, ha de reflectir decisions reals de planificació.

***

## **Fase 5: Pla de contingència (pensament professional)**

Heu d’identificar com a mínim:

*   **Dos riscos crítics** reals (escenaris ficticis no són vàlids)
*   L’impacte de cada risc en el projecte
*   Una estratègia clara de mitigació

Exemples:

*   Retard en el servidor → ús de buffers o paral·lelització
*   Problemes amb serveis cloud → alternativa definida

***

## **Què cal lliurar**

El lliurament s’haurà de fer dins del **repositori del projecte** i ha d’incloure com a mínim:

***

### **1. Document de planificació (README.md)**

Ubicat a la carpeta:

    /P01/Planificacio/

Aquest document ha de funcionar com un **informe professional de planificació** i ha d’incloure:

*   Introducció al context i objectiu de la planificació
*   Explicació de l’ordre de les tasques i dependències
*   Justificació de les estimacions temporals
*   Distribució del treball setmana a setmana
*   Decisions clau preses per l’equip
*   Reflexió sobre possibles colls d’ampolla o punts crítics

El document ha d’estar:

*   Ben estructurat
*   Redactat amb claredat
*   Amb format visual correcte

Cal incorporar captures de pantalla, imatges del diagrama i evidències rellevants.

***

### **2. Codi PlantUML i imatge del diagrama de Gantt**

Dins la mateixa carpeta de planificació:

*   Arxiu amb el codi PlantUML
*   Imatge exportada del diagrama de Gantt

El diagrama ha de mostrar:

*   Les 4 setmanes de planificació
*   Tasques del projecte
*   Paral·lelismes i solapaments
*   Relació temporal entre activitats i resultats

El diagrama ha de ser **coherent amb el README.md**.

***

### **3. Matriu d’assignació de responsabilitats (RACI)**

Cal elaborar una taula RACI indicant, com a mínim:

*   Qui executa la tasca (Responsible)
*   Qui en fa la validació final (Accountable)
*   Qui ha de ser consultat (Consulted)
*   Qui ha de ser informat (Informed)

L’objectiu és demostrar una **organització professional del treball en equip**.

***

### **4. Taula de riscos i contingències**

Cal incloure una taula amb:

*   El risc o incidència possible
*   La part del projecte afectada
*   L’impacte en la planificació
*   La mesura de contingència o resposta prevista

No es tracta només d’identificar problemes, sinó d’anticipar decisions.

***

## **Important**

Tots els elements del lliurament han d’estar **connectats entre si**:

*   El README explica la lògica del projecte
*   El Gantt la representa visualment
*   La RACI mostra la coordinació
*   La taula de riscos anticipa desviacions

El conjunt ha de transmetre que sou un equip capaç de **planificar, coordinar i justificar** un projecte real.

***

## **Preguntes clau (obligatòries al README)**

*   Quina és la tasca més crítica del projecte i per què?
*   On heu detectat el principal coll d’ampolla?
*   Quina decisió de planificació ha estat més difícil?
*   Heu modificat alguna estimació inicial? Per què?
*   Quin risc podria fer fracassar el projecte?
*   Si tinguéssiu una setmana més, què canviaríeu?

***

## **Criteris de qualitat**

Es valorarà especialment:

*   Coherència del Gantt amb el projecte
*   Realisme de les estimacions
*   Comprensió de dependències
*   Capacitat d’anticipar problemes
*   Qualitat professional del README
*   Ús crític i justificat de la IA
