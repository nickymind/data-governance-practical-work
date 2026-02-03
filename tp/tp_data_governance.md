# Trabajo Práctico – Data Governance aplicado a datasets transaccionales

**Materia:** Data Governance  
**Modalidad:** Individual o grupos de hasta 3  
**Entrega:** PDF + anexos (JSON/CSV)  
**Herramienta permitida:** GPT custom “DG Copilot (BIAN + PII)”

---

## 1. Objetivo del TP

Aplicar principios de **Data Governance** para:
- Comprender un dataset realista.
- Definir **metadata de negocio**.
- Clasificar **sensibilidad y PII**.
- Proponer **reglas de calidad**.
- Diseñar **controles mínimos** de gobierno.
- Justificar decisiones con criterio profesional.

No se evalúa volumen. Se evalúa **calidad del razonamiento**.

---

## 2. Dataset

Se provee el archivo:

`datasets/customer_transactions_sample.csv`

---

## 3. Consigna

A partir del dataset, desarrollar un **informe de Data Governance** que incluya:

### A) Contexto y uso (máx. 1 página)
- ¿Qué tipo de información contiene el dataset?
- ¿Cuáles podrían ser **2–3 casos de uso** razonables?
- ¿Qué **riesgos principales** presenta el uso indebido del dato?

### B) Metadata de negocio (obligatorio)
Construir un **diccionario de datos a nivel campo**, que incluya como mínimo:
- Nombre técnico del campo
- Nombre de negocio
- Definición clara
- Tipo de dato inferido
- Dominio / valores permitidos
- Ejemplos (enmascarados si aplica)

Debe quedar claro que una persona **no técnica** podría entender el dataset.

### C) Sensibilidad, PII y riesgo
Para cada campo:
- Clasificar como **No-PII / PII / Sensitive PII**.
- Indicar **tipo de PII** cuando aplique.
- Justificar brevemente la clasificación.

### D) BIAN como marco preferido
- Intentar mapear el dataset a:
  - **Service Domain**
  - **Business Object**
- Si no aplica claramente, justificar por qué y proponer una abstracción equivalente.
- Incluir **nivel de confianza** (alto / medio / bajo).

### E) Calidad de datos
Definir **al menos 10 reglas de calidad**, incluyendo:
- Claves (unicidad / no nulos)
- Dominios (enum, patrones)
- Reglas de consistencia (entre campos)
- Reglas de plausibilidad (fechas, montos)

Las reglas deben ser **medibles**.

### F) Controles mínimos de Data Governance
Proponer controles concretos para:
- Acceso
- Privacidad
- Calidad
- Retención
- Trazabilidad / linaje

No políticas extensas. **Controles aplicables**.

### G) Reflexión crítica (clave)
Responder brevemente:
- ¿Qué información faltante limita la calidad del gobierno del dato?
- ¿Qué decisión de clasificación fue más discutible y por qué?
- ¿Qué cambiaría si el caso de uso fuera **fraude en tiempo real**?

---

## 4. Uso del GPT

Está **permitido y recomendado** usar el GPT del curso.

Condición:
- El output del GPT **no se entrega tal cual**.
- Debe haber **criterio propio**, ajustes y justificación.
- Se penaliza copiar sin análisis.

---

## 5. Entregables

1. **Informe PDF** (10–15 páginas máximo).
2. **Anexo JSON** con la metadata estructurada (exportable a catálogo).
3. (Opcional) CSV con reglas de calidad.

---

## 6. Rúbrica de evaluación (100 puntos)

| Dimensión | Puntaje |
|---------|--------|
| Comprensión del dataset y casos de uso | 15 |
| Calidad de metadata de negocio | 20 |
| Clasificación PII y riesgo | 15 |
| Uso razonado de BIAN | 10 |
| Reglas de calidad (claras y medibles) | 20 |
| Controles de governance | 10 |
| Reflexión crítica y criterio profesional | 10 |

---

## 7. Criterios de desaprobación directa
- Definiciones vagas o genéricas.
- Clasificar todo como PII sin justificación.
- Reglas de calidad no medibles.
- Copiar output del GPT sin intervención humana.
- No distinguir hechos de supuestos.

---

## 8. Nivel esperado
Este TP apunta a un **perfil semi-senior**:
- No se espera perfección.
- Sí se espera **criterio, trade-offs y claridad conceptual**.
