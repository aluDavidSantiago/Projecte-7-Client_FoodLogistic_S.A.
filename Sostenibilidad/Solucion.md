# MEMÒRIA DE SOSTENIBILITAT

**Projecte:** Web de FoodLogístic\
**Mòdul:** Sostenibilitat\
**Curs:** CFGM
**Data:** 27-04-2026\
**Alumne/a:** Santiago Hernandez

***

## 1. URL de l’app

<https://aludavidsantiago.github.io/foodlogistic-web/>

***

## 2. Memòria de Sostenibilitat

### a) Recursos utilitzats al projecte

**Extensió de les imatges utilitzades**

*   `.png`: logotip corporatiu.
*   `.avif`: imatge de fons obtinguda d’Unsplash (format modern optimitzat).
*   `.mp4`: dos vídeos formatius a la secció de protecció de dades.

**Mida de les imatges i recursos**

*   Logotip PNG: 193 KB.
*   Vídeo formatiu 1: 8 MB.
*   Vídeo formatiu 2: 10 MB.
*   Pes total de la pàgina (EcoGrader): 19,78 MB.

**Fonts utilitzades**

*   Inter
*   Poppins

**Són fonts de sistema?**
No.\
Són fonts externes carregades des de Google Fonts amb `preconnect`, fet que optimitza el temps de càrrega i redueix la latència.

**Mode fosc**
Sí.\
La web és fosca per defecte, fet que millora la llegibilitat en entorns amb poca llum i redueix el consum energètic en pantalles OLED.

***

### b) Eines per mesurar l’impacte

## Aspecte Ambiental · Suportable

### 1. Website Carbon Calculator

**Resultats obtinguts**

*   Emissions per visita: 2,06 grams de CO₂.
*   Classificació de carboni: F.
*   Més contaminant que el 96 % de les webs analitzades.
*   Ús d’energia estàndard (no renovable).

**Projecció anual**
Amb 10.000 visites mensuals durant un any:

*   247,3 kg de CO₂ equivalents.
*   501 kWh d’energia consumida.
*   Impacte equivalent a l’absorció anual de 12 arbres.

**Comentari**
Tot i que les emissions per visita són moderades, el gran pes dels recursos multimèdia, especialment els vídeos, incrementa l’impacte ambiental anual. L’ús d’un allotjament amb energia verda i la reducció del pes dels vídeos permetria disminuir significativament les emissions.

***

### 2. EcoGrader

**Resultats obtinguts**

*   Puntuació EcoGrader: 40 / 100.
*   Emissions per càrrega: 7,71 g de CO₂.
*   Classificació de carboni digital: E.
*   Pitjor que el 93 % de les URLs analitzades.

**Desglossament d’emissions**

*   Media (vídeos): 19,22 MB – 7,4898 g CO₂e.
*   Imatges: 423 KB – 0,1649 g CO₂e.
*   Scripts: 67,79 KB – 0,0262 g CO₂e.
*   HTML/CSS: 6,68 KB – 0,0023 g CO₂e.

**Comentari**
EcoGrader confirma que el principal impacte ambiental del projecte prové del contingut multimèdia. El codi HTML i CSS té un impacte molt baix, indicador d’una bona base tècnica amb marge de millora mitjançant optimització del contingut audiovisual.

***

## Aspecte Social · Equitatiu (Accessibilitat – A11Y)

L’accessibilitat s’ha tractat com a disseny universal, assegurant que la web sigui usable per al 100 % de la població, incloses persones amb diversitat visual, auditiva o motora, usuaris amb connexions lentes i diferents contextos d’ús.

***

### 3. Lighthouse (Chrome DevTools)

**Eina utilitzada:** Lighthouse – mode Desktop.

**Resultats obtinguts**

*   Performance: 87 / 100.
*   Best Practices: 100 / 100.

**Anàlisi**
La puntuació de Performance és bona, tot i mostrar possibles millores relacionades amb:

*   Recursos multimèdia pesants.
*   Imatges sense amplada i alçada explícites.
*   Optimització de JavaScript.

La puntuació de Best Practices és excel·lent (100), indicant complir totes les bones pràctiques de seguretat i qualitat.

***

## Què cal fer: Criteris clars de millora aplicats

### 1. Contrast i Color

La web utilitza una paleta fosca amb text clar que compleix el mínim de 4.5:1 establert per les WCAG. Això millora la llegibilitat i permet reduir la brillantor del dispositiu, contribuint a l’estalvi energètic.

***

### 2. Alternatives Textuals (Alt Text)

Totes les imatges informatives inclouen l’atribut `alt`, millorant l’accessibilitat per a lectors de pantalla i el posicionament SEO.

**Exemple:**



***

### 3. Navegació per Teclat (Focus)

S’ha comprovat la navegació utilitzant exclusivament la tecla Tab, sense fer ús del ratolí.\
Els elements interactius del menú i de les seccions són accessibles i mostren visualment el focus actiu mitjançant un marc visible, com es pot observar a l’apartat “Serveis”.

***

## Documentació aportada

*   Captura de pantalla del focus visible al navegar amb la tecla Tab.
*   Captures dels resultats de Website Carbon Calculator i EcoGrader.
*   Captura de Lighthouse Desktop.
*   Fragment de codi amb atribut `alt`.
*   Checklist final.

***

## Checklist final

*   Contrast mínim 4.5:1 complert.
*   Imatges amb atribut `alt`.
*   Navegació amb tecla Tab funcional.
*   Focus visible.
*   Lighthouse superat (Performance i Best Practices).

***

## Conclusions sobre la sostenibilitat

### Impacte Ambiental

L’ús de codi semàntic i recursos lleugers redueix el consum de CPU i GPU, però el pes dels vídeos incrementa les emissions. Hi ha marge de millora optimitzant contingut multimèdia i utilitzant energia verda.

### Impacte Social

L’accessibilitat garanteix el dret universal a la informació, eliminant la bretxa digital i permetent l’ús de la web en diferents contextos i capacitats.

### Impacte Econòmic

Una web accessible millora el SEO, evita sancions legals i amplia el mercat potencial, assegurant la viabilitat del projecte.

