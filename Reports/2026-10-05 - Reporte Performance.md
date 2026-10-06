---
date: 2026-10-05
aliases: [reporte-2026-10-05, performance-05-oct]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-10-05

> [!info] Datos de cierre confirmados
> Pull realizado la mañana del 2026-10-06 (rutina "Daily Meta Ads Performance Report - 7 AM Guatemala") con rango explícito 2026-10-05 a 2026-10-05, día ya cerrado completamente en horario de Guatemala (GMT-6). El total de cuenta a nivel `ad_account` cuadra exactamente con la suma de las 5 campañas activas (gasto $50.92, impresiones 8,371 y clicks 124, todos coinciden exacto con la suma por campaña). El alcance de cuenta (6,582) es menor que la suma simple por campaña (6,563 — nota: en este caso la suma simple queda incluso por debajo del total de cuenta por el redondeo de reach individual, diferencia mínima). El activity log de la cuenta para la ventana 2026-10-05 06:00–2026-10-06 06:00 UTC no registra ningún evento.

> [!note] Sobre `Daily notes/2026-10-06 - Resumen del Dia.md`
> Ese archivo (sin acento) fue creado por la rutina distinta "Daily Summary - 11:50 PM Guatemala" (`trig_01DMJfrsQXaTY5KJntXisDPQ`), que se dispara a las 23:50 GT — antes de medianoche — por lo que documenta en realidad datos casi-finales de **2026-10-05** (el día que confirma este reporte), mal etiquetados como "10-06". Esa lectura casi-final ya anticipaba la recuperación de "Toma El control de tu pyme" confirmada aquí: CPL $7.89 (casi-final) → $8.01 (confirmado), 2 leads en ambas lecturas; Pyme El Salvador $13.55 → $13.65, 1 lead en ambas; Beco, Pyme Colombia y Odoo Test se confirman en 0 leads cada una. Este reporte genera además [[Daily notes/2026-10-05 - Resumen del Día]] **(con acento, archivo distinto)** como el resumen ejecutivo confirmado del día, sin sobrescribir la nota casi-final existente de la otra rutina.

## 📋 Resumen Ejecutivo

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| **CPL Promedio** | $16.97 USD | $6-7 | 🔴 +142.4% vs. meta; empeora +53.9% vs. el cierre confirmado de 10-04 ($11.03) |
| **Gasto Total** | $50.92 USD | - | 🟢 -7.7% vs. 10-04 ($55.16) |
| **Leads Totales** | 3 | 4-5/día | 🔴 Por debajo de meta, -40.0% vs. 10-04 (5) |
| **CTR Promedio** | 1.48% | 3-4% | 🔴 Por debajo de meta, pero mejora +5.7% vs. 10-04 (1.40%) |
| **CPC Promedio** | $0.41 USD | - | 🟢 -4.7% vs. 10-04 ($0.43) |
| **CPM Promedio** | $6.08 USD | - | ⚪ Sin cambio vs. 10-04 ($6.08) |
| **Impresiones** | 8,371 | - | 🔻 -7.7% vs. 10-04 (9,070) |
| **Clicks** | 124 | - | 🔻 -2.4% vs. 10-04 (127) |
| **Alcance (Reach)** | 6,582 | - | 🔻 -1.7% vs. 10-04 (6,696) |
| **ROAS** | No aplica | - | Campañas Lead Gen sin tracking de valor de conversión |

**Nota:** El CPL blendeado empeora +53.9% y se aleja más de la meta $6-7 (+142.4%), pero el deterioro está concentrado enteramente en la caída a cero leads de **Beco**, **Pyme Colombia** y **Odoo Test** — las tres cierran hoy sin ningún lead, el primer día en la serie documentada (desde 10-01) con tres campañas simultáneamente en cero. En contraste, **Toma El control de tu pyme**, la campaña ancla del proyecto, se recupera con fuerza: pasa de su segundo peor cierre confirmado de la serie ayer ($16.36 CPL, 1 lead) a liderar hoy la cuenta con **$8.01 CPL y 2 leads**, su mejor resultado confirmado desde el 10-03 ($6.59). **Pyme El Salvador** se mantiene prácticamente estable y sigue siendo la única otra campaña con lead ($13.65 CPL, +20.4% leads constante). El gasto total cae -7.7% mientras los leads caen -40.0%: la cuenta gasta menos pero convierte mucho peor.

## 🎯 Performance por Campaña (Ranked por CPL)

