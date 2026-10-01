---
date: 2026-09-30
aliases: [reporte-2026-09-30, performance-30-sep]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-09-30

> [!info] Datos de cierre confirmados
> Pull realizado la mañana del 2026-10-01 (rutina "Daily Meta Ads Performance Report - 7 AM Guatemala") con `date_preset=yesterday`, día ya cerrado completamente en horario de Guatemala (GMT-6). El total de cuenta a nivel `ad_account` cuadra exactamente con la suma de las 5 campañas activas (gasto $48.78, impresiones 7,445, clicks 101, y CPL blendeado $12.20 = $48.78 / 4 leads confirmados). El alcance de cuenta (5,712) es menor que la suma simple por campaña (5,866) por solape normal de audiencias. El activity log de la cuenta para la ventana 2026-09-30 00:00 GT – 2026-10-01 08:00 GT registra un único evento, 100% automático (`actor_name: "Meta"`): la creación de la audiencia personalizada `asa_auto_custom_audience` (9/30 ~5:36 PM hora de cuenta) — ninguna acción manual sobre presupuesto, targeting, creativo o estado de campañas.

> [!note] Sobre `Daily notes/2026-09-30 - Resumen del Dia.md`
> Ese archivo (sin acento en "Dia") fue creado por la rutina distinta "Daily Summary - 11:50 PM Guatemala" (`trig_01DMJfrsQXaTY5KJntXisDPQ`), que se dispara a las 23:50 GT — antes de medianoche — por lo que documenta en realidad datos casi-finales de **2026-09-29**, no de 2026-09-30 (bug de zona horaria confirmado vía `list_triggers`: cron sin cambios en `50 5 * * *` UTC desde su creación el 2026-08-28). Ese mismo bug produjo además `Daily notes/2026-10-01 - Resumen del Dia.md`, que documenta la lectura **casi-final de 2026-09-30** (20ª ocurrencia consecutiva confirmada en esa nota). Este reporte confirma esa lectura casi-final (CPL $11.96 → $12.20, 4 leads en ambas lecturas, gasto $47.83 → $48.78) y genera además [[Daily notes/2026-09-30 - Resumen del Día]] **(con acento, archivo distinto)** como el resumen ejecutivo confirmado del día que pide esta rutina, sin sobrescribir la nota casi-final existente de la otra rutina.

## 📋 Resumen Ejecutivo

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| **CPL Promedio** | $12.20 USD | $6-7 | 🔴 Fuera de meta, -2.7% vs. 09-29 ($12.54) — mejora marginal, sigue +74-103% sobre el techo de meta |
| **Gasto Total** | $48.78 USD | - | 🟢 -2.7% vs. 09-29 ($50.16) |
| **Leads Totales** | 4 | 4-5/día | 🟡 En el límite inferior de meta, estable vs. 09-29 (4) |
| **CTR Promedio** | 1.36% | 3-4% | 🔴 Por debajo de meta, -8.1% vs. 09-29 (1.48%) |
| **CPC Promedio** | $0.48 USD | - | 🔴 +9.1% vs. 09-29 ($0.44) |
| **CPM Promedio** | $6.55 USD | - | 🔴 +1.7% vs. 09-29 ($6.44) |
| **Impresiones** | 7,445 | - | 🔻 -4.4% vs. 09-29 (7,784) |
| **Clicks** | 101 | - | 🔻 -12.2% vs. 09-29 (115) |
| **Alcance (Reach)** | 5,712 | - | 🔻 -1.9% vs. 09-29 (5,823) |
| **ROAS** | No aplica | - | Campañas Lead Gen sin tracking de valor de conversión |

**Nota:** El CPL de cuenta baja levemente a $12.20 (-2.7% vs. 09-29), una mejora marginal que no cambia el panorama: sigue muy por encima de la meta $6-7. Los leads confirmados se mantienen en 4, igual que ayer, con gasto algo menor (-2.7%) — mismo volumen con algo menos de inversión, pero la composición por campaña cambió por completo: **Beco** da el giro más fuerte del día, duplicando sus leads y cayendo -46.3% de CPL hasta ser la única campaña dentro de meta; **Odoo Test**, que ayer fue el mejor performer de la cuenta, cae a cero leads; y **Pyme Colombia** encadena su segundo cierre confirmado consecutivo en cero.

## 🎯 Performance por Campaña (Ranked por CPL)

