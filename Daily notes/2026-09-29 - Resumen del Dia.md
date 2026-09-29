---
date: 2026-09-29
aliases: [resumen-2026-09-29]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-09-29

> [!warning] Decimoctava vez consecutiva que la rutina se dispara antes de medianoche Guatemala
> Al momento del pull (2026-09-29 05:50 UTC = **2026-09-28 23:50 hora de Guatemala, GMT-6**), el día calendario 2026-09-29 **todavía no ha comenzado** en la zona horaria de la cuenta Meta Ads. La métrica `date_preset=today` de la API corresponde en realidad a **2026-09-28** (a ~10 min de su cierre real, aún sujeta a la ventana de atribución de leads). Esta nota documenta esa lectura casi-final de 2026-09-28. Se confirmó vía `list_triggers` que el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") sigue en `50 5 * * *` UTC (23:50 GT), sin cambios desde su creación el 2026-08-28 — 18ª ocurrencia consecutiva documentada. No se reintentó la corrección esta sesión: solo el usuario puede editarlo desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ.

---

## 🎯 Campañas Revisadas

Lectura casi-final de **2026-09-28** (a ~10 minutos del cierre real, sujeta aún a cambios por ventana de atribución de leads):

| Campaña | Status | Gasto | Presupuesto/día | % Presup. | Leads | CPL | CTR | Emoji |
|---------|--------|-------|------------------|-----------|-------|-----|-----|-------|
| Toma El control de tu pyme (GT) | ACTIVE | $13.30 | N/D (a nivel ad set) | - | 3 | $4.43 🟢 | 1.76% 🟡 | 🟢 |
| Pyme Colombia (COL) | ACTIVE | $9.22 | $7.50 | 122.9% | 2 | $4.61 🟢 | 2.04% 🟡 | 🟢 |
| Pyme El Salvador (SV) | ACTIVE | $9.52 | $12.50 | 76.2% | 1 | $9.52 🟡 | 1.31% 🔴 | 🟡 |
| Beco (GT) | ACTIVE | $9.20 | $10.00 | 92.0% | 0 | N/D 🔴 | 0.90% 🔴 | 🔴 |
| Odoo Test (GT) | ACTIVE | $5.14 | $4.93 | 104.3% | 0 | N/D 🔴 | 0.98% 🔴 | 🔴 |
| Toma El control de tu pyme (USA) | PAUSED | $0.00 | - | - | - | - | - | ⏸️ |
| Accurate Partners - Loyalti | PAUSED | $0.00 | - | - | - | - | - | ⏸️ |
| Conversión Clientes Potenciales - MX | PAUSED | $0.00 | - | - | - | - | - | ⏸️ |
| Conversión Clientes Potenciales - PY | PAUSED | $0.00 | - | - | - | - | - | ⏸️ |
| 🟡 CONVERSIÓN - CLIENTES POTENCIALES | PAUSED | $0.00 | - | - | - | - | - | ⏸️ |

**Sin cambios manuales detectados hoy:** el activity log de la cuenta para la ventana 2026-09-28 00:00–2026-09-29 05:52 UTC solo registra un evento automático de **facturación de Meta** ("Account billed", 9/28 4:16 AM, actor "Meta") — ninguna acción manual sobre presupuesto, targeting, creativo o estado de campañas.

### 🔴 Beco y Odoo Test colapsan de vuelta a cero leads — tercer/cuarto giro abrupto documentado en ambas

Ayer (2026-09-27 confirmado) Beco fue el **mejor performer de toda la cuenta** (4 leads, $3.02 CPL) y Odoo Test rompió su racha de ceros (2 leads, $3.20 CPL). Hoy ambas cierran casi-final en **0 leads**, pese a gastar $9.20 y $5.14 respectivamente, sin ningún cambio manual registrado en el activity log. Confirma la hipótesis ya anotada en cierres previos: el patrón de saltos abruptos en estas dos campañas parece ser volatilidad normal de subasta/audiencia en cuenta de bajo volumen, no un problema estructural de creativo — pero ahora con una tercera y cuarta muestra respectivamente, el patrón es demasiado consistente para ignorar y merece revisión dedicada.

### 🟢 Toma El control de tu pyme (GT) es hoy el mejor performer de la cuenta

Sube a $4.43 CPL (mejor cierre documentado de esta campaña hasta ahora) manteniendo 3 leads, con gasto -25.5% vs. ayer ($17.85 → $13.30) — mejora de eficiencia, no de volumen de inversión. Sigue siendo la campaña con mayor alcance/impresiones de la cuenta, y su CTR (1.76%) mejora vs. ayer (1.05%) aunque sigue bajo la meta 3-4%.

