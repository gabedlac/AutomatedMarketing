---
date: 2026-09-26
aliases: [resumen-2026-09-26]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-09-26

> [!warning] Decimoquinta vez consecutiva que la rutina se dispara antes de medianoche Guatemala
> Al momento del pull (2026-09-26 05:51 UTC = **2026-09-25 23:51 hora de Guatemala, GMT-6**), el día calendario 2026-09-26 **todavía no ha comenzado** en la zona horaria de la cuenta Meta Ads. La métrica `date_preset=today` de la API corresponde en realidad a **2026-09-25** (a ~9 min de su cierre real, aún sujeta a la ventana de atribución de leads). Esta nota documenta esa lectura casi-final de 2026-09-25. Se confirmó vía `list_triggers` que el cron del trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` sigue en `50 5 * * *` UTC (23:50 GT), sin cambios desde su creación el 2026-08-28 — 15ª ocurrencia consecutiva documentada. No se reintentó la corrección esta sesión, dado que un intento anterior fue rechazado por el sistema (el trigger no fue creado por un agente; solo el usuario puede editarlo desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ).

---

## 🎯 Campañas Revisadas

Lectura casi-final de **2026-09-25** (a ~9 minutos del cierre real, sujeta aún a cambios por ventana de atribución de leads):

| Campaña | Status | Gasto | Presupuesto/día | Leads | CPL | CTR | Emoji |
|---------|--------|-------|------------------|-------|-----|-----|-------|
| Toma El control de tu pyme (GT) | ACTIVE | $14.21 | N/D (a nivel ad set) | 4 | **$3.55** 🟢 | 1.74% 🟡 | 🟢 |
| Beco (GT) | ACTIVE | $10.77 | $10.00 (107.7%) | 3 | $3.59 🟢 | 1.48% 🟡 | 🟢 |
| Pyme El Salvador (SV) | ACTIVE | $11.79 | $12.50 (94.3%) | 0 | — 🔴 | 1.04% 🔴 | 🔴 |
| Pyme Colombia (COL) | ACTIVE | $6.09 | $7.50 (81.2%) | 1 | $6.09 🟡 | 1.80% 🟡 | 🟡 |
| Odoo Test (GT) | ACTIVE | $4.82 | $4.93 (97.8%) | 0 | — 🔴 | 1.35% 🟡 | 🔴 |
| Toma El control de tu pyme (USA) | PAUSED | $0.00 | - | - | - | - | ⏸️ |
| Accurate Partners - Loyalti | PAUSED | $0.00 | - | - | - | - | ⏸️ |
| Conversión Clientes Potenciales - MX | PAUSED | $0.00 | - | - | - | - | ⏸️ |
| Conversión Clientes Potenciales - PY | PAUSED | $0.00 | - | - | - | - | ⏸️ |
| 🟡 CONVERSIÓN - CLIENTES POTENCIALES | PAUSED | $0.00 | - | - | - | - | ⏸️ |

### 🔄 Cambio real detectado: nueva creativo de "urgencia" en Pyme Colombia

El activity log de la cuenta muestra una acción manual real hoy, no automatizada: **Gabriel Calderon reemplazó la creatividad del único anuncio activo de Pyme Colombia** ("AD Pyme Urgencia COL", ad id `120256952282780211`, dentro del ad set `120256952282790211`) vía Power Editor a las **12:18 PM GT**, pasando de la creatividad `1578260823463271` a `1413857937560440`. El anuncio pasó por revisión de Meta (Pending Process → Pending Review → Active) y quedó activo a las **12:21 PM GT**, es decir sirvió apenas ~11 horas del día.

Esto coincide con el nombre "Urgencia", en línea con los 5 copys mejorados mencionados en [[CLAUDE.md]] para atacar la falta de urgencia en el copy — aunque ese proyecto los documentaba para la campaña GT "Toma El control de tu pyme", y el cambio de hoy se aplicó en cambio a **Pyme Colombia**. Es la primera acción concreta hacia el A/B testing pendiente, aunque no configurada como test formal (A/B test tool) sino como reemplazo directo de creativo.

Con la muestra reducida (~11h de exposición), el anuncio cierra con 1 lead a $6.09 CPL y CTR 1.80% — dentro de meta pero por debajo del CTR de 2.88% que tenía Pyme Colombia ayer. Insuficiente para concluir si el nuevo copy mejora o empeora el rendimiento; requiere un día completo de datos para evaluar.

### 🔴 Pyme El Salvador y Odoo Test vuelven a cero leads — revierte el hito de ayer

Ayer (09-24) las 5 campañas activas cerraron con al menos 1 lead por primera vez en las notas recientes. Hoy esa racha se rompe: **Pyme El Salvador y Odoo Test cierran ambas en cero leads**, exactamente las dos campañas que ayer se habían "recuperado" de sus rachas negativas previas. Esto contradice la lectura optimista de ayer (que atribuía los ceros anteriores a variance de bajo volumen) y sugiere que el patrón de ceros intermitentes en ambas campañas es más recurrente/estructural de lo que parecía tras un solo día de recuperación.

### 🟢 "Toma El control de tu pyme" (GT) sigue liderando, aunque su CPL sube

$3.55 CPL con 4 leads — sigue siendo el mejor performer de la cuenta y mantiene el mismo volumen de leads que ayer, pero su CPL sube +20.3% vs. el $2.95 de ayer.

### 🟢 Beco rompe su racha de CPL fuera de meta

Por primera vez en varias notas recientes, Beco cierra **dentro** de la meta $6-7 (de hecho muy por debajo, $3.59), con 3 leads — su mejor resultado documentado hasta ahora, revirtiendo el problema de conversión post-click que se venía flagueando.

---

## 🔬 Investigación Realizada

- Se revisaron las 5 campañas activas de la cuenta a nivel campaña con `date_preset=today` (equivalente a 2026-09-25 en horario de cuenta), incluyendo gasto, leads, CPL, CTR, CPC, CPM, alcance, clicks y presupuesto diario configurado.
- Se revisó el total de cuenta a nivel `ad_account` para contrastar contra la suma de campañas: cuadra exactamente ($47.68 gasto, $5.96 CPL blendeado, 8 leads implícitos en ambos casos).
- Se revisó el activity log completo de la cuenta para la ventana 2026-09-25 00:00–2026-09-26 05:52 UTC: a diferencia de los dos días anteriores (ambos vacíos), **hoy sí hay 5 eventos registrados** — el reemplazo de creativo en Pyme Colombia (4 eventos de status/actualización del mismo anuncio) y la adición de un nuevo usuario administrador a la cuenta ("Person added to account", user id `3158599694341600`, rol "Ad account admin") a las 9:07 AM GT, ambos ejecutados por Gabriel Calderon.
- Se confirmó el estado del trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` vía `list_triggers`: cron sigue en `50 5 * * *` UTC (23:50 GT), sin cambios desde su creación el 2026-08-28. No se reintentó la corrección esta sesión.
- No se realizó investigación externa de competencia ni tendencias de mercado en esta sesión.

