---
date: 2026-10-07
aliases: [reporte-2026-10-07, performance-07-oct]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-10-07

> [!info] Datos de cierre confirmados
> Pull realizado la mañana del 2026-10-08 (rutina "Daily Meta Ads Performance Report - 7 AM Guatemala") con rango explícito 2026-10-07 a 2026-10-07 (`date_preset=yesterday`), día ya cerrado completamente en horario de Guatemala (GMT-6). El total de cuenta a nivel `ad_account` cuadra exactamente con la suma de las 5 campañas activas (gasto $50.13, impresiones 7,165 y clicks 116, todos coinciden exacto con la suma por campaña). El alcance de cuenta (5,625) es menor que la suma simple por campaña (5,763) por solapamiento normal de audiencias entre campañas activas. El activity log de la cuenta para la ventana 2026-10-07 06:00–2026-10-08 06:00 UTC registra 10 eventos "Custom audience created", todos generados automáticamente por Meta (`actor_name: "Meta"`, `asa_auto_custom_audience`), no por el usuario.

> [!note] Sobre `Daily notes/2026-10-08 - Resumen del Dia.md`
> Ese archivo (sin acento) fue creado por la rutina distinta "Daily Summary - 11:50 PM Guatemala" (`trig_01DMJfrsQXaTY5KJntXisDPQ`), que se dispara a las 23:50 GT — antes de medianoche — por lo que documenta en realidad datos casi-finales de **2026-10-07** (el día que confirma este reporte), mal etiquetados como "10-08". Esa lectura casi-final ya anticipaba correctamente el repunte de "Toma El control" a 4 leads y la caída simultánea del trío Pyme Colombia/Odoo Test/Beco a cero: CPL blendeado $8.17 casi-final → $8.36 confirmado, 6 leads en ambas lecturas; Toma El control $3.75 → $3.85 (4 leads en ambas); Pyme El Salvador $6.60 → $6.74 (2 leads en ambas); el trío se confirma en 0 leads en ambas lecturas. Este reporte genera además [[Daily notes/2026-10-07 - Resumen del Día]] (con acento) como el resumen ejecutivo confirmado del día, sin sobrescribir la nota casi-final existente de la otra rutina ni el archivo "2026-10-07 - Resumen del Dia.md" (sin acento, que en realidad documenta el cierre del 10-06 por el mismo problema de etiquetado).

## 📋 Resumen Ejecutivo

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| **CPL Promedio** | $8.36 USD | $6-7 | 🟡 +19.4% a +39.3% por encima de la meta, pero el segundo mejor cierre confirmado de la serie reciente; empeora +8.9% vs. el cierre confirmado de 10-06 ($7.68) |
| **Gasto Total** | $50.13 USD | - | 🔴 +8.8% vs. 10-06 ($46.06) |
| **Leads Totales** | 6 | 4-5/día | 🟢 Iguala el cierre de ayer (0.0%) y vuelve a superar la meta por segundo día consecutivo |
| **CTR Promedio** | 1.62% | 3-4% | 🔴 Por debajo de meta, retrocede -5.8% vs. 10-06 (1.72%) |
| **CPC Promedio** | $0.43 USD | - | 🔻 +16.2% vs. 10-06 ($0.37) |
| **CPM Promedio** | $7.00 USD | - | 🔻 +8.9% vs. 10-06 ($6.43) |
| **Impresiones** | 7,165 | - | ⚪ -0.03% vs. 10-06 (7,167), prácticamente estable |
| **Clicks** | 116 | - | 🔻 -5.7% vs. 10-06 (123) |
| **Alcance (Reach)** | 5,625 | - | 🟢 +2.5% vs. 10-06 (5,489) |
| **ROAS** | No aplica | - | Campañas Lead Gen sin tracking de valor de conversión |