### 1. [[Beco]] (GT) — Mejor performer del día, única campaña dentro de meta 🟢
```
CPL: $4.88 USD 🟢
Leads: 2
Gasto: $9.75 USD
Clicks: 23
CTR: 1.21% 🔴
CPC: $0.42 USD
CPM: $5.12 USD
Impresiones: 1,905
Reach: 1,612
```
**Status:** ACTIVE — Presupuesto/día: $10.00 (gasto = 97.5% del presupuesto)
**Insight:** Pasa de 1 a 2 leads con gasto casi plano ($9.08 CPL → $4.88 CPL, -46.3%), duplicando conversión. Es la primera vez en varios cierres que una campaña cierra por debajo de la meta $6-7 y hoy es, por un margen amplio, la mejor de la cuenta.

### 2. [[Pyme El salvador]] (SV) — Empeora y sigue entre las más caras 🔴
```
CPL: $14.04 USD 🔴
Leads: 1
Gasto: $14.04 USD
Clicks: 32
CTR: 1.35% 🔴
CPC: $0.44 USD
CPM: $5.92 USD
Impresiones: 2,370
Reach: 1,758
```
**Status:** ACTIVE — Presupuesto/día: $12.50 (gasto = 112.3% del presupuesto, sobre-gasto)
**Insight:** Sube de $12.58 a $14.04 CPL (+11.6%) manteniendo 1 lead, y gasta 12.3% por encima de su presupuesto diario configurado — la única campaña con sobregasto hoy.

### 3. [[Toma El control de tu pyme]] (GT) — Mejora leve pero lejos de su mejor cierre confirmado 🔴
```
CPL: $14.14 USD 🔴
Leads: 1
Gasto: $14.14 USD
Clicks: 29
CTR: 1.30% 🔴
CPC: $0.49 USD
CPM: $6.34 USD
Impresiones: 2,231
Reach: 1,746
```
**Status:** ACTIVE — Presupuesto del único ad set activo ("TestA/B Urgencia"): $15.00 (gasto = 94.3% del presupuesto)
**Insight:** Es la campaña ancla del proyecto (foco del A/B test de 5 copys pendiente en [[CLAUDE.md]]) y mejora levemente su CPL (-6.4% vs. 09-29) pero sigue muy por encima de su mejor cierre confirmado ($4.64 CPL). El A/B test de copys sigue sin iniciarse formalmente.

### 4. [[Pyme Colombia]] (COL) — Segundo cierre confirmado consecutivo en cero 🔴
```
CPL: N/D (sin leads) 🔴
Leads: 0
Gasto: $6.54 USD
Clicks: 11
CTR: 2.81% 🟡
CPC: $0.59 USD
CPM: $16.68 USD
Impresiones: 392
Reach: 302
```
**Status:** ACTIVE — Presupuesto/día: $7.50 (gasto = 87.2% del presupuesto)
**Insight:** Cierra en cero por segundo día confirmado consecutivo, tras romper el 09-29 una racha de tres cierres dentro de meta con el creativo "Urgencia". El CTR relativo sigue siendo el más alto de la cuenta (2.81%), lo que hace menos probable una causa de creativo y refuerza la necesidad de revisar tracking/pixel antes de asumir solo volatilidad.

### 5. [[Odoo Test]] (GT) — Revierte a cero tras ser el mejor performer confirmado de ayer 🔴
```
CPL: N/D (sin leads) 🔴
Leads: 0
Gasto: $4.31 USD
Clicks: 6
CTR: 1.10% 🔴
CPC: $0.72 USD
CPM: $7.88 USD
Impresiones: 547
Reach: 448
```
**Status:** ACTIVE — Presupuesto/día: $4.93 (gasto = 87.4% del presupuesto)
**Insight:** Ayer confirmado fue el mejor performer de la cuenta ($5.68 CPL, 1 lead); hoy vuelve a cero con gasto similar, sin cambio manual registrado. Suma otro ciclo al patrón "cero → positivo → cero" ya documentado varias veces en esta campaña.

### Campañas sin actividad (PAUSED, $0 gasto)
- Toma El control de tu pyme (USA)
- Accurate Partners - Loyalti - Nuevas Obligaciones - JUN 2026
- Conversión Clientes Potenciales - MX
- Conversión Clientes Potenciales - PY
- 🟡 CONVERSIÓN - CLIENTES POTENCIALES

## 🔄 Cambios de cuenta detectados (confirmado vía activity log)

- **Un único evento, 100% automático.** El activity log de la cuenta para la ventana 2026-09-30 00:00 GT – 2026-10-01 08:00 GT registra solo "Custom audience created" (`asa_auto_custom_audience`), generado por el propio sistema de Meta (`actor_name: "Meta"`, `actor_id: 0`) el 9/30 a las 5:36 PM. Ninguna acción manual sobre presupuesto, targeting, creativo o estado de campañas.

## 💡 Insights Clave

