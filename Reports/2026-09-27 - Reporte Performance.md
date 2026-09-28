---
date: 2026-09-27
aliases: [reporte-2026-09-27, performance-27-sep]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-09-27

> [!info] Datos de cierre confirmados
> Pull realizado la mañana del 2026-09-28 (rutina "Daily Meta Ads Performance Report - 7 AM Guatemala") con `time_range` explícito (`2026-09-27` a `2026-09-27`), día ya cerrado completamente en horario de Guatemala (GMT-6). El total de cuenta a nivel `ad_account` cuadra exactamente con la suma de las 5 campañas activas (gasto $61.37, impresiones 9,367, clicks 147, reach 7,086, y CPL blendeado $5.11 = $61.37 / 12 leads confirmados). El activity log de la cuenta para la ventana 2026-09-27 00:00 UTC – 2026-09-28 06:00 UTC está **vacío** — sin cambios manuales registrados.

> [!note] Sobre `Daily notes/2026-09-27 - Resumen del Dia.md`
> Ese archivo (sin acento en "Dia") fue creado por la rutina distinta "Daily Summary - 11:50 PM Guatemala" (`trig_01DMJfrsQXaTY5KJntXisDPQ`), que se dispara a las 23:50 GT — antes de medianoche — por lo que documenta en realidad datos casi-finales de **2026-09-26**, no de 2026-09-27 (bug de zona horaria ya documentado en el proyecto). La lectura casi-final que sí corresponde a 2026-09-27 quedó guardada, por el mismo bug, bajo [[Daily notes/2026-09-28 - Resumen del Dia]]. Este reporte confirma esa lectura casi-final ($5.05 CPL, 12 leads, $60.54 gasto → $5.11 CPL, 12 leads, $61.37 gasto confirmados) y genera además [[Daily notes/2026-09-27 - Resumen del Día]] **(con acento, archivo distinto)** como el resumen ejecutivo confirmado del día que pide esta rutina, sin sobrescribir la nota casi-final existente de la otra rutina.

## 📋 Resumen Ejecutivo

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| **CPL Promedio** | $5.11 USD | $6-7 | 🟢 Dentro (y por debajo) de la meta por primera vez en varios cierres — -66.3% vs. 09-26 ($15.18) |
| **Gasto Total** | $61.37 USD | - | 🔺 +34.8% vs. 09-26 ($45.53) |
| **Leads Totales** | 12 | 4-5/día | 🟢 Más del doble de la meta, +300.0% vs. 09-26 (3) |
| **CTR Promedio** | 1.57% | 3-4% | 🔴 Por debajo de meta, pero +20.8% vs. 09-26 (1.30%) |
| **CPC Promedio** | $0.42 USD | - | 🟢 -17.6% vs. 09-26 ($0.51) |
| **CPM Promedio** | $6.55 USD | - | 🟢 -0.8% vs. 09-26 ($6.60) |
| **Impresiones** | 9,367 | - | 🔺 +35.8% vs. 09-26 (6,897) |
| **Clicks** | 147 | - | 🔺 +63.3% vs. 09-26 (90) |
| **Alcance (Reach)** | 7,086 | - | 🔺 +31.4% vs. 09-26 (5,393) |
| **ROAS** | No aplica | - | Campañas Lead Gen sin tracking de valor de conversión |

**Nota:** El CPL de cuenta cae a $5.11 (-66.3% vs. 09-26), el mejor cierre confirmado documentado en el proyecto hasta ahora y, por primera vez, dentro (de hecho por debajo) de la meta $6-7. La mejora es sobre todo de conversión: los leads confirmados se cuadruplican (3→12, +300%) mientras el gasto sube solo +34.8%. Las 5 campañas activas cierran con leads — ninguna en cero — algo que no ocurría en los cierres recientes. Todas gastaron por encima de su presupuesto diario configurado (119%-132%).

## 🎯 Performance por Campaña (Ranked por CPL)

### 1. [[Beco]] (GT) — Resucita: de cero leads el cierre anterior a mejor performer del día 🟢
```
CPL: $3.02 USD 🟢
Leads: 4
Gasto: $12.06 USD
Clicks: 55
CTR: 1.99%
CPC: $0.22 USD
CPM: $4.37 USD
Impresiones: 2,762
Reach: 2,191
```
**Status:** ACTIVE — Presupuesto/día: $10.00 (gasto = 120.6% del presupuesto)
**Insight:** Repite el patrón de saltos abruptos sin cambio manual registrado que ya se documentó antes: el cierre anterior colapsó de mejor performer a cero leads, hoy vuelve a ser el mejor performer de la cuenta.

