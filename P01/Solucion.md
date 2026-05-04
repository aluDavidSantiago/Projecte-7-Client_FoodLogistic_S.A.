P01 – Memoria técnica del proyecto

## Propuesta de infraestructura, seguridad y presencia web

**Cliente:** FoodLogístic S.A.  
**Proyecto Intermodular – CFGM SMX2**  
**Autores:** David Hernandez/ Santiago Moreno

***

## 1. Introducción

El presente documento constituye la **memoria técnica completa del proyecto FoodLogístic S.A.**, desarrollado en el marco del módulo de **Proyecto Intermodular** del ciclo formativo SMX2.

El objetivo principal de esta memoria es **documentar, justificar y explicar detalladamente** la solución técnica propuesta al cliente, de forma que pueda:

*   Entender qué se ha realizado
*   Evaluar la viabilidad técnica y organizativa
*   Visualizar la infraestructura y los servicios
*   Tomar decisiones informadas antes de su implantación

No se trata únicamente de describir el resultado final, sino de **explicar el proceso completo**, desde el análisis inicial hasta las conclusiones y aprendizajes adquiridos.

***

## 2. Análisis inicial y necesidades del cliente

### 2.1 Situación inicial

FoodLogístic S.A. es una empresa del sector de la logística alimentaria que presenta una estructura típica de PYME, con distintos departamentos y usuarios que trabajan con información sensible.

En el punto de partida del proyecto:

*   No existía una **infraestructura IT centralizada**
*   La gestión de usuarios era poco estructurada
*   No se garantizaba el **cumplimiento normativo** (RGPD / LOPDGDD)
*   No había una **presencia web corporativa** formal
*   No existía un plan de concienciación en seguridad para los empleados

***

### 2.2 Necesidades detectadas

A partir del análisis, se identificaron las siguientes necesidades:

| Área               | Necesidad                                 |
| ------------------ | ----------------------------------------- |
| Usuarios           | Gestión centralizada y segura             |
| Datos              | Compartición de ficheros con permisos     |
| Impresión          | Sistema de impresión compartido           |
| Seguridad          | Control de accesos y formación RGPD       |
| Legal              | Cumplimiento normativo obligatorio        |
| Imagen corporativa | Web informativa y legal                   |
| Gestión            | Planificación y organización del proyecto |

Este análisis sirve como base para definir la **propuesta de solución**.

***

## 3. Propuesta de solución global

La solución planteada se basa en una infraestructura **realista, escalable y alineada con entornos profesionales**, combinando servidores locales, servicios web y buenas prácticas de seguridad.

La propuesta se divide en cuatro grandes bloques:

1.  Infraestructura local
2.  Servicios y presencia web
3.  Seguridad y protección de datos
4.  Gestión y planificación del proyecto

***

## 4. Infraestructura técnica (T01, T03, T04)

### 4.1 Objetivo de la infraestructura

El objetivo principal era crear un entorno donde:

*   Los usuarios se autentiquen de forma centralizada
*   Los recursos estén organizados por departamentos
*   Se puedan aplicar políticas de seguridad
*   El mantenimiento sea sencillo

***

### 4.2 Tecnologías utilizadas

| Elemento                   | Tecnología                 |
| -------------------------- | -------------------------- |
| Sistema operativo servidor | Windows Server             |
| Gestor de dominio          | Active Directory           |
| Compartición de archivos   | NTFS + SMB                 |
| Impresión                  | Servidor de impresión      |
| Políticas                  | Group Policy Objects (GPO) |

***

### 4.3 Active Directory

#### Qué se tenía que hacer

*   Centralizar la gestión de usuarios y equipos
*   Organizar la empresa por departamentos

#### Qué se hizo

*   Creación de un dominio corporativo
*   Definición de Unidades Organizativas (OU)
*   Alta de usuarios por departamento
*   Asociación de equipos al dominio

#### Cómo se hizo