- **El CPL de cuenta baja a $12.20 (-2.7% vs. 09-29), una mejora marginal** que no acerca a la cuenta a la meta $6-7 — sigue +74% a +103% por encima del rango objetivo.
- **Los leads confirmados se mantienen en 4, igual que ayer, con gasto algo menor** ($50.16 → $48.78, -2.7%) — mismo volumen de leads con algo menos de inversión, pero con un cambio total en qué campañas los generan.
- **Beco da el giro más fuerte del día:** duplica sus leads (1→2) y cae -46.3% de CPL hasta $4.88, la única campaña dentro de meta y el mejor performer de la cuenta por un margen amplio.
- **Odoo Test revierte a cero justo después de ser el mejor performer confirmado de ayer** — ya es un patrón recurrente de "cero → positivo → cero" sin correlato en el activity log, documentado varias veces en esta campaña.
- **Pyme Colombia encadena su segundo cierre confirmado consecutivo en cero**, con CTR relativo aún alto (2.81%, el mejor de la cuenta) — ya no se puede tratar como evento aislado; merece verificación de pixel/tracking antes de seguir asumiendo solo volatilidad de subasta.
- **CTR de cuenta retrocede a 1.36% (-8.1% vs. 09-29) y se mantiene muy por debajo de la meta 3-4%** en las 5 campañas activas, sin excepción.
- **Pyme El Salvador es la única campaña con sobregasto hoy (112.3% de su presupuesto diario)**; el resto cierra entre 87.2% y 97.5%.
- **Este cierre confirma, con un ajuste menor de gasto, la lectura casi-final documentada en [[Daily notes/2026-10-01 - Resumen del Dia]]:** CPL confirmado $12.20 vs. $11.96 casi-final, 4 leads en ambas lecturas, gasto $48.78 vs. $47.83 casi-final — la ventana de atribución no sumó leads adicionales, solo un ligero ajuste de gasto (+2.0%).

## ✅ Recomendaciones Accionables

- [ ] **Dar seguimiento al giro de Beco:** duplicó leads y bajó -46.3% su CPL hasta ser la única campaña dentro de meta — confirmar si se sostiene en el próximo cierre antes de considerar escalar su presupuesto.
- [ ] **Escalar la verificación de Pyme Colombia:** ya son dos cierres confirmados consecutivos en cero leads con CTR relativo alto (2.81%) — revisar pixel, tracking de leads y calidad de audiencia específicamente para esta campaña antes del próximo ajuste de presupuesto.
- [ ] **Seguir documentando el patrón cíclico de Odoo Test (y, en menor medida, Beco):** ya van varios ciclos de "cero → positivo → cero" sin correlato en el activity log — evaluar si amerita una revisión de creativo/targeting dedicada en vez de seguir monitoreando pasivamente.
- [ ] **Retomar el A/B testing pendiente de los 5 nuevos copys** en "Toma El control de tu pyme" (GT), documentado en [[CLAUDE.md]] pero aún sin iniciar formalmente — la campaña sigue entre las más caras de la cuenta, muy lejos de su mejor cierre confirmado ($4.64 CPL).
- [ ] **Ajustar el `daily_budget` de Pyme El Salvador:** cierra con sobregasto (112.3%) y CPL en aumento (+11.6%) — revisar antes de que el patrón se repita.
- [ ] **Usuario:** el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") sigue disparándose a las 23:50 GT en vez de después de medianoche — 20ª ocurrencia consecutiva confirmada vía `list_triggers` (cron sin cambios desde su creación el 2026-08-28), causando que sus notas en `Daily notes/` queden mal etiquetadas con los datos del día anterior. Solo se puede corregir manualmente desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ; ningún agente automatizado tiene permiso para editarlo.

## 🔗 Enlaces Relacionados

- [[Daily notes/2026-09-30 - Resumen del Día]] - Resumen ejecutivo confirmado del día generado por esta misma rutina
- [[Daily notes/2026-10-01 - Resumen del Dia]] - Lectura casi-final registrada anoche por la otra rutina automatizada (mal etiquetada como "10-01"), consistente con este cierre confirmado
- [[Reports/2026-09-29 - Reporte Performance]] - Reporte del día anterior
- [[CLAUDE.md]] - Meta de CPL $6-7 (fuera de meta hoy); A/B test de 5 copys mejorados pendiente de formalizar en "Toma El control de tu pyme"
- [[cloud.md]] - Dashboard principal

---
Generado por: Claude Code (Reporte Automatizado) + Meta Ads API
Cuenta: GT | Octopus Innovations (2530001557366648)
Fecha: 2026-09-30
Tags: #daily-note #performance #meta-ads #octopus