---

## ✏️ Cambios Realizados

- **Reemplazo de creativo en Pyme Colombia**: el anuncio "AD Pyme Urgencia COL" reemplazó su creativo activo a las 12:18 PM GT (aprobado por Meta a las 12:21 PM). Es un cambio real de cuenta, ejecutado manualmente por el usuario vía Power Editor, no por esta sesión ni por ninguna automatización.
- **Nuevo administrador agregado a la cuenta publicitaria** a las 9:07 AM GT (user id `3158599694341600`), también manual.
- **Ningún cambio fue realizado por esta sesión.** Esta rutina automatizada solo leyó métricas y el activity log; no modificó presupuestos, targeting, copy ni estado de campañas.
- **Ningún cambio de infraestructura intentado hoy** (no se reintentó reprogramar el trigger).

---

## 📊 Análisis e Insights

- **El CPL blendeado de la cuenta sube a $5.96 (+29.0% vs. el $4.62 de ayer)** — se mantiene dentro/cerca de la meta $6-7, pero revierte la mejora radical documentada ayer.
- **Los leads confirmados bajan de 9 a 8 (-11.1%) mientras el gasto sube +14.6%** ($41.60 → $47.68) — combinación doblemente desfavorable: menos resultados con más inversión.
- **Dos de cinco campañas activas cierran en cero leads** (Pyme El Salvador, Odoo Test), justo las dos que ayer se habían recuperado — refuerza la sospecha de que sus ceros son un patrón recurrente, no variance puntual de un solo día.
- **CTR blendeado cae a 1.44% (-14.3% vs. ayer) y CPC sube a $0.41 (+17.1%)** — el tráfico fue menos eficiente hoy, no solo la conversión a lead.
- **CPM se mantiene estable** ($5.88 vs. $5.89, -0.2%) — el costo de exposición no cambió; el deterioro es en clics y conversión, no en la puja/competencia por audiencia.
- **Beco es el punto fuerte inesperado del día**: pasa de ser la única campaña fuera de meta ayer ($9.36 CPL) a la segunda mejor hoy ($3.59 CPL, 3 leads) — vale la pena investigar si hubo algún cambio no registrado en el activity log (p. ej. optimización automática de Meta) que explique el salto.
- El reemplazo de creativo en Pyme Colombia es la primera acción concreta hacia el A/B test de copys pendiente en [[CLAUDE.md]], aunque aplicado a una campaña distinta a la originalmente planeada (GT en vez de Colombia) y sin configurarse como test formal — insuficiente aún para medir impacto real por la ventana corta de exposición (~11h).
- Ninguna investigación de competencia o tendencias externas se realizó en esta sesión.