**Nota:** El CPL blendeado sube +8.9% a $8.36 y se aleja ligeramente de la meta $6-7, pero sigue siendo el segundo mejor cierre confirmado de toda la serie documentada desde el 2026-10-01 (solo detrás del $7.68 del 10-06), muy por debajo de los picos de $16-17 de inicios de octubre. El cierre repite casi exactamente el patrón de sube-y-baja ya visto el 10-05/10-06: **"Toma El control de tu pyme"**, que ayer cerró en cero leads por primera vez en la serie, se dispara hoy a **4 leads con $3.85 CPL** — su mejor cierre documentado hasta ahora. En sentido contrario, el trío **Pyme Colombia, Odoo Test y Beco**, que ayer se había recuperado los tres a la vez, cae hoy de nuevo a **cero leads simultáneamente** — la tercera vez que ocurre este patrón de trío. **Pyme El Salvador** alcanza por primera vez en toda la serie el rango meta de CPL ($6.74).

## 🎯 Performance por Campaña (Ranked por CPL)

### 1. [[Toma El control de tu pyme]] (GT) — Mejor CPL documentado de la campaña, rompe su propia racha de volatilidad 🟢
```
CPL: $3.85 USD 🟢
Leads: 4
Gasto: $15.38 USD
Clicks: 32
CTR: 1.61% 🔴
CPC: $0.48 USD
CPM: $7.74 USD
Impresiones: 1,988
Reach: 1,518
```
**Status:** ACTIVE — Presupuesto a nivel campaña: N/D (ABO, presupuesto gestionado a nivel ad set)
**Insight:** Un día después de cerrar en cero leads por primera vez en la serie, se dispara hoy a 4 leads con **$3.85 CPL** — su mejor cierre documentado desde el 2026-10-01, superando ampliamente su anterior mejor marca ($6.59, -41.6%). Es la sexta oscilación de polaridad en seis días consecutivos ($17.50 → $6.59 → $16.36 → $8.01 → 0 leads → **$3.85**), esta vez del lado positivo, sin ningún cambio manual registrado en el activity log que lo explique. Es, no obstante, el segundo mejor CPL de toda la cuenta documentada, detrás del $1.79 de Odoo Test del 2026-10-01 (ver [[Reports/2026-10-01 - Reporte Performance]]). Importante: este resultado llega **sin que el A/B test de los 5 copys mejorados** (documentado en [[CLAUDE.md]] desde el 2026-08-24) se haya lanzado formalmente aún, por lo que la mejora no puede atribuirse al nuevo copy.

### 2. [[Pyme El salvador]] (SV) — Alcanza la meta de CPL por primera vez en la serie 🟢
```
CPL: $6.74 USD 🟢
Leads: 2
Gasto: $13.47 USD
Clicks: 28
CTR: 1.55% 🔴
CPC: $0.48 USD
CPM: $7.45 USD
Impresiones: 1,807
Reach: 1,378
```
**Status:** ACTIVE — Presupuesto/día: $12.50 (gasto = 107.8% del presupuesto)
**Insight:** Mejora -37.0% vs. el cierre confirmado de ayer ($10.70) y cae por primera vez dentro del rango meta $6-7 en toda la serie documentada, con el doble de leads (2 vs. 1). El CTR retrocede -17.6% (1.88%→1.55%) pese a la mejora de CPL.

### 3. [[Pyme Colombia]] (COL) — Cae a cero leads pese al mejor CTR de la cuenta 🔴
```
Leads: 0
Gasto: $7.85 USD
Clicks: 25
CTR: 3.89% 🟢
CPC: $0.31 USD
CPM: $12.21 USD
Impresiones: 643
Reach: 509
```
Sin CPL calculable (0 leads).
**Status:** ACTIVE — Presupuesto/día: $7.50 (gasto = 104.7% del presupuesto)
**Insight:** Revierte su recuperación de ayer (3 leads, $2.50 CPL) y cae a cero, pese a registrar el mejor CTR de toda la cuenta hoy (3.89%, +25.5% vs. ayer) — una desconexión entre tráfico y conversión a lead similar a la observada en "Toma El control" el 10-06. Es la tercera vez que el trío {Pyme Colombia, Odoo Test, Beco} cae a cero leads de forma simultánea en la serie documentada.