*   Instalación del rol AD DS
*   Promoción del servidor como controlador de dominio
*   Estructuración lógica del directorio

***

### 4.4 Servidor de ficheros (T03)

#### Objetivo

Proporcionar almacenamiento compartido con acceso controlado.

#### Implementación

*   Carpetas por departamento
*   Permisos NTFS diferenciados
*   Acceso solo a usuarios autorizados

| Departamento   | Permisos            |
| -------------- | ------------------- |
| Administración | Lectura / Escritura |
| Logística      | Lectura / Escritura |
| RRHH           | Acceso restringido  |

***

### 4.5 Servidor de impresión (T04)

#### Qué se necesitaba

*   Centralizar impresoras
*   Optimizar recursos

#### Qué se implementó

*   Servidor de impresión
*   Printer pooling
*   Despliegue mediante GPO

Esto permite una gestión eficiente y transparente para los usuarios.

***

## 5. Seguridad y protección de datos (RGPD / LOPDGDD)

### 5.1 Medidas técnicas

*   Control de accesos por usuario
*   Separación de datos sensibles
*   Políticas de seguridad mediante GPO
*   Reducción del riesgo de accesos indebidos

***

### 5.2 Medidas organizativas

Uno de los puntos clave del proyecto fue la **concienciación del personal**.

#### Qué se hizo

*   Creación de vídeos informativos sobre:
    *   Uso correcto de datos personales
    *   Buenas prácticas de seguridad
*   Diferenciación de contenidos:
    *   Usuarios generales
    *   Departamento de RRHH

Esto demuestra que la seguridad no es solo técnica, sino también humana.

***

## 6. Presencia web corporativa

### 6.1 Objetivo de la web

Disponer de una web:

*   Informativa
*   Profesional
*   Legalmente correcta

***

### 6.2 Tecnologías utilizadas

*   HTML5
*   CSS
*   GitHub Pages
*   Git como sistema de control de versiones

***

### 6.3 Contenido legal obligatorio

Se desarrollaron e integraron:

*   Aviso legal
*   Política de privacidad
*   Política de cookies

Cumpliendo con:

*   RGPD
*   LOPDGDD
*   LSSI-CE

***

## 7. Control de versiones y repositorio (P02)

El proyecto se gestionó mediante **GitHub**, aplicando buenas prácticas:

*   Commits frecuentes
*   Mensajes descriptivos
*   Historial trazable

📦 Repositorio:  
<https://github.com/classesSMX2n/web-projecte7-aluDavidSantiagoy>

🌐 Web desplegada:  
<https://classessmx2n.github.io/web-projecte7-aluDavidSantiago/>

***

## 8. Planificación del proyecto (T09)

El proyecto se planificó mediante un **diagrama de Gantt**, donde se definieron:

*   Fases
*   Dependencias
*   Tiempos estimados
*   Orden lógico de implementación

Esto permitió:

*   Detectar riesgos
*   Organizar el trabajo
*   Justificar la viabilidad del proyecto

***

## 9. Problemas encontrados y soluciones

| Problema            | Solución aplicada            |
| ------------------- | ---------------------------- |
| Gestión de permisos | Estructuración clara de NTFS |
| Organización del AD | Uso correcto de OU           |
| Cumplimiento legal  | Documentación web específica |
| Coordinación        | Planificación previa         |

***

## 10. Aprendizajes adquiridos

Durante el desarrollo del proyecto se aprendió:

*   A diseñar una infraestructura realista
*   A documentar técnicamente un proyecto
*   A trabajar con visión de cliente
*   A cumplir normativas legales
*   A utilizar Git como herramienta profesional
*   A integrar diversas tareas en una solución global

***

## 11. Conclusiones finales

La solución propuesta para FoodLogístic S.A.:

*  Es técnicamente sólida
*  Cumple con la legislación vigente
*  Está bien documentada
*  Es viable para una PYME real
*  Demuestra competencias profesionales reales

Este proyecto refleja un escenario muy cercano al mundo laboral del sector IT.

