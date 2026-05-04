# P01 – MEMORIA TÉCNICA DEL PROYECTO

## Proyecto Intermodular SMX2

### Propuesta tecnológica para **FoodLogístic S.A.**

**Autores:**  
David Santiago  
Santiago Moreno

***

## 1. Introducción

Este documento recoge la **memoria técnica completa del proyecto FoodLogístic S.A.**, desarrollado dentro del módulo de **Proyecto Intermodular** del ciclo formativo SMX2.

El proyecto simula un **caso real de empresa**, donde se nos encarga analizar, diseñar y documentar una solución tecnológica integral que cubra:

*   Infraestructura informática
*   Seguridad y protección de datos
*   Presencia web corporativa
*   Uso de servicios en la nube
*   Planificación, presupuesto y toma de decisiones técnicas

La finalidad de esta memoria es **explicar de forma clara y estructurada**:

*   Qué se tenía que hacer
*   Qué se ha hecho realmente
*   Cómo se ha implementado
*   Con qué herramientas
*   Qué decisiones se tomaron y por qué
*   Qué se ha aprendido durante el proyecto

***

## 2. Análisis de necesidades del cliente

### 2.1 Contexto inicial

FoodLogístic S.A. es una empresa del sector de la **logística alimentaria**, que trabaja con:

*   Datos de clientes
*   Información interna
*   Empleados organizados por departamentos

Antes del proyecto, la empresa presentaba:

*   Falta de centralización IT
*   Riesgos de seguridad
*   Ausencia de documentación técnica
*   Presencia web inexistente o incompleta
*   Incumplimiento potencial de normativas legales

***

### 2.2 Necesidades detectadas

| Área      | Necesidad                      |
| --------- | ------------------------------ |
| Usuarios  | Gestión centralizada           |
| Datos     | Acceso controlado por perfiles |
| Impresión | Sistema compartido y eficiente |
| Seguridad | Cumplimiento RGPD y LOPDGDD    |
| Formación | Concienciación de empleados    |
| Web       | Imagen corporativa y legal     |
| Gestión   | Planificación y presupuesto    |

***

## 3. Propuesta de solución global

Se propone una solución **integral y realista**, dividida en tareas técnicas claramente diferenciadas pero interconectadas.

| Bloque           | Tareas        |
| ---------------- | ------------- |
| Infraestructura  | T01, T03, T04 |
| Web corporativa  | T02, T08, P02 |
| Seguridad y LOPD | T05           |
| Cloud            | T07           |
| Gestión          | T09, T12      |

***

## 4. Infraestructura técnica (T01, T03, T04)

### 4.1 Objetivo

Crear una infraestructura **centralizada, segura y escalable** basada en Windows Server.

***

### 4.2 Active Directory (T01)

**Qué se tenía que hacer**

*   Centralizar usuarios y equipos
*   Organizar la empresa por departamentos

**Cómo se hizo**

*   Instalación de Windows Server
*   Promoción a Controlador de Dominio
*   Creación de Unidades Organizativas (OU)
*   Alta de usuarios por perfiles

**Qué se aprendió**

*   Diseño lógico de dominios
*   Importancia de la jerarquía del AD
*   Gestión realista de usuarios en empresa

***

### 4.3 Servidor de ficheros (T03)

**Objetivo**
Garantizar un acceso seguro a la información.

**Implementación**

*   Carpetas por departamento
*   Permisos NTFS diferenciados
*   Acceso exclusivo según rol

| Departamento   | Acceso              |
| -------------- | ------------------- |
| Administración | Lectura / Escritura |
| Logística      | Lectura / Escritura |
| RRHH           | Acceso restringido  |

**Aprendizaje**

*   Gestión avanzada de permisos
*   Riesgos de mala asignación de accesos

***

### 4.4 Servidor de impresión (T04)

**Qué se hizo**

*   Instalación de rol de impresión
*   Printer pooling
*   Distribución mediante GPO

**Beneficio**