### 4. [[Beco]] (GT) — Cae a cero leads 🔴
```
Leads: 0
Gasto: $8.47 USD
Clicks: 27
CTR: 1.36% 🔴
CPC: $0.31 USD
CPM: $4.25 USD
Impresiones: 1,992
Reach: 1,716
```
Sin CPL calculable (0 leads).
**Status:** ACTIVE — Presupuesto/día: $10.00 (gasto = 84.7% del presupuesto, el único por debajo del 100% hoy)
**Insight:** Revierte el lead conseguido ayer ($10.04 CPL) y cierra en cero. El CTR se mantiene relativamente estable (1.32%→1.36%, +3.0%) pero no se traduce en conversión a lead.

### 5. [[Odoo Test]] (GT) — Cae a cero leads, CTR más débil de la cuenta 🔴
```
Leads: 0
Gasto: $4.96 USD
Clicks: 4
CTR: 0.54% 🔴
CPC: $1.24 USD
CPM: $6.75 USD
Impresiones: 735
Reach: 642
```
Sin CPL calculable (0 leads).
**Status:** ACTIVE — Presupuesto/día: $4.93 (gasto = 100.6% del presupuesto)
**Insight:** Revierte el lead conseguido ayer ($4.72 CPL) y cierra en cero. Su CTR cae -42.6% (0.94%→0.54%), el más débil de toda la cuenta hoy, y su CPC ($1.24) es el más alto de la cuenta.

### Campañas sin actividad (PAUSED, $0 gasto)
- Toma El control de tu pyme (USA)
- Accurate Partners - Loyalti - Nuevas Obligaciones - JUN 2026
- Conversión Clientes Potenciales - MX
- Conversión Clientes Potenciales - PY
- 🟡 CONVERSIÓN - CLIENTES POTENCIALES

## 🔄 Cambios de cuenta detectados (confirmado vía activity log)

- **10 eventos "Custom audience created"**, todos registrados a las 6:50 AM del 10/7 y generados automáticamente por Meta (`actor_name: "Meta"`, objeto `asa_auto_custom_audience`), no por el usuario. Es la segunda ventana consecutiva con este tipo de evento automático tras 7 ventanas previas sin ningún registro (ver [[Reports/2026-10-06 - Reporte Performance]]). No son cambios de presupuesto, targeting ni copy, y no explican ninguna de las oscilaciones de CPL/leads observadas hoy.

## 💡 Insights Clave

- **El CPL de cuenta sube +8.9% a $8.36** — se aleja ligeramente de la meta $6-7 (ahora +19.4% a +39.3% por encima), pero sigue siendo el segundo mejor cierre confirmado de toda la serie documentada desde el 2026-10-01, muy por debajo de los picos de $16-17 de inicios de octubre.
- **Los leads confirmados se mantienen en 6** (igual que el 10-06), pero el gasto sube +8.8% ($46.06 → $50.13) — la eficiencia empeora levemente porque el trío {Pyme Colombia, Odoo Test, Beco} vuelve a gastar presupuesto sin convertir, mientras "Toma El control" compensa con su mejor CPL de la serie.
- **Solo 2 de 5 campañas activas generan leads hoy** (Toma El control y Pyme El Salvador), igual que ayer en cantidad, pero con los roles casi invertidos respecto al trío — tercera oscilación de polaridad consecutiva entre "Toma El control" y el trío {Pyme Colombia, Odoo Test, Beco}.
- **"Toma El control de tu pyme" firma su mejor CPL documentado desde el inicio de la serie** ($3.85, 4 leads), superando su anterior mejor marca ($6.59) en -41.6% — sin que el A/B test de los 5 copys mejorados (documentado en [[CLAUDE.md]] desde el 2026-08-24) se haya lanzado formalmente aún, según el activity log.
- **"Pyme El Salvador" alcanza por primera vez en toda la serie documentada el rango meta de CPL** ($6-7), con $6.74 y 2 leads.
- **CTR blendeado cae a 1.62% (-5.8% vs. 1.72% de ayer)**, mientras CPC sube a $0.43 (+16.2%) y CPM sube a $7.00 (+8.9%) — el deterioro combina una subasta más cara con menos eficiencia de click, parcialmente compensado por la fuerte conversión a lead de "Toma El control".
- **Este cierre confirma, con ajuste menor al alza, la lectura casi-final documentada en [[Daily notes/2026-10-08 - Resumen del Dia]]** (mal etiquetada como "10-08" por el mismo bug de horario de la otra rutina): CPL confirmado $8.36 vs. $8.17 casi-final, 6 leads en ambas lecturas, gasto $50.13 vs. $49.01 casi-final (+2.3%).

