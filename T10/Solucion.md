# T10 – Pressupost del Projecte

## Proposta econòmica per a FoodLogístic S.A.

***

## 1. Introducció

Aquest document presenta la proposta econòmica del projecte de modernització dels sistemes informàtics de **FoodLogístic S.A.**, empresa logística amb una plantilla de **35 treballadors**, d’acord amb els requisits definits a l’activitat **T10 – Pressupost del projecte**.

La proposta inclou:

*   El **cost d’implantació inicial (pagament únic)**.
*   Els **costos recurrents mensuals i anuals** necessaris per garantir el funcionament continu, la seguretat i el manteniment del sistema.

Tots els imports estan basats en **preus reals de mercat**, obtinguts de fonts oficials i comercials contrastades.

***

## 2. Cost d’implantació (pagament únic)

### 2.1. Infraestructura cloud i programari (implantació)

La infraestructura cloud es basa en **Microsoft Azure**, amb servidors virtuals en alta disponibilitat.  
El desplegament inicial inclou la creació de les màquines virtuals, configuració del sistema operatiu i serveis bàsics.

| Concepte                                | Descripció                                                                   | Cost (€) |
| --------------------------------------- | ---------------------------------------------------------------------------- | -------- |
| Configuració infraestructura Azure HA   | Creació i configuració inicial de 2 VMs Windows Server (fitxers i impressió) | 0 €      |
| Programari base servidor                | Windows Server inclòs en el cost cloud                                       | 0 €      |
| **Total infraestructura (implantació)** |                                                                              | **0 €**  |

Nota: El cost de les màquines virtuals Azure es reflecteix als **costos recurrents**, ja que es factura mensualment.

***

### 2.2. Honoraris professionals (mà d’obra)

**Tarifa professional aplicada:**  
**40 €/hora**

La tarifa s’ajusta al mercat espanyol de consultoria IT. Segons SalaryExpert, la mitjana se situa al voltant de **32,74 €/hora**, sent habitual aplicar una tarifa superior en serveis facturats a client final.

| Tasca                                     | Hores     | Cost (€)    |
| ----------------------------------------- | --------- | ----------- |
| Disseny i desplegament infraestructura HA | 40 h      | 1.600 €     |
| Migració i configuració Microsoft 365     | 20 h      | 800 €       |
| Elaboració vídeo formatiu LOPD            | 15 h      | 600 €       |
| Desenvolupament landing page corporativa  | 25 h      | 1.000 €     |
| Documentació i validació final            | 10 h      | 400 €       |
| **Total mà d’obra**                       | **110 h** | **4.400 €** |

**Font de preus (mercat laboral IT):**  
<https://www.salaryexpert.com/salary/job/it-consultant/spain>

***

### 2.3. Total cost d’implantació

| Concepte              | Import (€)  |
| --------------------- | ----------- |
| Infraestructura cloud | 0 €         |
| Mà d’obra             | 4.400 €     |
| **TOTAL IMPLANTACIÓ** | **4.400 €** |

***

## 3. Costos recurrents (manteniment i subscripcions)

### 3.1. Infraestructura cloud Azure (servei mensual)

Per garantir alta disponibilitat, s’utilitzen **2 màquines virtuals Windows Server** a Microsoft Azure.

Configuració utilitzada:

*   Tipus: **Standard D4 v4**
*   4 vCPU
*   16 GB RAM
*   Región: West Europe
*   Model: **1 any reservat**
*   Cost mensual per VM: **199,46 €**

| Concepte                          | Cost mensual |
| --------------------------------- | ------------ |
| Azure – 2 VMs Windows Server (HA) | 398,92 €     |

**Font oficial Microsoft Azure:**  
<https://azure.microsoft.com/pricing/details/virtual-machines/windows/>

***

### 3.2. Plataforma SaaS – Correu i col·laboració

S’ha escollit **Microsoft 365 Empresa Estàndard**, amb subscripció anual i pagament mensual.

*   Preu oficial: **10,80 € / usuari / mes**
*   Nombre d’usuaris: **35**

| Concepte                        | Usuaris | Cost mensual |
| ------------------------------- | ------- | ------------ |
| Microsoft 365 Empresa Estàndard | 35      | 378,00 €     |

**Font oficial Microsoft:**  
<https://www.microsoft.com/es-es/microsoft-365/business/microsoft-365-plans-and-pricing>

***

### 3.3. Hosting i domini web

S’ha previst un allotjament web professional compartit, adequat per a una landing page corporativa.

| Concepte                 | Cost     |
| ------------------------ | -------- |
| Hosting web professional | 10 €/mes |
| Domini web (.com o .es)  | 12 €/any |

**Fonts de referència:**  
<https://www.deordenadores.com/hosting-espana/>  
<https://www.hostinger.com/es/precios>

***

### 3.4. Suport i manteniment IT

Servei mensual que inclou:

*   Gestió d’incidències Microsoft 365
*   Supervisió bàsica de la infraestructura Azure
*   Còpies de seguretat
*   Actualitzacions de seguretat
*   Suport tècnic remot

| Servei                          | Cost  |
| ------------------------------- | ----- |
| Quota mensual de manteniment IT | 250 € |

***

### 3.5. Total costos recurrents

| Concepte                  | Import             |
| ------------------------- | ------------------ |
| Azure (VMs)               | 398,92 €/mes       |
| Microsoft 365             | 378,00 €/mes       |
| Hosting web               | 10,00 €/mes        |
| Manteniment IT            | 250,00 €/mes       |
| **Total mensual**         | **1.036,92 €/mes** |
| **Total anual aproximat** | **12.443 €/any**   |

***

## 4. Justificació de la proposta econòmica

Els imports presentats es basen en **preus reals i fonts contrastades**:

*   **Azure**: calculadora oficial de Microsoft (VMs Windows Server, West Europe).
*   **Microsoft 365**: preus oficials de Microsoft per a Empresa Estàndard.
*   **Hosting**: comparatives actualitzades de proveïdors a Espanya.
*   **Tarifa professional**: salaris reals del mercat IT i extrapolació a serveis de consultoria.

El model de costos garanteix:

*   Transparència econòmica.
*   Coherència tècnica.
*   Escalabilitat futura.
*   Adequació als requisits empresarials de FoodLogístic S.A.

***

## 5. Conclusió

Aquest pressupost compleix els requisits de l’activitat **T10 – Pressupost del Projecte**, presentant una proposta:

*   Realista
*   Justificada amb fonts oficials
*   Tècnicament correcta
*   Alineada amb el mercat actual

