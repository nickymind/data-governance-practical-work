# PII & Data Sensitivity Taxonomy
**Curso de Data Governance**

## 1. Propósito
Establecer un marco claro y operativo para clasificar datos según su sensibilidad, identificar PII y definir **controles mínimos**. Este documento no es legal, es de **gobierno del dato**.

## 2. Clasificación de sensibilidad

### 2.1 No-PII
Datos que no identifican directa ni indirectamente a una persona física.

**Ejemplos**
- IDs técnicos no reversibles
- Métricas agregadas
- Códigos de producto
- Fechas de proceso
- Flags operativos

**Riesgo**
Bajo.

### 2.2 PII (Personally Identifiable Information)
Datos que identifican o pueden identificar razonablemente a una persona física.

**Ejemplos**
- Nombre y apellido
- Email
- Teléfono
- Dirección
- Documento de identidad
- Fecha de nacimiento
- IP asociada a individuo

**Riesgo**
Medio.

### 2.3 Sensitive PII (SPII)
PII cuyo uso indebido puede generar daño significativo.

**Ejemplos**
- Datos financieros individuales
- Credenciales
- Datos biométricos
- Información de salud
- Información crediticia detallada
- Geolocalización precisa

**Riesgo**
Alto.

## 3. Tipos de PII (clasificación granular)

| Tipo | Ejemplos |
|---|---|
| Identidad | Nombre, DNI, pasaporte |
| Contacto | Email, teléfono, dirección |
| Financiero | Cuenta, saldo, transacción |
| Credenciales | Usuario, password, token |
| Biometría | Huella, rostro |
| Digital | IP, device ID |
| Salud | Diagnóstico, cobertura |

## 4. Controles mínimos por nivel

### No-PII
- Control de calidad
- Control de cambios de schema
- Lineage documentado

### PII
- Control de acceso por rol
- Enmascaramiento en ambientes no productivos
- Trazabilidad de uso
- Retención definida

### Sensitive PII
- Acceso restringido y auditado
- Encriptación en reposo y tránsito
- Minimización de uso
- Revisión periódica de necesidad
- Registro de accesos

## 5. Principios clave
- La clasificación se basa en **uso y contexto**, no solo en el nombre del campo.
- La duda implica **clasificación conservadora**.
- La clasificación se revisa cuando cambia el uso del dato.