> [!caution] No confirmar como cierre real
> Estas cifras corresponden a una lectura tomada ~9 minutos antes del cierre real de 2026-09-25 y pueden moverse al resolverse la ventana de atribución de leads. Confirmar con el Reporte Performance formal cuando esté disponible (~7 AM GT).

---

## 📊 Datos Clave del Día

| Métrica (5 campañas activas) | 2026-09-25 (casi-final) | 2026-09-24 (casi-final, nota anterior) | Variación |
|---------|---------------------------|----------------------------------|-----------|
| Gasto Total | $47.68 | $41.60 | 🔻 +14.6% |
| Leads Confirmados | 8 | 9 | 🔻 -11.1% |
| CPL Promedio (blendeado) | **$5.96** | $4.62 | 🔻 +29.0% |
| CTR Promedio (blendeado) | 1.44% | 1.68% | 🔻 -14.3% |
| CPC Promedio | $0.41 | $0.35 | 🔻 +17.1% |
| CPM Promedio | $5.88 | $5.89 | 🟢 -0.2% |
| Impresiones | 8,103 | 7,064 | 🔺 +14.7% |
| Clicks | 117 | 119 | 🔻 -1.7% |
| Alcance (Reach) | 6,304 | 5,171 | 🔺 +21.9% |
| Mejor CPL del día | Toma El control (GT): **$3.55** | Toma El control (GT): $2.95 | Mismo líder, sube CPL |
| Peor performer del día | Pyme El Salvador y Odoo Test: $0 leads (empate) | Beco: $9.36 (único fuera de meta) | Cambia de tipo de problema |

**Detalle por campaña:**
- Toma El control de tu pyme (GT): $14.21 / 4 leads / $3.55 CPL
- Beco (GT): $10.77 / 3 leads / $3.59 CPL / 107.7% del presupuesto diario
- Pyme El Salvador (SV): $11.79 / 0 leads / 94.3% del presupuesto diario
- Pyme Colombia (COL): $6.09 / 1 lead / $6.09 CPL / 81.2% del presupuesto diario (incluye el nuevo creativo "Urgencia")
- Odoo Test (GT): $4.82 / 0 leads / 97.8% del presupuesto diario

---

## 📋 Próximas Acciones

- [ ] Confirmar mañana (~7 AM GT) el cierre real de 2026-09-25 vía Reporte Performance, en especial si el CPL blendeado (~$5.96) se mantiene o empeora con la ventana de atribución
- [ ] Investigar por qué Pyme El Salvador y Odoo Test vuelven a cero leads tras un solo día de recuperación — confirmar si es un patrón estructural (creativo, tracking, audiencia) en vez de variance
- [ ] Dar seguimiento a la creatividad "Urgencia" de Pyme Colombia con un día completo de datos antes de sacar conclusiones sobre su desempeño
- [ ] Evaluar formalizar el reemplazo de creativo de hoy como parte del A/B testing pendiente de los 5 nuevos copys, y decidir si también se aplica a "Toma El control de tu pyme" (GT), la campaña originalmente documentada en [[CLAUDE.md]]
- [ ] Investigar la mejora inesperada de Beco (de $9.36 a $3.59 CPL) para entender si es sostenible o un evento puntual
- [ ] Ajustar el `daily_budget` de Beco — sigue levemente sobre presupuesto (107.7%)
- [ ] **Usuario:** el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` sigue disparándose a las 23:50 GT en vez de después de medianoche (15ª ocurrencia consecutiva sin resolver) — solo se puede corregir manualmente desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ, ningún agente automatizado tiene permiso para editarlo
- [ ] **Usuario:** confirmar que el nuevo administrador agregado hoy a la cuenta (9:07 AM GT) es una adición esperada

---

## 🔗 Enlaces

- [[Reports/2026-09-24 - Reporte Performance]] — último reporte de cierre confirmado disponible (el de 2026-09-25 se genera mañana ~7 AM GT)
- [[Daily notes/2026-09-25 - Resumen del Dia]] — resumen del día anterior
- Tags: #daily-note #summary #meta-ads #octopus
