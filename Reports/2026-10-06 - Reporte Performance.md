---
date: 2026-10-06
aliases: [reporte-2026-10-06, performance-06-oct]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-10-06

> [!info] Datos de cierre confirmados
> Pull realizado la mañana del 2026-10-07 (rutina "Daily Meta Ads Performance Report - 7 AM Guatemala") con rango explícito 2026-10-06 a 2026-10-06, día ya cerrado completamente en horario de Guatemala (GMT-6). El total de cuenta a nivel `ad_account` cuadra exactamente con la suma de las 5 campañas activas (gasto $46.06, impresiones 7,167 y clicks 123, todos coinciden exacto con la suma por campaña). El alcance de cuenta (5,489) es menor que la suma simple por campaña (5,658) por solapamiento normal de audiencias entre campañas activas. El activity log de la cuenta para la ventana 2026-10-06 06:00–2026-10-07 06:00 UTC no registra ningún evento.

> [!note] Sobre `Daily notes/2026-10-07 - Resumen del Dia.md`
> Ese archivo (sin acento) fue creado por la rutina distinta "Daily Summary - 11:50 PM Guatemala" (`trig_01DMJfrsQXaTY5KJntXisDPQ`), que se dispara a las 23:50 GT — antes de medianoche, confirmado vía `list_triggers` (cron `50 5 * * *` UTC, sin cambios desde el 2026-08-28) — por lo que documenta en realidad datos casi-finales de **2026-10-06** (el día que confirma este reporte), mal etiquetados como "10-07". Esa lectura casi-final ya anticipaba correctamente la recuperación simultánea de Pyme Colombia, Beco y Odoo Test, y el desplome a cero leads de "Toma El control de tu pyme": CPL blendeado $7.58 casi-final → $7.68 confirmado, 6 leads en ambas lecturas; Pyme Colombia $2.49 → $2.50 (3 leads en ambas); Pyme El Salvador $10.53 → $10.70 (1 lead en ambas); Beco $9.80 → $10.04 (1 lead en ambas); Odoo Test $4.72 → $4.72 (exacto, 1 lead en ambas); Toma El control se confirma en 0 leads. **Corrección:** esa nota casi-final describe el CPL de Pyme Colombia como "el mejor de toda la serie documentada (10-01 a la fecha)" — no es exacto: Odoo Test registró $1.79 CPL el 2026-10-01 (ver [[Reports/2026-10-01 - Reporte Performance]]), un CPL más bajo. Este reporte genera además [[Daily notes/2026-10-06 - Resumen del Día]] **(con acento, archivo distinto)** como el resumen ejecutivo confirmado del día, sin sobrescribir la nota casi-final existente de la otra rutina.

## 📋 Resumen Ejecutivo

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| **CPL Promedio** | $7.68 USD | $6-7 | 🟡 +9.7-28.0% vs. meta, pero el mejor cierre confirmado de la serie reciente; mejora -54.7% vs. el cierre confirmado de 10-05 ($16.97) |
| **Gasto Total** | $46.06 USD | - | 🟢 -9.5% vs. 10-05 ($50.92) |
| **Leads Totales** | 6 | 4-5/día | 🟢 Supera la meta por primera vez en la serie reciente, +100.0% vs. 10-05 (3) |
| **CTR Promedio** | 1.72% | 3-4% | 🔴 Por debajo de meta, pero mejora +16.2% vs. 10-05 (1.48%) |
| **CPC Promedio** | $0.37 USD | - | 🟢 -9.8% vs. 10-05 ($0.41) |
| **CPM Promedio** | $6.43 USD | - | 🔻 +5.8% vs. 10-05 ($6.08) |
| **Impresiones** | 7,167 | - | 🔻 -14.4% vs. 10-05 (8,371) |
| **Clicks** | 123 | - | ⚪ -0.8% vs. 10-05 (124), prácticamente estable |
| **Alcance (Reach)** | 5,489 | - | 🔻 -16.6% vs. 10-05 (6,582) |
| **ROAS** | No aplica | - | Campañas Lead Gen sin tracking de valor de conversión |