### 1. [[Toma El control de tu pyme]] (GT) — Revierte por completo el cierre de ayer y lidera la cuenta 🟢
```
CPL: $8.01 USD 🟡
Leads: 2
Gasto: $16.02 USD
Clicks: 50
CTR: 1.96% 🔴
CPC: $0.32 USD
CPM: $6.27 USD
Impresiones: 2,554
Reach: 2,106
```
**Status:** ACTIVE — Presupuesto del único ad set activo: N/D a nivel campaña (gasto = $16.02)
**Insight:** Es la campaña ancla del proyecto (CPL original $9.29). Un día después de su segundo peor cierre confirmado de la serie ($16.36, 1 lead), se recupera con fuerza: **CPL $8.01 con 2 leads** — su mejor resultado confirmado desde el $6.59 del 10-03, y hoy la campaña líder de toda la cuenta en vez de la peor. El gasto cae -2.1% pero duplica sus leads (1→2), y el CTR mejora +36.1% (1.44%→1.96%). Es la cuarta oscilación extrema en cuatro días ($17.50 → $6.59 → $16.36 → $8.01), sin ningún cambio manual registrado en el activity log. El A/B test de los 5 copys documentado en [[CLAUDE.md]] sigue sin iniciarse formalmente; esta volatilidad refuerza la urgencia de lanzarlo para intentar estabilizarla en el lado bueno.

### 2. [[Pyme El salvador]] (SV) — Se mantiene estable, continúa fuera de meta 🔴
```
CPL: $13.65 USD 🔴
Leads: 1
Gasto: $13.65 USD
Clicks: 25
CTR: 1.10% 🔴
CPC: $0.55 USD
CPM: $6.01 USD
Impresiones: 2,273
Reach: 1,632
```
**Status:** ACTIVE — Presupuesto/día: $12.50 (gasto = 109.2% del presupuesto)
**Insight:** Prácticamente igual al cierre confirmado de ayer ($13.80, -1.1%), manteniendo 1 lead. Su CTR sigue débil (1.61%→1.10%, -31.7%) — la única campaña con lead que no mejora hoy, mientras el resto de la cuenta o se recupera fuerte (Toma El control) o cae a cero (Beco, Colombia, Odoo Test).

### 3-5. Beco, Pyme Colombia y Odoo Test — Las tres caen a cero leads simultáneamente 🔴
Sin CPL calculable (0 leads). Orden por gasto:

**[[Beco]] (GT)**
```
Leads: 0
Gasto: $8.43 USD
Clicks: 27
CTR: 1.44% 🔴
CPC: $0.31 USD
CPM: $4.48 USD
Impresiones: 1,880
Reach: 1,462
```
Status: ACTIVE — Presupuesto/día: $10.00 (gasto = 84.3% del presupuesto, por debajo por primera vez en varios cierres)

**[[Pyme Colombia]] (COL)**
```
Leads: 0
Gasto: $7.86 USD
Clicks: 14
CTR: 2.17% 🟢
CPC: $0.56 USD
CPM: $12.20 USD
Impresiones: 644
Reach: 497
```
Status: ACTIVE — Presupuesto/día: $7.50 (gasto = 104.8% del presupuesto)

**[[Odoo Test]] (GT)**
```
Leads: 0
Gasto: $4.96 USD
Clicks: 8
CTR: 0.78% 🔴
CPC: $0.62 USD
CPM: $4.86 USD
Impresiones: 1,020
Reach: 866
```
Status: ACTIVE — Presupuesto/día: $4.93 (gasto = 100.6% del presupuesto)

**Insight conjunto:** Es la primera vez en la ventana documentada (10-01 a la fecha) que tres campañas activas quedan simultáneamente sin ningún lead en el mismo día — hasta ahora, como mucho una campaña por día caía a cero. Pyme Colombia llevaba varios días consecutivos con 1 lead/día estable; Beco venía de una racha similar; Odoo Test había roto apenas el 10-03 una racha de dos ceros con su mejor CPL de la cuenta ($5.24/$5.31) y hoy vuelve a cero. Ninguna de las tres muestra un cambio manual en el activity log que explique la caída; el CTR de Pyme Colombia incluso mejora (2.17%, el mejor de la cuenta hoy), reforzando que es un problema de conversión a lead puntual y no de calidad del tráfico.

### Campañas sin actividad (PAUSED, $0 gasto)
- Toma El control de tu pyme (USA)
- Accurate Partners - Loyalti - Nuevas Obligaciones - JUN 2026
- Conversión Clientes Potenciales - MX
- Conversión Clientes Potenciales - PY
- 🟡 CONVERSIÓN - CLIENTES POTENCIALES

## 🔄 Cambios de cuenta detectados (confirmado vía activity log)

- **Cero eventos registrados.** El activity log de la cuenta para la ventana 2026-10-05 06:00–2026-10-06 06:00 UTC no registra ningún evento, ni manual ni automático. Tanto la fuerte recuperación de "Toma El control" como la caída simultánea a cero de las otras tres campañas activas siguen sin ningún correlato de cambio registrado en la cuenta — apunta a volatilidad normal de subasta/entrega/atribución en una cuenta de bajo volumen, no a una intervención del usuario o del sistema.

## 💡 Insights Clave

