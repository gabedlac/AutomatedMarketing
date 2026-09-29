---
date: 2026-09-28
aliases: [reporte-2026-09-28, performance-28-sep]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-09-28

> [!info] Datos de cierre confirmados
> Pull realizado la mañana del 2026-09-29 (rutina "Daily Meta Ads Performance Report - 7 AM Guatemala") con `time_range` explícito (`2026-09-28` a `2026-09-28`), día ya cerrado completamente en horario de Guatemala (GMT-6). El total de cuenta a nivel `ad_account` cuadra exactamente con la suma de las 5 campañas activas (gasto $47.61, impresiones 7,711, clicks 102, y CPL blendeado $7.94 = $47.61 / 6 leads confirmados). El alcance de cuenta (5,802) es menor que la suma simple por campaña (6,211) por solape normal de audiencias. El activity log de la cuenta para la ventana 2026-09-28 00:00 UTC – 2026-09-29 13:19 UTC solo registra un evento automático de facturación de Meta ("Account billed", 9/28 4:16 AM) — sin cambios manuales.

> [!note] Sobre `Daily notes/2026-09-29 - Resumen del Dia.md`
> Ese archivo (sin acento en "Dia") fue creado por la rutina distinta "Daily Summary - 11:50 PM Guatemala" (`trig_01DMJfrsQXaTY5KJntXisDPQ`), que se dispara a las 23:50 GT — antes de medianoche — por lo que documenta en realidad datos casi-finales de **2026-09-28**, no de 2026-09-29 (bug de zona horaria documentado 18 veces consecutivas en el proyecto, sin cambios en el cron desde su creación el 2026-08-28). Este reporte confirma esa lectura casi-final ($7.74 CPL, 6 leads, $46.41 gasto → $7.94 CPL, 6 leads, $47.61 gasto confirmados) y genera además [[Daily notes/2026-09-28 - Resumen del Día]] **(con acento, archivo distinto)** como el resumen ejecutivo confirmado del día que pide esta rutina, sin sobrescribir la nota casi-final existente de la otra rutina.

## 📋 Resumen Ejecutivo

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| **CPL Promedio** | $7.94 USD | $6-7 | 🔴 Fuera de meta, +55.4% vs. 09-27 ($5.11) — revierte el mejor cierre confirmado del proyecto |
| **Gasto Total** | $47.61 USD | - | 🔻 -22.4% vs. 09-27 ($61.37) |
| **Leads Totales** | 6 | 4-5/día | 🟡 Dentro de meta pero -50.0% vs. 09-27 (12) |
| **CTR Promedio** | 1.32% | 3-4% | 🔴 Por debajo de meta, -15.9% vs. 09-27 (1.57%) |
| **CPC Promedio** | $0.47 USD | - | 🔴 +11.9% vs. 09-27 ($0.42) |
| **CPM Promedio** | $6.17 USD | - | 🟢 -5.8% vs. 09-27 ($6.55) |
| **Impresiones** | 7,711 | - | 🔻 -17.7% vs. 09-27 (9,367) |
| **Clicks** | 102 | - | 🔻 -30.6% vs. 09-27 (147) |
| **Alcance (Reach)** | 5,802 | - | 🔻 -18.1% vs. 09-27 (7,086) |
| **ROAS** | No aplica | - | Campañas Lead Gen sin tracking de valor de conversión |

**Nota:** El CPL de cuenta sube a $7.94 (+55.4% vs. 09-27), revirtiendo el mejor cierre confirmado documentado hasta ahora y volviendo a estar fuera de la meta $6-7. El retroceso combina menor gasto (-22.4%) y una caída de leads mayor (-50.0%): Beco y Odoo Test, que ayer cerraron entre las mejores campañas de la cuenta, hoy cierran ambas en cero leads sin ningún cambio manual registrado. Las otras 3 campañas activas (Toma El control, Pyme Colombia, Pyme El Salvador) sí generaron leads, dos de ellas dentro de meta de CPL.

## 🎯 Performance por Campaña (Ranked por CPL)

### 1. [[Toma El control de tu pyme]] (GT) — Mejor performer del día, mejor cierre confirmado de la campaña 🟢
```
CPL: $4.64 USD 🟢
Leads: 3
Gasto: $13.93 USD
Clicks: 40
CTR: 1.76% 🟡
CPC: $0.35 USD
CPM: $6.12 USD
Impresiones: 2,278
Reach: 1,860
```
**Status:** ACTIVE — Presupuesto del único ad set activo ("TestA/B Urgencia"): $15.00 (gasto = 92.9% del presupuesto)
**Insight:** Mantiene 3 leads y mejora su CPL de $5.95 a $4.64 (-22.0%) — su mejor cierre confirmado hasta ahora y hoy la campaña líder de la cuenta. El A/B test de 5 copys nuevos documentado en [[CLAUDE.md]] sigue sin iniciarse formalmente; "TestA/B Urgencia" sigue siendo el único ad set activo.

