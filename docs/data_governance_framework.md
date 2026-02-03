# Marco Mínimo de Data Governance
**Curso de Data Governance**

## 1. Qué es Data Governance (en práctica)
Es el conjunto de **roles, reglas y controles** que aseguran que los datos:
- Sean entendibles
- Sean confiables
- Sean usados correctamente
- No generen riesgo innecesario

No es burocracia. Es habilitador.

## 2. Roles clave

### Data Owner
- Responsable del significado y uso del dato
- Define reglas de negocio
- Aprueba acceso y cambios relevantes

### Data Steward
- Traduce negocio a metadata
- Define reglas de calidad
- Monitorea cumplimiento

### Data Custodian
- Opera la plataforma
- Implementa controles técnicos
- Garantiza disponibilidad y seguridad

## 3. Dimensiones de calidad de datos

| Dimensión | Pregunta clave |
|---|---|
| Exactitud | ¿El dato es correcto? |
| Completitud | ¿Faltan valores? |
| Consistencia | ¿Coincide entre sistemas? |
| Unicidad | ¿Está duplicado? |
| Oportunidad | ¿Llega a tiempo? |
| Validez | ¿Respeta el dominio esperado? |

## 4. Reglas de calidad (ejemplos)
- `% nulos < 1%`
- `fecha <= hoy`
- `email cumple regex`
- `monto >= 0`
- `id único`

Las reglas deben ser **medibles y monitoreables**.

## 5. Lineage (linaje)
Documenta:
- Origen del dato
- Transformaciones relevantes
- Sistemas consumidores
- Uso principal

No requiere tooling complejo para empezar. Puede ser descriptivo.

## 6. Controles mínimos de gobierno
- Diccionario de datos vivo
- Ownership explícito
- Clasificación de sensibilidad
- Reglas de calidad básicas
- Lineage a alto nivel
- Accesos definidos por rol

## 7. Principios
- Gobernar lo crítico primero
- Menos reglas, mejor cumplidas
- Governance by design, no post-hoc