- **El CPL de cuenta sube +53.9% a $16.97** — el peor cierre confirmado de toda la serie documentada, pero el número es engañoso: está inflado enteramente por la caída a cero leads de tres campañas, no por un deterioro generalizado (la campaña con más leads, Toma El control, de hecho mejora con fuerza).
- **Los leads confirmados caen -40.0% a 3** (vs. 5 en los dos cierres anteriores) — la cifra más baja de la serie reciente.
- **El gasto total cae -7.7% a $50.92** mientras los leads caen -40.0% — la cuenta gasta menos y convierte mucho peor, la combinación más desfavorable posible.
- **Solo 2 de 5 campañas activas generan al menos 1 lead hoy** (Toma El control y Pyme El Salvador) — la peor composición confirmada de la serie; ayer era 1 de 5 (solo Odoo Test).
- **La jerarquía de campañas se invierte por completo**: "Toma El control de tu pyme", que fue la peor o segunda peor campaña en 3 de los últimos 4 cierres, es hoy la única con buen CPL relativo y el doble de leads que cualquier otra — mientras tres campañas que venían siendo las más estables (1 lead/día sin falta) caen a cero.
- **CTR blendeado mejora a 1.48% (+5.7% vs. 1.40% de ayer)** y CPC baja a $0.41 (-4.7%), con CPM plano en $6.08 — la subasta no se encareció hoy; el deterioro del CPL blendeado es puramente un problema de conversión a lead concentrado en 3 campañas puntuales, no de costos de medios.
- **Solo 2 de 4 campañas con `daily_budget` configurado sobrepasan su presupuesto hoy** (Pyme Colombia 104.8%, Pyme El Salvador 109.2%), mientras Odoo Test cierra prácticamente exacto (100.6%) y **Beco queda claramente por debajo (84.3%)** — rompe la racha de sobrepaso generalizado de cierres anteriores.
- **Sexta ventana consecutiva sin ningún evento en el activity log** — ni la recuperación de Toma El control ni la caída simultánea a cero de las otras tres campañas tienen un correlato de cambio registrado en la cuenta.
- **Este cierre confirma, con un ajuste menor, la lectura casi-final documentada en [[Daily notes/2026-10-06 - Resumen del Dia]]:** CPL confirmado $16.97 vs. $16.73 casi-final, 3 leads en ambas lecturas, gasto $50.92 vs. $50.19 casi-final (+1.5%).

## ✅ Recomendaciones Accionables

- [ ] **Investigar la caída simultánea a cero leads de Pyme Colombia, Beco y Odoo Test** — evento sin precedente en la serie documentada (10-01 a la fecha); ninguna tiene cambio manual registrado. Confirmar en el próximo cierre si es volatilidad puntual de subasta/atribución o el inicio de un problema real (fatiga de audiencia, aprendizaje del algoritmo).
- [ ] **Dar seguimiento a si "Toma El control de tu pyme" sostiene su recuperación** ($8.01 CPL, 2 leads) o si continúa su patrón de oscilación extrema (cuatro cambios de polaridad en cuatro días); lanzar por fin el A/B testing de los 5 copys documentado en [[CLAUDE.md]] desde el 2026-08-24 para intentar estabilizarla en el lado bueno en vez de seguir monitoreando pasivamente.
- [ ] **Revisar si Pyme El Salvador necesita un ajuste de creativo o targeting** — es la única campaña con lead que no mejora hoy y lleva varios días fuera de meta con CTR débil.
- [ ] **Confirmar si Beco sostiene su gasto por debajo del presupuesto (84.3%)** en el próximo cierre, o si fue puntual del día de cero leads.
- [ ] **Usuario:** el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") sigue disparándose a las 23:50 GT en vez de después de medianoche, causando que sus notas en `Daily notes/` queden mal etiquetadas con los datos del día anterior (ver [[Daily notes/2026-10-06 - Resumen del Dia]]). Solo se puede corregir manualmente desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ; ningún agente automatizado tiene permiso para editarlo.

## 🔗 Enlaces Relacionados

- [[Daily notes/2026-10-05 - Resumen del Día]] - Resumen ejecutivo confirmado del día generado por esta misma rutina
- [[Daily notes/2026-10-06 - Resumen del Dia]] - Lectura casi-final registrada anoche por la otra rutina automatizada (mal etiquetada como "10-06"), consistente con este cierre confirmado
- [[Reports/2026-10-04 - Reporte Performance]] - Reporte del día anterior
- [[CLAUDE.md]] - Meta de CPL $6-7 (fuera de meta, +142.4%); A/B test de 5 copys mejorados pendiente de formalizar en "Toma El control de tu pyme", urgencia reforzada tras cuarta oscilación extrema en cuatro días
- [[cloud.md]] - Dashboard principal

---
Generado por: Claude Code (Reporte Automatizado) + Meta Ads API
Cuenta: GT | Octopus Innovations (2530001557366648)
Fecha: 2026-10-05
Tags: #daily-note #performance #meta-ads #octopus