**Nota:** El CPL blendeado mejora con fuerza (-54.7%) y se acerca más que nunca a la meta $6-7 (apenas +9.7% a +28.0% por encima, según se compare con el extremo inferior o superior del rango) — el mejor cierre confirmado de toda la serie documentada desde el 2026-10-01. La mejora es un espejo casi exacto del cierre de ayer: las tres campañas que cayeron a cero leads simultáneamente el 10-05 (**Pyme Colombia**, **Beco** y **Odoo Test**) se recuperan hoy las tres a la vez, con Pyme Colombia destacando con **$2.50 CPL y 3 leads** — su mejor resultado desde que la campaña tiene datos en esta serie, aunque no el mejor CPL de toda la cuenta documentada (Odoo Test ya había registrado $1.79 el 10-01). En el sentido contrario, **"Toma El control de tu pyme"**, la campaña ancla del proyecto y la que lideró la cuenta ayer ($8.01 CPL, 2 leads), se desploma hoy a **cero leads** — su primer cierre sin ningún lead en toda la serie documentada, pese a que su gasto baja -18.2% y su CTR se mantiene relativamente estable. Es la quinta oscilación de polaridad en cinco días consecutivos para esta campaña.

## 🎯 Performance por Campaña (Ranked por CPL)

### 1. [[Pyme Colombia]] (COL) — Recuperación histórica para la campaña, lidera la cuenta 🟢
```
CPL: $2.50 USD 🟢
Leads: 3
Gasto: $7.50 USD
Clicks: 23
CTR: 3.10% 🟢
CPC: $0.33 USD
CPM: $10.11 USD
Impresiones: 742
Reach: 607
```
**Status:** ACTIVE — Presupuesto/día: $7.50 (gasto = 100.0% del presupuesto)
**Insight:** Ayer cerró en cero leads por primera vez en la serie; hoy revierte con fuerza a **$2.50 CPL y 3 leads**, su mejor cierre documentado y el mejor CTR de toda la cuenta hoy (3.10%, +42.9% vs. ayer). No es, sin embargo, el mejor CPL de toda la serie de la cuenta: Odoo Test ya había registrado $1.79 el 2026-10-01. Sin cambio manual registrado en el activity log que explique la recuperación.

### 2. [[Odoo Test]] (GT) — Vuelve a tener leads, dentro de meta 🟢
```
CPL: $4.72 USD 🟢
Leads: 1
Gasto: $4.72 USD
Clicks: 8
CTR: 0.94% 🔴
CPC: $0.59 USD
CPM: $5.55 USD
Impresiones: 850
Reach: 724
```
**Status:** ACTIVE — Presupuesto/día: $4.93 (gasto = 95.7% del presupuesto)
**Insight:** Revierte el cierre en cero de ayer con 1 lead a $4.72, dentro de la meta $6-7. El CTR mejora +20.5% (0.78%→0.94%) pero sigue siendo el más débil de la cuenta hoy.

### 3. [[Beco]] (GT) — Recupera lead, sigue fuera de meta 🟡
```
CPL: $10.04 USD 🔴
Leads: 1
Gasto: $10.04 USD
Clicks: 29
CTR: 1.32% 🔴
CPC: $0.35 USD
CPM: $4.57 USD
Impresiones: 2,196
Reach: 1,718
```
**Status:** ACTIVE — Presupuesto/día: $10.00 (gasto = 100.4% del presupuesto)
**Insight:** Vuelve a generar 1 lead tras el cierre en cero de ayer, pero el CPL ($10.04) queda muy por encima de la meta $6-7. El CTR cae -8.3% (1.44%→1.32%), el único de los tres "recuperados" que empeora en CTR.

### 4. [[Pyme El salvador]] (SV) — Mejora pero sigue fuera de meta 🟡
```
CPL: $10.70 USD 🔴
Leads: 1
Gasto: $10.70 USD
Clicks: 29
CTR: 1.89% 🟡
CPC: $0.37 USD
CPM: $6.98 USD
Impresiones: 1,533
Reach: 1,187
```
**Status:** ACTIVE — Presupuesto/día: $12.50 (gasto = 85.6% del presupuesto, por debajo por primera vez en varios cierres)
**Insight:** Mejora -21.6% vs. el cierre confirmado de ayer ($13.65), manteniendo 1 lead. Su CTR se recupera con fuerza (+71.8%, 1.10%→1.89%) — la señal más fuerte de esta campaña en varios días, aunque el CPL sigue fuera de meta.

