---
date: 2026-09-29
aliases: [reporte-2026-09-29, performance-29-sep]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-09-29

> [!info] Datos de cierre confirmados
> Pull realizado la mañana del 2026-09-30 (rutina "Daily Meta Ads Performance Report - 7 AM Guatemala") con `date_preset=yesterday`, día ya cerrado completamente en horario de Guatemala (GMT-6). El total de cuenta a nivel `ad_account` cuadra con la suma de las 5 campañas activas (gasto $50.16 vs. $50.14 sumado, impresiones 7,784 vs. 7,783 sumado, clicks 115 exacto, CPL blendeado $12.54 = $50.16 / 4 leads confirmados). El alcance de cuenta (5,823) es menor que la suma simple por campaña (5,917) por solape normal de audiencias. El activity log de la cuenta para la ventana 2026-09-29 00:00 UTC – 2026-09-30 13:30 UTC no registra **ningún evento**, ni manual ni automático (ni siquiera la facturación automática de Meta que sí apareció en cierres previos).

> [!note] Sobre `Daily notes/2026-09-29 - Resumen del Dia.md`
> Ese archivo (sin acento en "Dia") fue creado por la rutina distinta "Daily Summary - 11:50 PM Guatemala" (`trig_01DMJfrsQXaTY5KJntXisDPQ`), que se dispara a las 23:50 GT — antes de medianoche — por lo que documenta en realidad datos casi-finales de **2026-09-29**, no de 2026-09-30 (bug de zona horaria documentado 19 veces consecutivas en el proyecto; se confirmó vía `list_triggers` que el cron sigue en `50 5 * * *` UTC sin cambios desde su creación el 2026-08-28 — **20ª ocurrencia consecutiva**). Este reporte confirma esa lectura casi-final (CPL $12.33 → $12.54, 4 leads en ambas lecturas, gasto $49.32 → $50.16) y genera además [[Daily notes/2026-09-29 - Resumen del Día]] **(con acento, archivo distinto)** como el resumen ejecutivo confirmado del día que pide esta rutina, sin sobrescribir la nota casi-final existente de la otra rutina.

## 📋 Resumen Ejecutivo

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| **CPL Promedio** | $12.54 USD | $6-7 | 🔴 Fuera de meta, +58.0% vs. 09-28 ($7.94) — peor cierre confirmado en varios días |
| **Gasto Total** | $50.16 USD | - | 🟡 +5.4% vs. 09-28 ($47.61) |
| **Leads Totales** | 4 | 4-5/día | 🟡 En el límite inferior de meta, -33.3% vs. 09-28 (6) |
| **CTR Promedio** | 1.48% | 3-4% | 🔴 Por debajo de meta (mejora +12.1% vs. 09-28: 1.32%, pero lejos del rango) |
| **CPC Promedio** | $0.44 USD | - | 🟢 -6.4% vs. 09-28 ($0.47) |
| **CPM Promedio** | $6.44 USD | - | 🔴 +4.4% vs. 09-28 ($6.17) |
| **Impresiones** | 7,784 | - | 🟢 +0.9% vs. 09-28 (7,711) |
| **Clicks** | 115 | - | 🟢 +12.7% vs. 09-28 (102) |
| **Alcance (Reach)** | 5,823 | - | 🟢 +0.4% vs. 09-28 (5,802) |
| **ROAS** | No aplica | - | Campañas Lead Gen sin tracking de valor de conversión |

**Nota:** El CPL de cuenta sube a $12.54 (+58.0% vs. 09-28), el peor cierre confirmado documentado en varios días y muy por encima de la meta $6-7. El deterioro combina gasto prácticamente estable (+5.4%) con una caída de leads de 6 a 4 (-33.3%). El movimiento más notable es un doble vuelco: **Toma El control de tu pyme** (GT) —la campaña ancla del proyecto— pasa de ser el mejor performer confirmado de ayer ($4.64 CPL, 3 leads) al peor entre las que sí generan leads hoy ($15.10 CPL, 1 lead); y **Pyme Colombia**, que llevaba tres cierres consecutivos dentro de meta con el creativo "Urgencia", cae a cero leads por primera vez en esa racha. En sentido contrario, Beco y Odoo Test —que ayer cerraron en cero— rebotan hoy con 1 lead cada una.

## 🎯 Performance por Campaña (Ranked por CPL)

### 1. [[Odoo Test]] (GT) — Mejor performer del día, rompe su patrón de ceros 🟢
```
CPL: $5.68 USD 🟢
Leads: 1
Gasto: $5.68 USD
Clicks: 14
CTR: 1.77% 🟡
CPC: $0.41 USD
CPM: $7.18 USD
Impresiones: 791
Reach: 569
```
**Status:** ACTIVE — Presupuesto/día: $4.93 (gasto = 115.2% del presupuesto)
**Insight:** Ayer confirmado cerró en cero leads; hoy recupera 1 lead a $5.68 CPL, dentro de meta y el mejor cierre de la cuenta. Suma un nuevo ciclo al patrón "cero → positivo" ya documentado varias veces en esta campaña, sin cambio manual que lo explique.

