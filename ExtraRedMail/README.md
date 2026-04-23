
# Servidor de correo con iRedMail en Ubuntu Server

Guía técnica de la práctica de configuración de un servidor de correo electrónico utilizando **iRedMail** sobre **Ubuntu Server**, incluyendo la gestión de dominios, usuarios, envío y recepción de correos y análisis de logs.

---

## Información del alumno

- **Nombre:** Santiago Hernández  
- **Número de lista:** 10  
- **Centro:** Escola Pia Santa Anna – Mataró  
- **Ciclo:** ASIX / CFGS  
- **Sistema operativo:** Ubuntu Server  
- **Software principal:** iRedMail 1.8.0  

---

## Objetivo de la práctica

El objetivo de esta práctica es desplegar y configurar un servidor de correo totalmente funcional, capaz de:

- Gestionar dominios de correo
- Crear y administrar usuarios
- Enviar y recibir correos internos
- Enviar correos a direcciones externas
- Analizar el comportamiento del correo en servicios externos (Gmail)
- Consultar y revisar los logs del sistema

---

## Contenido del repositorio

Este repositorio contiene la documentación completa del proceso realizado durante la práctica.

- ✅ Configuración inicial del sistema
- ✅ Instalación y configuración de iRedMail
- ✅ Acceso y uso del panel iRedAdmin
- ✅ Gestión de dominios y usuarios
- ✅ Uso de Roundcube (webmail)
- ✅ Envío de correos internos y externos
- ✅ Creación de un segundo dominio
- ✅ Revisión de logs de actividad
- ✅ Análisis del correo clasificado como spam

---

## Tecnologías y herramientas utilizadas

- **Sistema operativo:** Ubuntu Server
- **Servidor de correo:** iRedMail
- **Servidor web:** Nginx
- **Base de datos:** MariaDB
- **Webmail:** Roundcube
- **Panel de administración:** iRedAdmin
- **Seguridad:** Fail2ban, nftables
- **Monitorización:** Netdata
- **Virtualización:** VirtualBox

---

## Dominios y usuarios configurados

### Dominio principal
- `tucat.test`
  - `postmaster@tucat.test`
  - `tucatito10@tucat.test`

### Segundo dominio
- `alumno10.test`
  - `alumnito10@alumno10.test`

---

## Resultados obtenidos

- El servidor de correo funciona correctamente para envío y recepción interna.
- El correo entre dominios configurados en el mismo servidor se entrega sin problemas.
- Los correos enviados a Gmail llegan correctamente pero se clasifican como spam.
- El motivo principal es la ausencia de registros DNS reales (SPF, DKIM, DMARC) y el uso de dominios `.test`.
- El sistema registra todas las acciones en los logs de administración.

---

## Estructura de la documentación

La guía técnica incluida en este repositorio sigue una estructura clara por fases:

1. Preparación del entorno
2. Instalación de iRedMail
3. Configuración inicial
4. Administración del servidor
5. Creación de usuarios
6. Uso de webmail
7. Envío de correos externos
8. Segundo dominio
9. Logs y auditoría
10. Conclusiones

Cada fase incluye comandos utilizados, validaciones realizadas y capturas de pantalla del proceso.

---

## Conclusión

Esta práctica permite comprender el funcionamiento real de un servidor de correo, tanto a nivel de instalación como de administración. También pone de manifiesto la importancia de la configuración DNS y la reputación de un dominio para evitar la clasificación como correo no deseado en servicios externos.

El servidor queda correctamente configurado y preparado para ampliaciones futuras en un entorno real.

---

## Estado del proyecto

✅ Práctica finalizada  
✅ Funcional y documentada  
✅ Lista para entrega académica