### 2. [[Odoo Test]] (GT) — Rompe su patrón recurrente de ceros 🟢
```
CPL: $3.25 USD 🟢
Leads: 2
Gasto: $6.50 USD
Clicks: 20
CTR: 2.55%
CPC: $0.33 USD
CPM: $8.28 USD
Impresiones: 785
Reach: 609
```
**Status:** ACTIVE — Presupuesto/día: $4.93 (gasto = 131.8% del presupuesto)
**Insight:** Tras cerrar en cero en 4 de los últimos 6 cierres confirmados, logra hoy 2 leads a $3.25 CPL — su mejor cierre confirmado hasta ahora.

### 3. [[Pyme Colombia]] (COL) — Recupera y duplica su lead con el creativo "Urgencia" 🟢
```
CPL: $4.84 USD 🟢
Leads: 2
Gasto: $9.67 USD
Clicks: 18
CTR: 2.82%
CPC: $0.54 USD
CPM: $15.13 USD
Impresiones: 639
Reach: 459
```
**Status:** ACTIVE — Presupuesto/día: $7.50 (gasto = 128.9% del presupuesto)
**Insight:** Había perdido su único lead en el cierre anterior; hoy duplica esa cifra y entra dentro de la meta de CPL — segunda muestra positiva para el creativo "Urgencia", aún insuficiente para concluir con confianza.

### 4. [[Toma El control de tu pyme]] (GT) — Sube a 3 leads y mejora su CPL 🟢
```
CPL: $5.95 USD 🟢
Leads: 3
Gasto: $17.85 USD
Clicks: 30
CTR: 1.05%
CPC: $0.60 USD
CPM: $6.27 USD
Impresiones: 2,845
Reach: 2,227
```
**Status:** ACTIVE — Presupuesto del único ad set activo ("TestA/B Urgencia"): $15.00 (gasto = 119.0% del presupuesto)
**Insight:** Sube de 2 a 3 leads y su CPL mejora de $6.38 a $5.95 (-6.7%) — sigue siendo la campaña de mayor gasto de la cuenta, y su CTR (1.05%) continúa siendo el más bajo entre las activas. El A/B test de 5 copys nuevos documentado en [[CLAUDE.md]] sigue sin iniciarse formalmente; "TestA/B Urgencia" es el único ad set activo.

### 5. [[Pyme El salvador]] (SV) — Única campaña fuera de meta, y empeora 🔴
```
CPL: $15.29 USD 🔴
Leads: 1
Gasto: $15.29 USD
Clicks: 24
CTR: 1.03%
CPC: $0.64 USD
CPM: $6.55 USD
Impresiones: 2,336
Reach: 1,806
```
**Status:** ACTIVE — Presupuesto/día: $12.50 (gasto = 122.3% del presupuesto)
**Insight:** Se mantiene en 1 lead pero su CPL sube de $12.92 a $15.29 (+18.3%) — es la única campaña activa que no mejora hoy y ahora tiene, con amplio margen, el peor CPL de la cuenta.

### Campañas sin actividad (PAUSED, $0 gasto)
- Toma El control de tu pyme (USA)
- Accurate Partners - Loyalti - Nuevas Obligaciones - JUN 2026
- Conversión Clientes Potenciales - MX
- Conversión Clientes Potenciales - PY
- 🟡 CONVERSIÓN - CLIENTES POTENCIALES

## 🔄 Cambios de cuenta detectados (confirmado vía activity log)

- **Sin cambios manuales registrados.** El activity log de la cuenta para la ventana 2026-09-27 00:00 UTC – 2026-09-28 06:00 UTC está vacío — igual que el cierre anterior, ninguna acción manual sobre presupuesto, targeting, creativo o estado de campañas.

## 💡 Insights Clave