### 🟢 Pyme Colombia se mantiene estable dentro de meta

2 leads a $4.61 CPL (vs. $4.84 ayer, -4.8%) — tercera lectura consecutiva positiva para el creativo "Urgencia", cada vez con más confianza estadística aunque el volumen sigue siendo bajo.

### 🟡 Pyme El Salvador mejora pero sigue siendo la más cara de la cuenta

CPL baja de $15.29 a $9.52 (-37.7%) — mejor cierre documentado de esta campaña, y por primera vez en varios días **no es la peor performer de la cuenta** (ese lugar lo toman hoy Beco y Odoo Test con 0 leads). Aun así, entre las campañas con al menos 1 lead, sigue siendo la más cara.

---

## 📊 Análisis e Insights

- **El CPL blendeado de la cuenta sube a $7.74 (+51.5% vs. el $5.11 confirmado de ayer)** — vuelve a estar fuera (por encima) de la meta $6-7, revirtiendo el mejor cierre documentado del proyecto.
- **Los leads confirmados caen a la mitad: de 12 a 6 (-50.0%) con un gasto que baja -24.4%** ($61.37 → $46.41) — el retroceso es casi enteramente de conversión a lead (Beco y Odoo Test a cero), no de menor inversión relativa.
- **CTR blendeado baja a 1.34% (-14.6% vs. ayer) y se mantiene por debajo de la meta 3-4%.**
- **CPC blendeado sube a $0.46 (+9.5% vs. ayer $0.42); CPM baja ligeramente a $6.15 (-6.1% vs. $6.55).**
- **3 de 5 campañas activas cierran con al menos 1 lead** (vs. 5 de 5 ayer) — Beco y Odoo Test son las únicas en cero hoy.
- **Un único evento en el activity log hoy, de tipo automático (facturación), sin cambios manuales** — igual que los cierres previos, el movimiento de métricas no está asociado a ninguna acción operativa visible de usuario ni de esta rutina.
- El retroceso simultáneo de Beco y Odoo Test — justo las dos campañas que "resucitaron" ayer — refuerza que su historial reciente es de alta volatilidad más que de una tendencia sostenida en cualquier dirección; conviene tratarlas como de riesgo/alta varianza hasta ver más cierres.
- Dado que esta es una lectura casi-final tomada minutos antes del cierre, la ventana de atribución de leads podría sumar (o restar) resultados adicionales en las próximas horas. Confirmar con el Reporte Performance formal (~7 AM GT).

> [!caution] No confirmar como cierre real
> Estas cifras corresponden a una lectura tomada ~10 minutos antes del cierre real de 2026-09-28 y pueden moverse al resolverse la ventana de atribución de leads. Confirmar con el Reporte Performance formal cuando esté disponible (~7 AM GT).

---

## ✏️ Cambios Realizados

- **Ningún cambio fue realizado por esta sesión.** Esta rutina automatizada solo leyó métricas y el activity log; no modificó presupuestos, targeting, copy ni estado de campañas.
- **Ningún cambio manual detectado en la cuenta hoy** — el activity log de la ventana 2026-09-28 00:00–2026-09-29 05:52 UTC solo contiene un evento automático de facturación de Meta.
- **El A/B testing de los 5 copys mejorados documentado en [[CLAUDE.md]] sigue sin iniciarse formalmente** en "Toma El control de tu pyme" (GT) — ninguna tarea de la lista de "Tareas Activas" del proyecto se marcó como completada hoy.
- **Ningún cambio de infraestructura intentado hoy** (no se reintentó reprogramar el trigger con el bug de zona horaria; ver advertencia arriba).

---

## 🔬 Investigación Realizada

