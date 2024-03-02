# Patrón-de-notificaciones

* Status: accepted
* Deciders: Manuel López Corchado y Victor Candel Casado
* Date: 2024-03-02

## Context and Problem Statement

Es necesaria la implementación de un patrón para mandar las notificaciones de actualización de pedidos.

## Decision Drivers

* RF-5.2

## Considered Options

* PubSub
* Observer

## Decision Outcome

Chosen option: "PubSub", because por su orientación a notificaciones particulares y mayor escalabilidad

### Positive Consequences

* Descacoplamiento
* Escalabilidad
* Flexibilidad de suscripción

### Negative Consequences

* Complejidad de implementación
* Dificultad para depurar mensajes