### 5. [[Toma El control de tu pyme]] (GT) — Se desploma a cero leads, su primer cierre sin ningún lead en la serie 🔴
```
Leads: 0
Gasto: $13.10 USD
Clicks: 34
CTR: 1.84% 🟡
CPC: $0.39 USD
CPM: $7.10 USD
Impresiones: 1,846
Reach: 1,422
```
Sin CPL calculable (0 leads).
**Status:** ACTIVE — Presupuesto del único ad set activo: N/D a nivel campaña (gasto = $13.10)
**Insight:** Es la campaña ancla del proyecto (CPL original $9.29, ver [[CLAUDE.md]]). Un día después de liderar toda la cuenta con su mejor cierre confirmado desde el 10-03 ($8.01 CPL, 2 leads), cae hoy a **cero leads** — su primer cierre sin ningún lead en toda la serie documentada (10-01 a la fecha), pese a que el gasto baja -18.2% y el CTR se mantiene relativamente estable (1.96%→1.84%, -6.1%). Es la quinta oscilación de polaridad en cinco días ($17.50 → $6.59 → $16.36 → $8.01 → **0 leads**), sin ningún cambio manual registrado en el activity log. El A/B test de los 5 copys documentado en [[CLAUDE.md]] desde el 2026-08-24 sigue sin iniciarse formalmente; este primer cierre en cero refuerza con más fuerza que nunca la urgencia de lanzarlo.

### Campañas sin actividad (PAUSED, $0 gasto)
- Toma El control de tu pyme (USA)
- Accurate Partners - Loyalti - Nuevas Obligaciones - JUN 2026
- Conversión Clientes Potenciales - MX
- Conversión Clientes Potenciales - PY
- 🟡 CONVERSIÓN - CLIENTES POTENCIALES

## 🔄 Cambios de cuenta detectados (confirmado vía activity log)

- **Cero eventos registrados.** El activity log de la cuenta para la ventana 2026-10-06 06:00–2026-10-07 06:00 UTC no registra ningún evento, ni manual ni automático. Tanto la recuperación simultánea de Pyme Colombia, Beco y Odoo Test como el desplome a cero de "Toma El control de tu pyme" siguen sin ningún correlato de cambio registrado en la cuenta — apunta a volatilidad normal de subasta/entrega/atribución en una cuenta de bajo volumen, no a una intervención del usuario o del sistema.

## 💡 Insights Clave

- **El CPL de cuenta mejora -54.7% a $7.68** — el mejor cierre confirmado de toda la serie documentada desde el 2026-10-01, y ahora apenas +9.7% a +28.0% por encima de la meta $6-7 (el rango más cercano a meta registrado hasta ahora).
- **Los leads confirmados se duplican a 6** (vs. 3 el 10-05), superando por primera vez la meta de 4-5/día.
- **El gasto total cae -9.5% a $46.06** mientras los leads suben +100.0% — la combinación más favorable de la serie reciente: la cuenta gasta menos y convierte mucho mejor.
- **Día espejo casi exacto del cierre de ayer:** las tres campañas que cerraron en cero leads el 10-05 (Pyme Colombia, Beco, Odoo Test) se recuperan hoy las tres a la vez, mientras la única campaña con buen cierre ayer (Toma El control) cae hoy a cero — la jerarquía de la cuenta se invierte por completo por segundo día consecutivo.
- **4 de 5 campañas activas generan al menos 1 lead hoy** (todas salvo Toma El control) — la mejor composición confirmada de la serie; ayer era apenas 2 de 5.
- **CTR blendeado mejora a 1.72% (+16.2% vs. 1.48% de ayer)** y CPC baja a $0.37 (-9.8%), aunque CPM sube a $6.43 (+5.8%) — la mejora del CPL blendeado combina mejor conversión a lead con una subasta ligeramente más cara, no al revés.
- **Solo 2 de 4 campañas con `daily_budget` configurado sobrepasan su presupuesto hoy** (Pyme Colombia 100.0% exacto, Beco 100.4%), mientras Odoo Test (95.7%) y especialmente Pyme El Salvador (85.6%) cierran por debajo — ningún sobrepaso significativo, a diferencia de cierres anteriores.
- **Séptima ventana consecutiva sin ningún evento en el activity log** — ni la recuperación triple ni el desplome de Toma El control tienen un correlato de cambio registrado en la cuenta.
- **Este cierre confirma, con ajuste menor al alza, la lectura casi-final documentada en [[Daily notes/2026-10-07 - Resumen del Dia]]:** CPL confirmado $7.68 vs. $7.58 casi-final, 6 leads en ambas lecturas, gasto $46.06 vs. $45.46 casi-final (+1.3%). Esa nota también describe el CPL de Pyme Colombia como "el mejor de toda la serie documentada" — este reporte corrige esa afirmación: Odoo Test registró $1.79 CPL el 2026-10-01, un resultado mejor (ver [[Reports/2026-10-01 - Reporte Performance]]).