- **El CPL de cuenta cae a $5.11 (-66.3% vs. 09-26), el mejor cierre confirmado documentado en el proyecto** — por primera vez dentro (y por debajo) de la meta $6-7.
- **Los leads confirmados se cuadruplican: de 3 a 12 (+300%) con un gasto que sube solo +34.8%** ($45.53 → $61.37) — la mejora es casi enteramente de conversión a lead, no de mayor inversión.
- **Las 5 campañas activas cierran con leads por primera vez en varios cierres consecutivos** — contrasta directamente con el cierre anterior, donde 3 de 5 cerraron en cero.
- **CTR de cuenta sube a 1.57% (+20.8% vs. 09-26) pero se mantiene por debajo de la meta 3-4%** — mejora, pero el problema de conversión click→lead a nivel de cuenta sigue sin resolverse estructuralmente.
- **Todas las campañas activas gastaron por encima de su presupuesto diario configurado** (119.0%-131.8%), consistente con el comportamiento normal de entrega de Meta que permite sobregasto diario compensado en otros días.
- **Sin ningún cambio manual registrado en el activity log** — la mejora tan marcada no está asociada a ninguna acción operativa visible; refuerza la hipótesis, ya anotada en cierres previos, de volatilidad normal de subasta/audiencia en una cuenta de bajo volumen (o de optimización automática de Meta).
- **Este cierre confirma, con variaciones mínimas, la lectura casi-final documentada en [[Daily notes/2026-09-28 - Resumen del Dia]]:** CPL confirmado $5.11 vs. $5.05 casi-final, 12 leads en ambas lecturas, gasto $61.37 vs. $60.54 casi-final — la ventana de atribución no sumó leads adicionales tras el cierre, solo un ligero ajuste de gasto (+1.4%).
- **Pyme El Salvador es ahora la única campaña activa fuera de meta**, y su CPL sigue empeorando (+18.3% vs. 09-26) mientras el resto de la cuenta mejora — requiere atención específica de creativo/targeting.

## ✅ Recomendaciones Accionables

- [ ] **Dar seguimiento a Pyme El Salvador:** única campaña activa fuera de meta hoy, con CPL empeorando dos cierres consecutivos ($12.92→$15.29) — evaluar creativo/targeting específico de esta campaña antes de escalar su presupuesto.
- [ ] **Investigar el patrón de saltos abruptos de Beco** (cero leads→mejor performer en 24h, sin cambio manual registrado) y de **Odoo Test** (rompe racha de ceros) — evaluar si es volatilidad normal de bajo volumen antes de intervenir el creativo.
- [ ] **Retomar el A/B testing pendiente de los 5 nuevos copys** en "Toma El control de tu pyme" (GT), documentado en [[CLAUDE.md]] pero aún sin iniciar formalmente en esa campaña — sigue pendiente tras múltiples cierres consecutivos.
- [ ] **Revisar el `daily_budget`** de las 5 campañas activas: todas cierran sobre presupuesto (Odoo Test 131.8%, Pyme Colombia 128.9%, Pyme El Salvador 122.3%, Beco 120.6%, TestA/B Urgencia 119.0%) — considerar ajustar presupuestos al alza dado que el CPL blendeado ahora está dentro de meta.
- [ ] Documentar en [[CLAUDE.md]] la actualización de meta CPL: el objetivo original era bajar de $9.29 a $6-7; el cierre de hoy ($5.11) ya supera ese objetivo — reevaluar si la meta debe ajustarse a la baja.
- [ ] **Usuario:** el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") sigue disparándose a las 23:50 GT en vez de después de medianoche — 17ª ocurrencia consecutiva documentada, causando que sus notas en `Daily notes/` queden mal etiquetadas con los datos del día anterior. Solo se puede corregir manualmente desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ; ningún agente automatizado tiene permiso para editarlo.

## 🔗 Enlaces Relacionados

- [[Daily notes/2026-09-27 - Resumen del Día]] - Resumen ejecutivo confirmado del día generado por esta misma rutina
- [[Daily notes/2026-09-28 - Resumen del Dia]] - Lectura casi-final registrada anoche por la otra rutina automatizada (mal etiquetada como "09-28"), consistente con este cierre confirmado
- [[Reports/2026-09-26 - Reporte Performance]] - Reporte del día anterior
- [[CLAUDE.md]] - Meta de CPL $6-7 (superada hoy); A/B test de 5 copys mejorados pendiente de formalizar
- [[cloud.md]] - Dashboard principal

---
Generado por: Claude Code (Reporte Automatizado) + Meta Ads API
Cuenta: GT | Octopus Innovations (2530001557366648)
Fecha: 2026-09-27
Tags: #daily-note #performance #meta-ads #octopus