### 2. [[Pyme Colombia]] (COL) — Tercera lectura consecutiva positiva con el creativo "Urgencia" 🟢
```
CPL: $4.67 USD 🟢
Leads: 2
Gasto: $9.34 USD
Clicks: 13
CTR: 2.04% 🟡
CPC: $0.72 USD
CPM: $14.64 USD
Impresiones: 638
Reach: 483
```
**Status:** ACTIVE — Presupuesto/día: $7.50 (gasto = 124.5% del presupuesto)
**Insight:** Se mantiene en 2 leads con CPL estable ($4.84→$4.67, -3.5%) — tercer cierre confirmado consecutivo dentro de meta desde el cambio de creativo, cada vez con más confianza estadística aunque el volumen sigue siendo bajo. Sigue siendo la campaña con mayor sobregasto de presupuesto de la cuenta (124.5%).

### 3. [[Pyme El salvador]] (SV) — Mejora fuerte pero sigue fuera de meta 🟡
```
CPL: $9.68 USD 🟡
Leads: 1
Gasto: $9.68 USD
Clicks: 20
CTR: 1.27% 🔴
CPC: $0.48 USD
CPM: $6.17 USD
Impresiones: 1,569
Reach: 1,209
```
**Status:** ACTIVE — Presupuesto/día: $12.50 (gasto = 77.4% del presupuesto)
**Insight:** Su CPL mejora de $15.29 a $9.68 (-36.7%), la mejor lectura confirmada de la campaña en varios cierres, pero sigue por encima del techo de meta ($6-7). Es la única de las tres campañas con leads que no logra entrar en meta hoy.

### 4. [[Beco]] (GT) — Colapsa a cero leads tras ser el mejor performer del cierre anterior 🔴
```
CPL: N/D (sin leads) 🔴
Leads: 0
Gasto: $9.47 USD
Clicks: 22
CTR: 0.88% 🔴
CPC: $0.43 USD
CPM: $3.79 USD
Impresiones: 2,499
Reach: 2,079
```
**Status:** ACTIVE — Presupuesto/día: $10.00 (gasto = 94.7% del presupuesto)
**Insight:** Ayer confirmado fue el mejor performer de toda la cuenta (4 leads, $3.02 CPL); hoy cierra en cero pese a gastar $9.47, sin ningún cambio manual en el activity log. Confirma la lectura casi-final de anoche y suma un nuevo giro abrupto al patrón de volatilidad ya documentado varias veces en esta campaña — amerita revisión dedicada de creativo, targeting o tracking de conversión.

### 5. [[Odoo Test]] (GT) — También cae a cero tras romper su racha de ceros ayer 🔴
```
CPL: N/D (sin leads) 🔴
Leads: 0
Gasto: $5.19 USD
Clicks: 7
CTR: 0.96% 🔴
CPC: $0.74 USD
CPM: $7.14 USD
Impresiones: 727
Reach: 580
```
**Status:** ACTIVE — Presupuesto/día: $4.93 (gasto = 105.3% del presupuesto)
**Insight:** Había roto su patrón recurrente de ceros el cierre anterior (2 leads, $3.25 CPL); hoy vuelve a cero, reforzando que su historial es de alta volatilidad más que de una tendencia sostenida en cualquier dirección.

### Campañas sin actividad (PAUSED, $0 gasto)
- Toma El control de tu pyme (USA)
- Accurate Partners - Loyalti - Nuevas Obligaciones - JUN 2026
- Conversión Clientes Potenciales - MX
- Conversión Clientes Potenciales - PY
- 🟡 CONVERSIÓN - CLIENTES POTENCIALES

## 🔄 Cambios de cuenta detectados (confirmado vía activity log)

- **Sin cambios manuales registrados.** El activity log de la cuenta para la ventana 2026-09-28 00:00 UTC – 2026-09-29 13:19 UTC contiene un único evento, automático: "Account billed" (facturación de Meta, 9/28 4:16 AM, actor "Meta"). Ninguna acción manual sobre presupuesto, targeting, creativo o estado de campañas.

## 💡 Insights Clave

