# BIAN – Reference Light
**Uso preferido en el curso**

## 1. Qué es BIAN
BIAN (Banking Industry Architecture Network) es un **marco semántico** para modelar capacidades, dominios y objetos de negocio en banca.

En este curso se usa como:
- Marco de referencia preferido
- Lenguaje común
- Herramienta de orden conceptual

No es obligatorio ni exhaustivo.

## 2. Conceptos clave

### Service Domain
Área funcional del negocio bancario que ofrece capacidades específicas.

### Business Object
Entidad de negocio gestionada dentro de un Service Domain.

## 3. Service Domains frecuentes (nivel alto)

| Service Domain | Descripción |
|---|---|
| Customer Management | Gestión del cliente |
| Account Management | Gestión de cuentas |
| Transaction Processing | Movimientos y pagos |
| Product Management | Productos financieros |
| Party Data Management | Datos maestros de personas |
| Credit Management | Préstamos y riesgo |
| Compliance | Controles regulatorios |

## 4. Business Objects típicos

| Business Object | Descripción |
|---|---|
| Customer | Persona o empresa |
| Account | Cuenta bancaria |
| Transaction | Movimiento financiero |
| Product | Producto financiero |
| Agreement | Contrato |
| Party | Individuo u organización |

## 5. Ejemplo de mapeo
Campo: `account_balance`

- Service Domain: Account Management
- Business Object: Account
- Contexto: Core bancario
- Sensibilidad: Sensitive PII
- Uso típico: Reporting financiero, atención al cliente

## 6. Uso didáctico en el curso
- Si el dataset es bancario, intentar mapeo BIAN.
- Si no aplica, usar abstracción equivalente:
  - Cliente
  - Producto
  - Evento
  - Transacción

Siempre con nivel de confianza explícito.

## 7. Regla de oro
BIAN **ordena el pensamiento**, no reemplaza el criterio.
