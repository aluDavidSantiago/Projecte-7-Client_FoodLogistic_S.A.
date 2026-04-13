Aquí tens **tot el contingut del T03 convertit a Markdown**, net, estructurat i sense cap element extra:

***

# T03: Servidor de fitxers

## Breu descripció

## Introducció

Quan el volum de negoci creix, també augmenta el volum de dades, i sovint apareixen problemes de desorganització i manca de visió global.  
A FoodLogistic, cada departament emmagatzemava documentació localment, generant dispersió i risc.

L’objectiu de la tasca és **implementar una infraestructura de fitxers segura, organitzada i controlada**, utilitzant:

*   Permisos NTFS i SMB
*   Quotes
*   Filtratge de fitxers (FSRM)

Cal demostrar domini de tres vies d’administració:

*   Explorador de Fitxers
*   Server Manager
*   PowerShell

***

# Descripció de l'activitat

L’activitat es divideix en fites que simulen un procés real de consultoria i implantació.

***

# 1. Preparació i Seguretat de Grups (Active Directory)

Abans de crear el servidor de fitxers, cal preparar l’Active Directory sobre el domini **foodlogistic.test**, amb una estructura d’OUs coherent i justificada segons les necessitats detectades.

S’han de crear els següents **grups de seguretat**:

| Grup          | Funció                        |
| ------------- | ----------------------------- |
| Administracio | Gestió de factures i albarans |
| Transport     | Xofers i caps de flota        |
| Direccio      | Gerència                      |

***

# 2. Implementació de Recursos Compartits (Tres mètodes)

S’han de crear estructures de carpetes al servidor utilitzant mètodes diferents.

***

## A. Carpeta *Public* (Mètode: Explorador d’Arxius)

*   Compartida per a tots els usuaris.
*   Configuració:
    *   Permisos **SMB: Lectura**
    *   Permisos **NTFS: Modificació**
*   Verificar la combinació de permisos efectiva.

***

## B. Carpeta *Operacions* (Mètode: Server Manager - FSSM)

Passos:

1.  Instal·lar el rol **File and Storage Services** (si no està instal·lat).
2.  Crear el recurs compartit via Server Manager.
3.  Activar **Access-Based Enumeration**.
4.  Restricció: només el grup **Transport** pot accedir.

***

## C. Carpeta *Confidencial* (Mètode: PowerShell bàsic)

*   Crear carpeta **Direccio$** (recurs ocult).
*   Accessos: només el grup **Direccio**.
*   Compartir amb:
    ```powershell
    New-SmbShare -Name "Direccio$" -Path "C:\Direccio" -FullAccess "Direccio"
    ```
*   Crear GPO que munti automàticament la unitat **Z:** per als usuaris del grup Direccio.

***

## D. Carpeta *Confidencial* (Mètode: PowerShell avançat)

(*Opcional, més puntuació*)

*   Crear carpeta **Direccio**.
*   Accessos: només el grup **Direccio**.
*   Compartir amb:
    ```powershell
    New-SmbShare -Name "Direccio" -Path "C:\Direccio" -FullAccess "Direccio" -FolderEnumerationMode AccessBased
    ```
*   Habilitar Access-Based Enumeration via PowerShell.
*   Crear GPO per mapar unitat **Z:** als usuaris de Direccio.

> Cal triar entre el mètode C o D (D té més puntuació).

***

# 3. Control d’Emmagatzematge (FSRM i Quotes NTFS)

FoodLogistic detecta que els usuaris emmagatzemen fotos personals i omplen el disc. Cal aplicar mesures de control.

***

## Quotes NTFS (Control per Volum)

*   Activar quotes NTFS a la unitat de dades.
*   Límit per defecte: **500 MB per usuari nou**.

***

## FSRM (Control per Carpeta)

### A. Quota de Carpeta

A la carpeta **Public**:

*   Quota de **200 MB Hard Quota**
*   Avís al **90%** amb el missatge:
        Compte! FoodLogístic t'informa que estàs a punt d'esgotar l'espai compartit.

### B. Filtrat de Fitxers

A la carpeta **Operacions**:

*   Bloquejar:
    *   Arxius executables (.exe, .msi)
    *   Fitxers d'àudio i vídeo

***

# 4. Verificació i Auditoria

Des d’un client Windows 10/11:

*   Verificar accés i visibilitat segons cada grup.
*   Provar còpia d’un `.exe` a Operacions (ha de ser bloquejat).
*   Provar renombrar `.exe` a `.txt` per comprovar si el filtratge actiu el detecta.

***

# Què cal lliurar

Lliurar un informe tècnic en **format Markdown** amb:

## 1. Resum de Configuració

Incloure una taula amb:

*   Nom de carpeta
*   Camí UNC
*   Grups amb accés
*   Mètode utilitzat (Explorador, Server Manager o PowerShell)

## 2. Evidències

Captures i explicacions de:

*   Permisos
*   Quotes NTFS
*   Configuracions FSRM
*   GPO de mapatge

## 3. Proves de Funcionament

Des del client:

*   Resultats de les proves d’accés
*   Quotes en acció
*   Bloqueig de fitxers restringits

***

# Material de suport

*   0224 SOX. Material UD8: AA2 (Moodle de l’assignatura)

***

Si vols, també puc preparar:

*   La plantilla del teu informe final en Markdown
*   Les taules ja estructurades
*   Scripts PowerShell completament funcionals
*   Un exemple d’evidències o esquema de GPO

Només digues què necessites.