### 2. [[Beco]] (GT) — También rebota de cero a positivo 🟢
```
CPL: $9.08 USD 🟡
Leads: 1
Gasto: $9.08 USD
Clicks: 27
CTR: 1.25% 🔴
CPC: $0.34 USD
CPM: $4.20 USD
Impresiones: 2,161
Reach: 1,704
```
**Status:** ACTIVE — Presupuesto/día: $10.00 (gasto = 90.8% del presupuesto)
**Insight:** Igual que Odoo Test, recupera 1 lead tras cerrar ayer en cero, con gasto casi idéntico ($9.47 → $9.08, -4.1%). Ya son varios los ciclos de "cero → positivo → cero" documentados entre Beco y Odoo Test sin correlato en el activity log — el patrón sigue siendo demasiado recurrente para tratarlo solo como ruido.

### 3. [[Pyme El salvador]] (SV) — Retrocede tras su mejor cierre 🟡
```
CPL: $12.58 USD 🔴
Leads: 1
Gasto: $12.58 USD
Clicks: 34
CTR: 1.63% 🔴
CPC: $0.37 USD
CPM: $6.05 USD
Impresiones: 2,080
Reach: 1,541
```
**Status:** ACTIVE — Presupuesto/día: $12.50 (gasto = 100.6% del presupuesto)
**Insight:** Sube de $9.68 a $12.58 CPL (+30.0%) con el mismo gasto relativo (+30.0%) y mantiene 1 lead — pierde la mejora del cierre anterior y vuelve a ser, junto con Toma El control, de las más caras de la cuenta entre las que sí generan leads.

### 4. [[Toma El control de tu pyme]] (GT) — Colapsa tras ser el mejor performer confirmado del cierre anterior 🔴
```
CPL: $15.10 USD 🔴
Leads: 1
Gasto: $15.10 USD
Clicks: 34
CTR: 1.56% 🔴
CPC: $0.44 USD
CPM: $6.95 USD
Impresiones: 2,173
Reach: 1,652
```
**Status:** ACTIVE — Presupuesto del único ad set activo ("TestA/B Urgencia"): $15.00 (gasto = 100.7% del presupuesto)
**Insight:** Es la campaña ancla del proyecto (foco del A/B test de 5 copys pendiente en [[CLAUDE.md]]) y hoy sufre su peor cierre confirmado: pasa de $4.64 CPL con 3 leads a $15.10 CPL con solo 1 lead (+225.4% de CPL, -66.7% de leads), con gasto prácticamente igual (+8.4%). Sin ningún cambio manual registrado en el activity log. El A/B test de copys sigue sin iniciarse formalmente — "TestA/B Urgencia" continúa siendo el único ad set activo.

### 5. [[Pyme Colombia]] (COL) — Rompe su racha positiva, cae a cero leads 🔴
```
CPL: N/D (sin leads) 🔴
Leads: 0
Gasto: $7.70 USD
Clicks: 6
CTR: 1.04% 🔴
CPC: $1.28 USD
CPM: $13.32 USD
Impresiones: 578
Reach: 451
```
**Status:** ACTIVE — Presupuesto/día: $7.50 (gasto = 102.7% del presupuesto)
**Insight:** Llevaba tres cierres confirmados consecutivos dentro de meta con el creativo "Urgencia" (último: $4.67 CPL, 2 leads); hoy cierra en cero pese a gastar $7.70 (-17.6% vs. ayer), con CTR también más bajo (1.04% vs. 2.04%). Sin cambio manual registrado que lo explique — junto con el colapso de "Toma El control", es la señal más relevante del día.

### Campañas sin actividad (PAUSED, $0 gasto)
- Toma El control de tu pyme (USA)
- Accurate Partners - Loyalti - Nuevas Obligaciones - JUN 2026
- Conversión Clientes Potenciales - MX
- Conversión Clientes Potenciales - PY
- 🟡 CONVERSIÓN - CLIENTES POTENCIALES

## 🔄 Cambios de cuenta detectados (confirmado vía activity log)

- **Sin cambios registrados de ningún tipo.** El activity log de la cuenta para la ventana 2026-09-29 00:00 UTC – 2026-09-30 13:30 UTC devuelve cero eventos: ni cambios manuales de presupuesto, targeting, creativo o estado de campañas, ni siquiera el evento automático de facturación de Meta que sí apareció en cierres anteriores.

## 💡 Insights Clave