*   Ahorro de recursos
*   Mantenimiento centralizado

***

## 5. Web corporativa (T02, T08, P02)

### 5.1 Web individual (T02)

Cada miembro del grupo desarrolló una **propuesta web individual**, publicada mediante GitHub Pages.

*   Web T02:  
    <https://aludavidsantiago.github.io/foodlogistic-web/>
*   Repositorio:  
    <https://github.com/aluDavidSantiago/foodlogistic-web>

**Aprendizajes**

*   Estructura HTML
*   Diseño responsivo
*   Publicación web real

***

### 5.2 Comparativa de webs (T08)

Se compararon **dos propuestas (Web A y Web B)** para decidir una web final.

**Criterios analizados**

*   Diseño visual
*   Contenido informativo
*   Experiencia de usuario
*   Imagen profesional
*   Aspectos legales

**Decisión final**
Se opta por una **web combinada**, integrando:

*   Diseño visual atractivo (Web A)
*   Contenido claro y completo (Web B)

Esto permitió una solución **equilibrada y profesional**.

***

### 5.3 Web final – P02

**Web oficial del proyecto**

*   <https://classessmx2n.github.io/web-projecte7-aluDavidSantiago/>

**Repositorio**

*   <https://github.com/classesSMX2n/web-projecte7-aluDavidSantiago>

Incluye:

*   Página principal
*   Secciones informativas
*   Aviso legal
*   Política de privacidad
*   Política de cookies
*   Vídeos formativos RGPD

***

## 6. Seguridad y LOPD (T05)

### 6.1 Vídeos formativos

Se desarrolló un **vídeo formativo sobre LOPD/RGPD para empleados**, explicando:

*   Uso correcto de datos
*   Riesgos de malas prácticas
*   Responsabilidades legales

El vídeo se integró directamente en la web corporativa.

**Aprendizaje**

*   La seguridad no es solo técnica
*   Importancia de concienciar al personal

***

## 7. Servicios en la nube – Migración (T07)

Se realizó una **presentación técnica** sobre la **migración del correo corporativo a la nube**.

**Contenido**

*   Justificación de la migración
*   Ventajas del cloud
*   Seguridad y disponibilidad
*   Comparación con sistema local

**Aprendizaje**

*   Evaluación de servicios cloud
*   Argumentación técnica ante cliente

***

## 8. Planificación del proyecto (T09)

Se elaboró un **diagrama de Gantt** con:

*   Fases del proyecto
*   Dependencias
*   Cronograma realista

Esto permitió:

*   Mejor organización
*   Identificación de riesgos
*   Visión global del proyecto

***

## 9. Presupuesto y viabilidad (T12)

Se realizó un estudio de **presupuesto y viabilidad**, justificando:

*   Costes técnicos
*   Recursos humanos
*   Enfoque realista para una PYME

**Conclusión**
La solución es **económicamente viable** gracias al uso de:

*   Software estándar
*   Servicios en la nube
*   Infraestructura optimizada

***

## 10. Reparto de trabajo y aportación individual

Cada miembro del equipo participó activamente en:

*   Infraestructura
*   Web
*   Seguridad
*   Documentación
*   Presentaciones
*   Decisiones técnicas

Se trabajó de forma coordinada, simulando un **entorno profesional real**.

***

## 11. Aprendizajes globales

Durante el proyecto se adquirieron competencias clave:

*   Diseño de infraestructuras reales
*   Documentación técnica profesional
*   Trabajo en equipo
*   Pensamiento crítico
*   Toma de decisiones justificadas
*   Uso de Git y GitHub

***

## 12. Conclusiones finales

El proyecto FoodLogístic S.A. demuestra:

✅ Capacidad técnica  
✅ Capacidad organizativa  
✅ Cumplimiento legal  
✅ Visión empresarial  
✅ Preparación para el mundo laboral

La solución propuesta es **completa, realista y bien documentada**, cumpliendo los objetivos del Proyecto Intermodular.