## ✅ Recomendaciones Accionables

- [ ] **Lanzar por fin el A/B testing de los 5 copys mejorados** documentado en [[CLAUDE.md]] desde el 2026-08-24 para "Toma El control de tu pyme" — la campaña acaba de firmar su mejor CPL de la serie ($3.85) **sin** que el test se haya lanzado, lo que significa que la mejora no puede atribuirse todavía al nuevo copy; formalizar el test permitiría medir causalmente futuras mejoras en lugar de atribuirlas a volatilidad natural.
- [ ] **Investigar si la caída simultánea a cero leads de Pyme Colombia, Odoo Test y Beco** (tercera vez que ocurre) responde a un problema técnico de tracking/formulario — Pyme Colombia registra hoy su mejor CTR de la cuenta (3.89%) sin que se traduzca en ningún lead, una desconexión que merece revisión de pixel/lead form y no solo de creativo.
- [ ] **Confirmar si "Pyme El Salvador" sostiene** su primer cierre dentro de meta ($6.74 CPL) en el próximo reporte o fue puntual.
- [ ] **Extender la revisión creativa a toda la cuenta:** el CTR blendeado (1.62%) sigue muy por debajo de la meta 3-4% incluso en días de buen CPL — el problema de atractivo de los creativos parece generalizado, no aislado a una campaña.
- [ ] **Usuario:** el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") sigue disparándose antes de medianoche GT, causando que sus notas en `Daily notes/` queden mal etiquetadas con los datos del día anterior (ver [[Daily notes/2026-10-08 - Resumen del Dia]]). Solo se puede corregir manualmente desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ; ningún agente automatizado tiene permiso para editarlo.

## 🔗 Enlaces Relacionados

- [[Daily notes/2026-10-07 - Resumen del Día]] - Resumen ejecutivo confirmado del día generado por esta misma rutina
- [[Daily notes/2026-10-08 - Resumen del Dia]] - Lectura casi-final registrada anoche por la otra rutina automatizada (mal etiquetada como "10-08"), consistente con este cierre confirmado
- [[Reports/2026-10-06 - Reporte Performance]] - Reporte del día anterior
- [[Reports/2026-10-01 - Reporte Performance]] - Contiene el mejor CPL confirmado de toda la serie (Odoo Test, $1.79)
- [[CLAUDE.md]] - Meta de CPL $6-7; A/B test de 5 copys mejorados aún pendiente de formalizar en "Toma El control de tu pyme" pese a su mejor cierre de la serie
- [[cloud.md]] - Dashboard principal

---
Generado por: Claude Code (Reporte Automatizado) + Meta Ads API
Cuenta: GT | Octopus Innovations (2530001557366648)
Fecha: 2026-10-07
Tags: #daily-note #performance #meta-ads #octopus