- **El CPL de cuenta sube a $12.54 (+58.0% vs. 09-28), el peor cierre confirmado documentado en varios días** — se aleja aún más de la meta $6-7.
- **Los leads confirmados caen de 6 a 4 (-33.3%) con gasto prácticamente estable** ($47.61 → $50.16, +5.4%) — el deterioro es de conversión a lead, no de menor inversión.
- **Doble vuelco simultáneo en las dos campañas más estables del cierre anterior:** "Toma El control de tu pyme" (GT) pasa de mejor performer confirmado ($4.64 CPL, 3 leads) a peor campaña con leads ($15.10 CPL, 1 lead); Pyme Colombia rompe su racha de tres cierres dentro de meta y cae a cero leads. Ninguna tiene cambio manual que lo explique en el activity log — apunta a volatilidad de auction/audiencia, pero dado que "Toma El control" es la campaña ancla del proyecto, merece verificación adicional de pixel/tracking antes de descartar causas operativas.
- **Beco y Odoo Test rebotan de cero a positivo**, sumando ya varios ciclos de "cero → positivo → cero" sin correlato en el activity log — el patrón es demasiado recurrente para seguir tratándolo solo como ruido de subasta.
- **CTR de cuenta mejora ligeramente a 1.48% (+12.1% vs. 09-28) pero se mantiene muy por debajo de la meta 3-4%** en las 5 campañas activas, sin excepción.
- **Todas las campañas activas cierran cerca o levemente sobre su presupuesto diario configurado** (rango 90.8%–115.2%), sin sobregasto extremo como en cierres anteriores.
- **Este cierre confirma, con un ajuste menor de gasto, la lectura casi-final documentada en [[Daily notes/2026-09-29 - Resumen del Dia]]:** CPL confirmado $12.54 vs. $12.33 casi-final, 4 leads en ambas lecturas, gasto $50.16 vs. $49.32 casi-final — la ventana de atribución no sumó leads adicionales, solo un ligero ajuste de gasto (+1.7%).

## ✅ Recomendaciones Accionables

- [ ] **Investigar a fondo el colapso de "Toma El control de tu pyme" (GT):** es la campaña ancla del proyecto y hoy registra su peor cierre confirmado (+225.4% de CPL) justo cuando venía de ser el mejor performer — descartar causas operativas (pixel, tracking de leads, ventana de atribución) antes de asumir solo volatilidad normal, y priorizar el A/B test de 5 copys pendiente en [[CLAUDE.md]] sobre esta misma campaña.
- [ ] **Dar seguimiento a Pyme Colombia:** rompió hoy una racha de tres cierres confirmados dentro de meta con el creativo "Urgencia" — confirmar si es un evento aislado o el inicio de una tendencia antes del próximo ajuste de presupuesto.
- [ ] **Continuar documentando el patrón de Beco y Odoo Test:** ya van varios ciclos de "cero → positivo" sin correlato en el activity log — evaluar si amerita una revisión de creativo/targeting dedicada en vez de seguir monitoreando pasivamente.
- [ ] **Retomar el A/B testing pendiente de los 5 nuevos copys** en "Toma El control de tu pyme" (GT), documentado en [[CLAUDE.md]] pero aún sin iniciar formalmente — cobra más urgencia dado el colapso de hoy en esa misma campaña.
- [ ] Monitorear el cierre de mañana: si "Toma El control" y Pyme Colombia no se recuperan y el CPL blendeado se mantiene sobre $10-12, escalar la investigación de tracking de leads más allá de creativo/targeting.
- [ ] **Usuario:** el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") sigue disparándose a las 23:50 GT en vez de después de medianoche — **20ª ocurrencia consecutiva** confirmada vía `list_triggers` (cron sin cambios desde su creación el 2026-08-28), causando que sus notas en `Daily notes/` queden mal etiquetadas con los datos del día anterior. Solo se puede corregir manualmente desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ; ningún agente automatizado tiene permiso para editarlo.

## 🔗 Enlaces Relacionados

- [[Daily notes/2026-09-29 - Resumen del Día]] - Resumen ejecutivo confirmado del día generado por esta misma rutina
- [[Daily notes/2026-09-29 - Resumen del Dia]] - Lectura casi-final registrada anoche por la otra rutina automatizada (mal etiquetada como "09-30" en su ejecución), consistente con este cierre confirmado
- [[Reports/2026-09-28 - Reporte Performance]] - Reporte del día anterior
- [[CLAUDE.md]] - Meta de CPL $6-7 (fuera de meta hoy); A/B test de 5 copys mejorados pendiente de formalizar en la campaña que hoy colapsó
- [[cloud.md]] - Dashboard principal

---
Generado por: Claude Code (Reporte Automatizado) + Meta Ads API
Cuenta: GT | Octopus Innovations (2530001557366648)
Fecha: 2026-09-29
Tags: #daily-note #performance #meta-ads #octopus
