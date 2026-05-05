# Intranet empresarial amb WordPress (Projecte malambo)**

## ** Descripció del projecte**
Aquest repositori conté el desenvolupament complet del projecte **Implantació d’una intranet empresarial amb WordPress** per a l’empresa fictícia *malambo*.  
L’objectiu és crear una plataforma interna que permeti als treballadors:

- compartir documents
- treballar amb documents online
- gestionar correu electrònic
- organitzar calendaris i tasques
- accedir a tota la informació des d’un portal web

La intranet s’ha implementat amb **WordPress**, ampliat amb plugins que afegeixen funcionalitats de gestió documental, ofimàtica web, calendari i gestió de projectes.

---

## ** Estructura del projecte**
El projecte es divideix en quatre grans blocs:

### **1️ Instal·lació i configuració inicial de WordPress**
Inclou:
- Instal·lació de Local WP  
- Creació del lloc WordPress  
- Configuració d’usuari administrador  
- Ajustos generals (idioma, zona horària, títol, permalinks)

### **2️ Gestor d’arxius web**
Mitjançant el plugin **WP File Manager**, s’ha implementat:
- Creació d’una estructura documental corporativa  
- Pujada i classificació d’arxius  
- Configuració de permisos i rols  
- Proves de gestió documental (pujar, moure, renombrar, eliminar)

### **3️ Ofimàtica web**
Integració amb **Google Docs** per permetre:
- Creació de documents, fulls de càlcul i presentacions  
- Inserció dels documents a WordPress amb *Embed Google Docs*  
- Proves de treball col·laboratiu en temps real

### **4️ Aplicacions web d’escriptori**
Ampliació de la intranet amb:
- Calendari corporatiu (plugin *The Events Calendar*)  
- Gestió de projectes i tasques (plugin *WP Project Manager*)  
- Creació d’esdeveniments i tasques  
- Verificació del funcionament

---

## ** Arquitectura de la solució**
```
Servidor web
   ↓
 WordPress
   ↓
 Plugins
```

### **Plugins utilitzats**
| Servei | Plugin |
|--------|--------|
| Gestor d’arxius | WP File Manager |
| Ofimàtica web | Embed Google Docs / OnlyOffice connector |
| Correu web | WP Mail Logging / Roundcube embed |
| Calendari | The Events Calendar |
| Gestió d’usuaris | User Role Editor |
| Seguretat | Wordfence |
| Gestió de projectes | WP Project Manager |

---

## ** Gestió d’usuaris i permisos**
S’han creat els següents rols:

- Administrador – control total  
- Editor – pot editar continguts  
- Author – pot crear continguts propis  
- Subscriber – només pot consultar  

S’han fet proves d’accés per validar que cada rol té les capacitats correctes.

---

## ** Estructura documental creada**
```
Empresa
├── Documents
├── Projectes
├── Recursos
└── Clients
```

Inclou carpetes personalitzades amb el nom i cognoms de l’alumne per garantir l’autoria.

---

## ** Documents d’ofimàtica creats**
- Document de text: *Informe intern malambo – Nom Cognoms*  
- Full de càlcul: *Control de projectes malambo – Nom Cognoms*  
- Presentació: *Presentació intranet malambo – Nom Cognoms*

Tots ells integrats a la pàgina **Oficina digital malambo**.

---

## ** Calendari i tasques**
### **Esdeveniments creats**
- Reunió tècnica  
- Revisió intranet  
- Formació interna  

### **Projecte creat**
**Implementació intranet malambo – Nom Cognoms**, amb tasques:
- Configuració WordPress  
- Gestor documental  
- Integració ofimàtica  

---

## ** Captures de pantalla**
El repositori inclou (o inclourà) una carpeta `/captures` amb:
- Instal·lació Local WP  
- Panell d’administració  
- Configuració de plugins  
- Gestor d’arxius  
- Documents incrustats  
- Calendari i tasques  

---

## ** Proves realitzades**
- Accés amb diferents rols  
- Gestió d’arxius (pujar, moure, renombrar, eliminar)  
- Edició col·laborativa en Google Docs  
- Creació i consulta d’esdeveniments  
- Gestió de tasques i projectes  

---

## ** Informe tècnic**
El projecte inclou un informe PDF amb:
- Explicació de cada fase  
- Captures de pantalla  
- Comentaris tècnics  
- Problemes trobats i solucions  

---

## ** Objectiu final**
Aquest projecte prepara la base per a futures ampliacions de la intranet, incloent:
- aplicacions internes
- gestió documental avançada
- integració amb serveis corporatius

