# Implantación de una intranet empresarial con WordPress

## Empresa: *malambo*

**Alumno:** Santiago Hernandez  
**Módulo:** Aplicaciones web  
**Resultado de aprendizaje:** RA3 – Implantación y configuración de servicios web  
**Herramientas utilizadas:** Local WP, WordPress, WP File Manager  
**Entorno:** Desarrollo local

***

## 1. Introducción

En el presente proyecto se ha realizado la implantación de una intranet empresarial para la empresa ficticia **malambo**, especializada en servicios informáticos. El objetivo principal es disponer de una plataforma web interna que permita organizar documentación, gestionar usuarios y simular un entorno real de trabajo corporativo.

La solución adoptada se ha basado en **WordPress**, ampliado mediante plugins específicos que permiten añadir funcionalidades de gestión documental y control de accesos. El proyecto se ha desarrollado íntegramente en un entorno local para facilitar las pruebas y evitar riesgos sobre un sistema en producción.

***

## 2. Preparación del entorno de trabajo (RA3)

Para la realización del proyecto se ha utilizado **Local WP**, una herramienta que permite crear entornos locales completos con servidor web, base de datos y WordPress preinstalado.

El sitio creado simula formar parte de la intranet interna de la empresa malambo, incluyendo información de autoría visible tanto en el nombre del sitio como en la organización de los contenidos.

### 2.1 Instalación de Local WP

Se procedió a la descarga de Local WP desde su página oficial y se realizó la instalación siguiendo el asistente por defecto. Una vez completada la instalación, se accedió a la interfaz principal desde la cual se gestionan los distintos proyectos WordPress locales.


***

## 3. Creación y configuración del sitio WordPress

Se creó un nuevo sitio WordPress con el nombre:

**malambo-intranet-Nombre-Apellidos**

Este nombre permite identificar claramente tanto la empresa como el autor del proyecto. Durante el proceso de instalación se configuró el entorno recomendado (*Preferred*) y se creó el usuario administrador con credenciales personalizadas y una contraseña segura.

### 3.1 Acceso al panel de administración

Una vez finalizada la instalación, se accedió correctamente al panel de administración de WordPress mediante la ruta `/wp-admin`, verificando el correcto funcionamiento del sistema.

### 3.2 Configuración básica del sitio

Dentro del apartado **Ajustes → Generales** se configuraron los parámetros básicos del sitio:

*   Título del sitio:  
    *Intranet Empresa malambo – Nombre Apellidos*
*   Descripción:  
    *Plataforma interna de gestión documental y servicios digitales de la empresa malambo*
*   Idioma del sitio
*   Zona horaria: Europe/Madrid

Estos ajustes permiten adaptar WordPress a un contexto de intranet corporativa.

### 3.3 Configuración de enlaces permanentes

Para mejorar la organización de las URLs y la compatibilidad con plugins, se configuraron los enlaces permanentes utilizando la opción **Nombre de la entrada**.

***

## 4. Implantación del gestor de archivos web

Con el objetivo de dotar a la intranet de capacidades de gestión documental, se instaló el plugin **WP File Manager**, que permite administrar archivos y carpetas del servidor desde el panel de administración de WordPress.

### 4.1 Instalación del plugin

El plugin se instaló desde el repositorio oficial de WordPress y se activó correctamente, apareciendo una nueva opción en el menú lateral.

### 4.2 Acceso inicial y consideraciones de seguridad

Al acceder al gestor de archivos, se comprobó que permite visualizar toda la estructura del servidor, incluidos archivos críticos del sistema. Por este motivo, se decidió trabajar únicamente dentro de una carpeta de prácticas creada específicamente para el proyecto, evitando modificar archivos sensibles.

***

## 5. Creación de directorio seguro y estructura documental

Dentro de la carpeta `wp-content` se creó el directorio:

    uploads-malambo-Nombre-Apellidos

En su interior se creó la carpeta principal de la empresa:

    Empresa-malambo-Nombre-Apellidos

Y dentro de ella la siguiente estructura documental:

    Empresa-malambo-Nombre-Apellidos
    ├── Documents
    ├── Projectes
    ├── Recursos
    └── Clients

Esta estructura simula la organización documental interna de una empresa real.

***

## 6. Subida y clasificación de archivos

Se subieron distintos archivos de prueba, clasificándolos correctamente según su finalidad:

*   **Documents:** Documento PDF con normas internas.
*   **Projectes:** Documento de texto con una propuesta de proyecto.
*   **Recursos:** Imagen de la rana Pepe como recurso gráfico.
*   **Clients:** Archivo relacionado con un cliente ficticio.

Algunos archivos incluyen el nombre y apellidos del alumno para reforzar la autoría.

***

## 7. Creación de usuarios y roles

Para simular el funcionamiento real de una empresa, se crearon distintos usuarios con roles específicos:

| Usuario       | Rol           |
| ------------- | ------------- |
| Administrador | Administrator |
| Director      | Editor        |
| Trabajador    | Author        |
| Externo       | Subscriber    |

Cada rol tiene permisos diferentes acordes a su función.

***

## 8. Pruebas de permisos y acceso

Se realizaron pruebas iniciando sesión con cada tipo de usuario para comprobar los permisos:

*   El usuario externo solo puede consultar información.
*   El trabajador puede crear y editar sus propios contenidos.
*   El director puede gestionar contenidos de otros usuarios.
*   El administrador tiene control total del sistema.

Estas pruebas demuestran una correcta separación de roles y un control básico de accesos.

***

## 9. Comprobación de seguridad e integridad

Se comprobó que:

*   El gestor de archivos solo es accesible por el administrador.
*   Todo el trabajo se ha realizado dentro de la carpeta de prácticas.
*   No se han modificado archivos del núcleo de WordPress.
*   El sitio continúa funcionando correctamente.

El uso del gestor de archivos se considera seguro en este contexto al estar limitado a un entorno de desarrollo y con control de accesos adecuado.

***

# IMGs

<img src="IMG/cri2.png" alt="..." width="700" height="auto"> 

<img src="IMG/cri1.png" alt="..." width="700" height="auto"> 

## 10. Conclusión

La implantación de la intranet para la empresa malambo ha permitido crear un entorno web funcional que simula una plataforma empresarial real. Se han trabajado aspectos como la gestión documental, la organización de la información, los permisos de usuario y la seguridad del sistema.

Este proyecto constituye una base sólida sobre la cual se podrán integrar en fases posteriores servicios adicionales como ofimática web, calendarios o gestión de tareas.


