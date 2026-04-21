# **T04: Servidor d’impressió**

## **Breu descripció**

## **Introducció**

En el món de la logística, la impressió continua tenint un paper molt important. Documents com ara albarans o fulls de transport necessiten ser impresos de manera constant, i el vostre client no és una excepció.

L'empresa disposa d’un magatzem on el volum d’impressió d’albarans és crític. Si una impressora falla o es col·lapsa, els camions no poden sortir, fet que pot trencar la cadena de fred.

L’objectiu d’aquesta activitat és configurar un **Servidor d’Impressió a Windows Server** que gestioni aquest volum mitjançant **Printer Pooling** (cua d’impressió compartida), de manera que la càrrega de treball es reparteixi entre dos dispositius.

***

## **Descripció de l’activitat**

El servidor haurà de tenir implementats:

*   Els **serveis de directori (Active Directory)**
*   El **servei de servidor d’impressió**

Això permetrà una gestió centralitzada d’usuaris, equips i recursos d’impressió.

El client, integrat al domini, haurà de:

*   Autenticar-se amb credencials de xarxa
*   Accedir als recursos compartits
*   Utilitzar les impressores desplegades des del servidor

Cal documentar **cada pas del procés** com si fos un **informe tècnic d’implementació per a un client real**, utilitzant un llenguatge clar, estructurat i professional.  
S’han de justificar les decisions preses i descriure les configuracions realitzades.

***

## **Fases tècniques de l’activitat**

### **1. Preparació de l’entorn i simulació de maquinari**

*   Verificar o preparar l’entorn necessari, o bé aprofitar-ne un de similar ja existent.
*   Instal·lar i configurar **dues instàncies d’impressora PDF24** al servidor.  
    Als materials de suport es proporciona una guia pas a pas.
*   Assignar noms corporatius a les impressores:
    *   `IMP_MAGATZEM_A`
    *   `IMP_MAGATZEM_B`

***

### **2. Instal·lació del rol i configuració del Pool**

*   Instal·lar el rol **Print and Document Services** al Windows Server.
*   Accedir a la consola **Print Management**.
*   Configurar el **Printer Pooling**:
    *   Accedir a les propietats de `IMP_MAGATZEM_A`.
    *   A la pestanya **Ports**, marcar la casella **Enable printer pooling**.
    *   Seleccionar el port on es troba la segona impressora `IMP_MAGATZEM_B`.
    *   A partir d’aquest moment, ambdues impressores funcionaran sota un mateix nom de xarxa, repartint-se la feina.

**Nota tècnica:**  
A la impressora `IMP_MAGATZEM_A` han de quedar seleccionats **els dos ports virtuals**.

***

### **3. Desplegament automatitzat de la impressora mitjançant una GPO**

L’empresa no vol que els mossos de magatzem hagin d’instal·lar manualment la impressora.

*   Crear una **GPO (Group Policy Object)** anomenada:
    *   `GPO_Impressores_Magatzem`
*   Utilitzar l’opció **Deploy with Group Policy** des de la consola **Print Management** per vincular la impressora:
    *   Al domini
    *   O a una **Unitat Organitzativa (OU)** específica on es trobi l’usuari de proves
*   Comprovar que, en iniciar sessió en un client **Windows 11**, la impressora apareix automàticament.

**Nota tècnica:**  
Pot ser necessari:

*   Tancar la sessió de l’usuari
*   I/o forçar l’actualització de les directives amb l’ordre:

```bash
gpupdate /force
```

***

### **4. Prova de càrrega i seguretat**

*   **Simulació de balanceig**:
    *   Enviar 10 documents seguits a la impressora del magatzem.
    *   Observar com el servidor reparteix les peticions entre les dues instàncies.
*   **Restriccions d’ús**:
    *   Configurar les **Printing Priorities** o els **Available Times**
    *   Limitar el funcionament de la impressora a l’horari laboral (per exemple, de 06:00 a 22:00).

***

## **Material de suport**

*   **0224 SOX. Material UD8: AA3** (Moodle de l’assignatura)
*   **Guia tècnica: Instal·lació i configuració PDF24**
*   Repositori:
    *   <https://github.com/cfugarolas/activitats/blob/main/activitat3/pdf24.md>  
        Instal·lació i configuració PDF24
