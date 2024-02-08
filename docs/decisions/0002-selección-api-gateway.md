# Selección-API-Gateway

* Status: accepted
* Deciders: Manuel López Corchado y Víctor Candel Casado
* Date: 2024-02-08

## Context and Problem Statement

Es necesario implementar un componente API Gateway en el sistema.

## Decision Drivers

* RF3 : El sistema tendrá un componente API Gateway que hará de intermediario entre el cliente y el sistema mediante conexiones HTTP/REST.

## Considered Options

* KONG Gateway
* APISIX

## Decision Outcome

Chosen option: "APISIX", because tiene un mejor rendimiento

### Positive Consequences

* Buen rendimiento con latencia mínima.
* Altamente escalable.
* Menos vulnerabilidad debido a una alta seguridad en la autentificación.

### Negative Consequences

* Complejidad de configuración.