## ✅ Recomendaciones Accionables

- [ ] **Lanzar por fin el A/B testing de los 5 copys mejorados** documentado en [[CLAUDE.md]] desde el 2026-08-24 para "Toma El control de tu pyme" — hoy registró su primer cierre en cero leads de toda la serie, la quinta oscilación de polaridad en cinco días consecutivos ($17.50→$6.59→$16.36→$8.01→0 leads), sin ningún cambio manual que la explique.
- [ ] **Verificar si el cero leads de "Toma El control" es un problema de tracking/formulario** (lead form, pixel, atribución) y no solo de demanda — el CTR se mantuvo relativamente estable (1.84%, apenas -6.1% vs. ayer) mientras los leads cayeron de 2 a 0, una desconexión entre tráfico y conversión a lead que merece revisión técnica además de creativa.
- [ ] **Confirmar si Pyme Colombia, Beco y Odoo Test sostienen su recuperación** en el próximo cierre o si fue un pico puntual de subasta/atribución — es la segunda vez en dos días que el trío oscila junto (cero el 10-05, recuperación el 10-06).
- [ ] **Revisar si Pyme El Salvador necesita un ajuste adicional de creativo o targeting** — mejora hoy (-21.6% CPL, +71.8% CTR) pero sigue siendo la única campaña con lead que permanece fuera de meta.
- [ ] **Extender la revisión creativa a toda la cuenta, no solo a Toma El control:** el CTR blendeado (1.72%) sigue muy por debajo de la meta 3-4% incluso en el mejor cierre de CPL de la serie — el problema de atractivo de los creativos parece generalizado, no aislado a una campaña.
- [ ] **Usuario:** el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") sigue disparándose a las 23:50 GT en vez de después de medianoche (confirmado vía `list_triggers`: cron `50 5 * * *` UTC sin cambios desde el 2026-08-28), causando que sus notas en `Daily notes/` queden mal etiquetadas con los datos del día anterior (ver [[Daily notes/2026-10-07 - Resumen del Dia]]). Solo se puede corregir manualmente desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ; ningún agente automatizado tiene permiso para editarlo.

## 🔗 Enlaces Relacionados

- [[Daily notes/2026-10-06 - Resumen del Día]] - Resumen ejecutivo confirmado del día generado por esta misma rutina
- [[Daily notes/2026-10-07 - Resumen del Dia]] - Lectura casi-final registrada anoche por la otra rutina automatizada (mal etiquetada como "10-07"), consistente con este cierre confirmado salvo la corrección de la afirmación sobre "mejor CPL de la serie"
- [[Reports/2026-10-05 - Reporte Performance]] - Reporte del día anterior
- [[Reports/2026-10-01 - Reporte Performance]] - Contiene el mejor CPL confirmado de la serie (Odoo Test, $1.79)
- [[CLAUDE.md]] - Meta de CPL $6-7 (más cerca que nunca, +9.7% a +28.0%); A/B test de 5 copys mejorados pendiente de formalizar en "Toma El control de tu pyme", urgencia reforzada tras su primer cierre en cero leads
- [[cloud.md]] - Dashboard principal

---
Generado por: Claude Code (Reporte Automatizado) + Meta Ads API
Cuenta: GT | Octopus Innovations (2530001557366648)
Fecha: 2026-10-06
Tags: #daily-note #performance #meta-ads #octopus