- **El CPL de cuenta sube a $7.94 (+55.4% vs. 09-27), revirtiendo el mejor cierre confirmado documentado en el proyecto** — vuelve a estar fuera de la meta $6-7.
- **Los leads confirmados caen a la mitad: de 12 a 6 (-50.0%) mientras el gasto baja -22.4%** ($61.37 → $47.61) — el retroceso es casi enteramente de conversión a lead (Beco y Odoo Test a cero), no de menor inversión relativa.
- **Beco y Odoo Test cierran ambas en cero leads confirmados**, justo las dos campañas que el día anterior confirmado habían sido de las mejores de la cuenta (4 leads/$3.02 CPL y 2 leads/$3.25 CPL respectivamente) — sin ningún cambio manual que lo explique, es ya un patrón recurrente de saltos abruptos en ambas campañas que merece revisión dedicada de creativo, targeting o tracking de conversión.
- **CTR de cuenta cae a 1.32% (-15.9% vs. 09-27) y se mantiene por debajo de la meta 3-4%** en las 5 campañas activas, sin excepción.
- **Pyme Colombia es la única campaña que gasta sobre presupuesto (124.5%)**; Odoo Test también levemente sobre (105.3%), mientras Beco (94.7%) y Pyme El Salvador (77.4%) quedan por debajo de su presupuesto diario configurado.
- **Este cierre confirma, con un ajuste menor de gasto, la lectura casi-final documentada en [[Daily notes/2026-09-29 - Resumen del Dia]]:** CPL confirmado $7.94 vs. $7.74 casi-final, 6 leads en ambas lecturas, gasto $47.61 vs. $46.41 casi-final — la ventana de atribución no sumó leads adicionales tras el cierre, solo un ligero ajuste de gasto (+2.6%).
- **Pyme El Salvador mejora con fuerza (-36.7% de CPL) pero sigue siendo la única campaña con leads fuera de meta** — su recuperación no es aún suficiente para considerarla resuelta.

## ✅ Recomendaciones Accionables

- [ ] **Investigar a fondo el patrón de Beco y Odoo Test:** ambas pasaron de estar entre las mejores campañas de la cuenta el cierre anterior a cero leads confirmados hoy, sin cambio manual registrado en ninguna de las dos — con ya varios giros abruptos documentados entre las dos campañas, evaluar una revisión dedicada de creativo/targeting o del pixel/tracking de conversión antes de seguir asumiendo "volatilidad normal".
- [ ] **Dar seguimiento a Pyme El Salvador:** mejora fuerte hoy (-36.7% CPL) pero sigue siendo la única campaña con leads fuera de la meta $6-7 — confirmar si la mejora se sostiene en el próximo cierre antes de escalar presupuesto.
- [ ] **Ajustar el `daily_budget` de Pyme Colombia:** tercer cierre consecutivo sobre presupuesto (124.5% hoy) — considerar subirlo dado que su CPL se mantiene dentro de meta.
- [ ] **Retomar el A/B testing pendiente de los 5 nuevos copys** en "Toma El control de tu pyme" (GT), documentado en [[CLAUDE.md]] pero aún sin iniciar formalmente en esa campaña — sigue pendiente tras múltiples cierres consecutivos, pese a que "TestA/B Urgencia" es hoy el mejor performer confirmado de la cuenta.
- [ ] Monitorear de cerca el cierre de mañana: si el CPL blendeado vuelve a superar $7-8 con Beco/Odoo Test en cero por segunda vez consecutiva, escalar la investigación de tracking de leads más allá de creativo/targeting.
- [ ] **Usuario:** el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") sigue disparándose a las 23:50 GT en vez de después de medianoche — 18ª ocurrencia consecutiva confirmada vía `list_triggers` (cron sin cambios desde su creación el 2026-08-28), causando que sus notas en `Daily notes/` queden mal etiquetadas con los datos del día anterior. Solo se puede corregir manualmente desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ; ningún agente automatizado tiene permiso para editarlo.

## 🔗 Enlaces Relacionados

- [[Daily notes/2026-09-28 - Resumen del Día]] - Resumen ejecutivo confirmado del día generado por esta misma rutina
- [[Daily notes/2026-09-29 - Resumen del Dia]] - Lectura casi-final registrada anoche por la otra rutina automatizada (mal etiquetada como "09-29"), consistente con este cierre confirmado
- [[Reports/2026-09-27 - Reporte Performance]] - Reporte del día anterior
- [[CLAUDE.md]] - Meta de CPL $6-7 (fuera de meta hoy); A/B test de 5 copys mejorados pendiente de formalizar
- [[cloud.md]] - Dashboard principal

---
Generado por: Claude Code (Reporte Automatizado) + Meta Ads API
Cuenta: GT | Octopus Innovations (2530001557366648)
Fecha: 2026-09-28
Tags: #daily-note #performance #meta-ads #octopus