- Se revisaron las 5 campañas activas de la cuenta a nivel campaña con `date_preset=today` (equivalente a 2026-09-28 en horario de cuenta), incluyendo gasto, leads (derivados de `cost_per_lead`), CTR, CPC, CPM, alcance, clicks y presupuesto diario configurado.
- Se revisó el total de cuenta a nivel `ad_account` para contrastar contra la suma de campañas: gasto cuadra ($46.41 vs. $46.38 sumado), CPL blendeado cuadra ($7.74, ≈6 leads implícitos en ambos casos); el alcance total de cuenta (5,682) es menor que la suma simple por campaña (6,059) por solape normal de audiencias entre campañas.
- Se revisó el activity log completo de la cuenta para la ventana 2026-09-28 00:00–2026-09-29 05:52 UTC: un único evento automático de facturación ("Account billed"), sin cambios manuales.
- Se confirmó el estado de los dos triggers automatizados de la cuenta vía `list_triggers`: "Daily Summary - 11:50 PM Guatemala" (`trig_01DMJfrsQXaTY5KJntXisDPQ`) sigue en `50 5 * * *` UTC sin cambios desde su creación el 2026-08-28 — 18ª ocurrencia consecutiva del bug de zona horaria; "Daily Meta Ads Performance Report - 7 AM Guatemala" (`trig_015F5ZAcF8dpKuJLH6NreZnt`) corrió exitosamente ayer (2026-09-28 13:22 UTC) generando el reporte confirmado de 2026-09-27.
- No se realizó investigación externa de competencia ni tendencias de mercado en esta sesión.

---

## 📊 Datos Clave del Día

| Métrica (5 campañas activas) | 2026-09-28 (casi-final) | 2026-09-27 (confirmado) | Variación |
|---------|---------------------------|----------------------------------|-----------|
| Gasto Total | $46.41 | $61.37 | 🔻 -24.4% |
| Leads Confirmados | 6 | 12 | 🔴 -50.0% |
| CPL Promedio (blendeado) | **$7.74** | $5.11 | 🔴 +51.5% |
| CTR Promedio (blendeado) | 1.34% | 1.57% | 🔴 -14.6% |
| CPC Promedio | $0.46 | $0.42 | 🔴 +9.5% |
| CPM Promedio | $6.15 | $6.55 | 🟢 -6.1% |
| Impresiones | 7,550 | 9,367 | 🔻 -19.4% |
| Clicks | 101 | 147 | 🔻 -31.3% |
| Alcance (Reach) | 5,682 | 7,086 | 🔻 -19.8% |
| Mejor CPL del día | Toma El control (GT): **$4.43** | Beco (GT): $3.02 | Cambio de líder |
| Peor performer del día | Beco y Odoo Test: $0 leads (empate) | Pyme El Salvador: $15.29 CPL (único fuera de meta) | Beco y Odoo Test caen de mejores a peores |

**Detalle por campaña:**
- Toma El control de tu pyme (GT): $13.30 / 3 leads / $4.43 CPL
- Pyme Colombia (COL): $9.22 / 2 leads / $4.61 CPL
- Pyme El Salvador (SV): $9.52 / 1 lead / $9.52 CPL
- Beco (GT): $9.20 / 0 leads
- Odoo Test (GT): $5.14 / 0 leads

---

## 📋 Próximas Acciones

- [ ] Confirmar mañana (~7 AM GT) el cierre real de 2026-09-28 vía Reporte Performance — prioritario dado que la lectura casi-final muestra un retroceso marcado del CPL blendeado (+51.5% vs. el mejor cierre documentado) y caída de leads a la mitad
- [ ] Investigar a fondo el patrón de Beco y Odoo Test: ambas pasaron de mejor performer/rompiendo racha de ceros ayer a cero leads hoy, sin cambio manual registrado — con ya 3-4 giros abruptos documentados entre las dos, evaluar si vale la pena una revisión de creativo/targeting específica antes de seguir asumiendo "volatilidad normal"
- [ ] Dar seguimiento a Pyme El Salvador: mejora fuerte hoy (-37.7% CPL) pero sigue siendo la más cara entre las campañas con leads — confirmar si la mejora se sostiene en el próximo cierre
- [ ] Retomar el A/B testing pendiente de los 5 nuevos copys en "Toma El control de tu pyme" (GT), documentado en [[CLAUDE.md]] pero aún sin iniciar formalmente — sigue pendiente tras múltiples cierres consecutivos
- [ ] Revisar `daily_budget` de las campañas que cierran fuera de rango: Odoo Test (104.3%) y Pyme Colombia (122.9%) sobre presupuesto; Pyme El Salvador (76.2%) y Beco (92.0%) por debajo
- [ ] **Usuario:** el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` sigue disparándose a las 23:50 GT en vez de después de medianoche (18ª ocurrencia consecutiva sin resolver) — solo se puede corregir manualmente desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ, ningún agente automatizado tiene permiso para editarlo

---

## 🔗 Enlaces

- [[Reports/2026-09-27 - Reporte Performance]] — último reporte de cierre confirmado disponible (el de 2026-09-28 se genera mañana ~7 AM GT)
- [[Daily notes/2026-09-28 - Resumen del Dia]] — resumen del día anterior
- Tags: #daily-note #summary #meta-ads #octopus
