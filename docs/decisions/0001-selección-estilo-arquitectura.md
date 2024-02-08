# Selección-Estilo-Arquitectura

* Status: proposed
* Deciders: Manuel López Corchado y Víctor Candel Casado
* Date: 2024-02-08

## Context and Problem Statement

Se necesita una arquitectura basada en microservicios y compatible con la aplicación web, tendrá que ser modular y escalable, y deberá permtir gestionar los clientes, pedidos, repartos, rutas, estadísticas, incidencias y pagos.

## Decision Drivers

* RF1: Migrar la arquitectura monolítica a una basada en microservicios. Este requisito es el objetivo principal del proyecto y afecta a todos los demás componentes del sistema.
* RF4: Realizar pedidos de los productos. Este componente permitirá a los clientes realizar pedidos de los productos disponibles
* RF5: Gestionar el reparto y las rutas de los camiones. Este componente se encargará de asignar los pedidos a las flotas de transporte, calcular las rutas óptimas de los camiones.
* RF6: Proporcionar estadísticas sobre el estado de los pedidos y los camiones. Este componente proporcionará información valiosa sobre el estado de los pedidos y la situación en tiempo real de los camiones.
* RF7: Reportar incidencias en el reparto. Este componente permitirá reportar a los gestores de las rutas cualquier tipo de incidencia que ocurra durante el reparto.
* RF8: Realizar pagos mediante una pasarela externa. Este componente se integrará con una pasarela de pago externa que proporcionará otra empresa.
* RF9: Conectarse a bases de datos para consultar la distinta información.

## Considered Options

* Arquitectura cliente servidor modelo de 3 capas con microservicios en capa servidor.
* Arquitectura orientada a servicios.
* Arquitectura basada en eventos.

## Decision Outcome

Chosen option: "Arquitectura cliente servidor modelo de 3 capas con microservicios en capa servidor", because según los requisitos y la naturaleza del problema consideramos que es la que mejor encaja.

### Positive Consequences

* Mayor modularidad de los componentes del sistema.
* Mayor escalabilidad en el sistema.
* Mejor fiabilidad por independencia del funcionamiento de los microservicios.

### Negative Consequences

* Mayor complejidad al gestionar varios servicios.
* Costes de implementación y mantenimiento.
* Riesgo de caída del sistema
