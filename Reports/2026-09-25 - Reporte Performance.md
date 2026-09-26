---
date: 2026-09-25
aliases: [reporte-2026-09-25, performance-25-sep]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-09-25

> [!info] Datos de cierre confirmados
> Pull realizado 2026-09-26 ~07:19 GT con `time_range` explícito (`2026-09-25` a `2026-09-25`), día ya cerrado completamente en horario de Guatemala (GMT-6). El total de cuenta a nivel `ad_account` cuadra exactamente con la suma de las 5 campañas activas (gasto $48.41, impresiones 8,271, clicks 119, y `cost_per_lead` blendeado $6.05125 = $48.41 / 8 leads confirmados). El activity log de la cuenta para la ventana 2026-09-25 00:00–2026-09-26 13:19 UTC registró 5 eventos (detallados abajo), a diferencia de los dos cierres anteriores (ambos vacíos).

> [!note] Corrección de `Daily notes/2026-09-25 - Resumen del Dia.md`
> Esa nota fue creada por la rutina "Daily Summary - 11:50 PM Guatemala" (`trig_01DMJfrsQXaTY5KJntXisDPQ`), que se dispara a las 23:50 GT — antes de medianoche — por lo que su lectura de "hoy" correspondía en realidad a **2026-09-24**, no a 2026-09-25 (bug de zona horaria documentado 14 veces consecutivas en el proyecto, sin corrección disponible salvo por el usuario). Este reporte corrige esa nota con los datos reales y confirmados de 2026-09-25 — ver sección de enlaces.

## 📋 Resumen Ejecutivo

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| **CPL Promedio** | $6.05 USD | $6-7 | 🟢 Dentro de meta, aunque +29.0% vs. 09-24 ($4.69) |
| **Gasto Total** | $48.41 USD | - | 🔻 +14.7% vs. 09-24 ($42.20) |
| **Leads Totales** | 8 | 4-5/día | 🟢 Supera la meta, aunque -11.1% vs. 09-24 (9) |
| **CTR Promedio** | 1.44% | 3-4% | 🔴 Por debajo de meta, -16.3% vs. 09-24 (1.72%) |
| **CPC Promedio** | $0.41 USD | - | 🔻 +20.6% vs. 09-24 ($0.34) |
| **CPM Promedio** | $5.85 USD | - | 🟢 -0.2% vs. 09-24 ($5.86) |
| **Impresiones** | 8,271 | - | 🔺 +14.9% vs. 09-24 (7,198) |
| **Clicks** | 119 | - | 🔻 -4.0% vs. 09-24 (124) |
| **Alcance (Reach)** | 6,486 | - | 🔺 +21.9% vs. 09-24 (5,321) |
| **ROAS** | No aplica | - | Campañas Lead Gen sin tracking de valor de conversión |

**Nota:** El CPL de cuenta sube a $6.05 (+29.0% vs. 09-24), se mantiene dentro de la meta $6-7 pero revierte buena parte de la mejora radical documentada ayer. La causa es la combinación exacta opuesta a la de ayer: más gasto (+14.7%) y menos leads (-11.1%). Dos de las 5 campañas activas (Pyme El Salvador, Odoo Test) cierran hoy en cero leads — exactamente las dos que ayer se habían "recuperado" de sus rachas negativas, revirtiendo por completo el hito de ayer (las 5 con al menos 1 lead).

## 🎯 Performance por Campaña (Ranked por CPL)

### 1. [[Toma El control de tu pyme]] (GT) — Sigue liderando, aunque su CPL sube 🟢
```
CPL: $3.59 USD 🟢
Leads: 4
Gasto: $14.37 USD
Clicks: 43
CTR: 1.70%
CPC: $0.33 USD
CPM: $5.69 USD
Impresiones: 2,524
Reach: 2,053
```
**Status:** ACTIVE — Presupuesto del único ad set activo ("Urgencia"): $15.00 (gasto = 95.8% del presupuesto)
**Insight:** Mejor performer de la cuenta por tercer cierre consecutivo, mismo volumen de leads que ayer (4), pero su CPL sube +18.1% ($3.04→$3.59) y por primera vez en varios días su ad set "Urgencia" se acerca a su presupuesto configurado (95.8%, vs. 80.9% ayer).

### 2. [[Beco]] (GT) — Rompe su racha de CPL fuera de meta, mejor cierre documentado 🟢
```
CPL: $3.64 USD 🟢
Leads: 3
Gasto: $10.91 USD
Clicks: 34
CTR: 1.50%
CPC: $0.32 USD
CPM: $4.80 USD
Impresiones: 2,273
Reach: 1,799
```
**Status:** ACTIVE — Presupuesto/día: $10.00 (gasto = 109.1% del presupuesto)
**Insight:** Pasa de ser la única campaña fuera de meta ayer ($9.46 CPL) a la segunda mejor hoy ($3.64 CPL, 3 leads) — su mejor cierre documentado en el proyecto. Sigue levemente sobre presupuesto (109.1%), patrón recurrente sin corregir.

### 3. [[Pyme Colombia]] (COL) — Primer día completo con el nuevo creativo "Urgencia" 🟢
```
CPL: $6.14 USD 🟢
Leads: 1
Gasto: $6.14 USD
Clicks: 8
CTR: 1.77%
CPC: $0.77 USD
CPM: $13.58 USD
Impresiones: 452
Reach: 343
```
**Status:** ACTIVE — Presupuesto/día: $7.50 (gasto = 81.9% del presupuesto)
**Insight:** Primer cierre de día completo con el nuevo creativo del anuncio "AD Pyme Urgencia COL" (reemplazado ayer a las 12:18 PM GT). CPL $6.14 dentro de meta pero en el límite superior, con solo 1 lead y el CPM más alto de la cuenta ($13.58) — aún insuficiente para concluir si el nuevo copy mejora el rendimiento; requiere 1-2 cierres más.

### 4. [[Pyme El salvador]] (SV) — Cierra en cero leads, revierte su recuperación de ayer 🔴
```
Leads: 0
Gasto: $12.03 USD
Clicks: 24
CTR: 1.06%
CPC: $0.50 USD
CPM: $5.32 USD
Impresiones: 2,262
Reach: 1,735
```
**Status:** ACTIVE — Presupuesto/día: $12.50 (gasto = 96.2% del presupuesto)
**Insight:** Vuelve a cero leads tras un solo cierre de recuperación (2 leads, 09-24) — refuerza la sospecha de que su patrón de ceros intermitentes es más estructural (creativo, tracking o audiencia) que variance puntual de bajo volumen.

### 5. [[Odoo Test]] (GT) — Cierra en cero leads, revierte su recuperación de ayer 🔴
```
Leads: 0
Gasto: $4.96 USD
Clicks: 10
CTR: 1.32%
CPC: $0.50 USD
CPM: $6.53 USD
Impresiones: 760
Reach: 592
```
**Status:** ACTIVE — Presupuesto/día: $4.93 (gasto = 100.6% del presupuesto)
**Insight:** Igual que Pyme El Salvador, vuelve a cero leads tras su único cierre de recuperación (1 lead, 09-24). Es la única campaña que cierra hoy prácticamente exacta a su presupuesto configurado (100.6%), tras varios días consecutivos por encima.

### Campañas sin actividad (PAUSED, $0 gasto)
- Toma El control de tu pyme (USA)
- Accurate Partners - Loyalti - Nuevas Obligaciones - JUN 2026
- Conversión Clientes Potenciales - MX
- Conversión Clientes Potenciales - PY
- 🟡 CONVERSIÓN - CLIENTES POTENCIALES

## 🧪 A/B Test — "Toma El control de tu pyme" (GT)

| Ad Set | Status | Presupuesto/día | Gasto | % del presupuesto | Clicks | CTR | Leads | CPL |
|--------|--------|------------------|-------|--------------------|--------|-----|-------|-----|
| TestA/B Urgencia | ACTIVE 🟢 | $15.00 | $14.37 | 95.8% | 43 | 1.70% | 4 | $3.59 |
| TestA/B Excel | PAUSED ⏸️ | $7.50 | $0.00 | - | 0 | - | - | - |
| TestA/B Productividad | PAUSED ⏸️ | $5.00 | $0.00 | - | 0 | - | - | - |
| GT + QTZ | PAUSED ⏸️ | $20.00 | $0.00 | - | 0 | - | - | - |

**Nota:** "Urgencia" sigue siendo el único ad set activo del A/B test formal; su gasto se acerca más a su presupuesto que ayer (95.8% vs. 80.9%) y su CPL sube de $3.04 a $3.59 (+18.1%), aunque se mantiene como el mejor performer de la cuenta.

## 🔄 Cambio de cuenta detectado (confirmado vía activity log)

- **Reemplazo de creativo en Pyme Colombia:** Gabriel Calderon reemplazó vía Power Editor el creativo del anuncio "AD Pyme Urgencia COL" (ad id `120256952282780211`, ad set `120256952282790211`), pasando de la creatividad `1578260823463271` a `1413857937560440`. El cambio se inició a las **12:18 PM GT** y el anuncio quedó activo tras revisión de Meta a las **12:21 PM GT** — es la primera acción concreta hacia el A/B testing pendiente de los 5 copys mejorados documentado en [[CLAUDE.md]], aunque aplicada a Pyme Colombia en vez de la campaña GT originalmente planeada.
- **Nuevo administrador agregado a la cuenta** a las 9:07 AM GT (user id `3158599694341600`, rol "Ad account admin"), acción manual de Gabriel Calderon.
- Ningún otro cambio de presupuesto, targeting o estado fue registrado en la ventana 2026-09-25 00:00–2026-09-26 13:19 UTC.

## 💡 Insights Clave

- **El CPL de cuenta sube a $6.05 (+29.0% vs. 09-24), se mantiene dentro de la meta $6-7** pero revierte buena parte del mejor cierre confirmado del proyecto documentado ayer ($4.69).
- **Los leads bajan de 9 a 8 (-11.1%) mientras el gasto sube +14.7%** ($42.20→$48.41) — combinación doblemente desfavorable: menos resultados con más inversión.
- **Dos de cinco campañas activas cierran en cero leads (Pyme El Salvador, Odoo Test)** — exactamente las dos que ayer se habían recuperado de sus rachas negativas — revierte por completo el hito de ayer (las 5 activas con al menos 1 lead) y refuerza que el patrón de ceros intermitentes en ambas es más estructural que variance de un solo día.
- **CTR cae a 1.44% (-16.3% vs. ayer) y CPC sube a $0.41 (+20.6%)** — el tráfico fue menos eficiente hoy, no solo la conversión a lead.
- **CPM se mantiene prácticamente estable** ($5.85 vs. $5.86, -0.2%) — el costo de exposición no cambió; el deterioro está en clics y conversión, no en la puja/competencia por audiencia.
- **Beco es el punto fuerte inesperado del cierre**: pasa de ser la única campaña fuera de meta ayer ($9.46 CPL) a la segunda mejor hoy ($3.64 CPL, 3 leads) — su mejor cierre documentado en el proyecto, sin ningún cambio manual registrado en el activity log que lo explique.
- **El reemplazo de creativo en Pyme Colombia** (confirmado en el activity log a las 12:18-12:21 PM GT) es la primera acción concreta hacia el A/B test pendiente de los 5 copys mejorados de [[CLAUDE.md]], aunque aplicado a una campaña distinta a la originalmente planeada. Con su primer día completo de exposición, cierra en $6.14 CPL y 1 lead — dentro de meta pero insuficiente aún para concluir sobre su desempeño real.

## ✅ Recomendaciones Accionables

- [ ] **Investigar por qué Pyme El Salvador y Odoo Test vuelven a cero leads** tras un solo cierre de recuperación — el patrón repetido en 3 de los últimos 4 cierres sugiere un problema estructural (creativo, tracking o audiencia) más que variance de bajo volumen.
- [ ] **Dar seguimiento al nuevo creativo "Urgencia" de Pyme Colombia** con 1-2 cierres más antes de concluir si mejora o empeora el rendimiento frente al creativo anterior.
- [ ] **Evaluar formalizar el reemplazo de creativo de Pyme Colombia** como parte del A/B testing pendiente de los 5 nuevos copys, y decidir si también se aplica a "Toma El control de tu pyme" (GT), la campaña originalmente documentada en [[CLAUDE.md]].
- [ ] **Investigar la mejora de Beco** ($9.46→$3.64 CPL) para entender si es sostenible o un evento puntual, dado que no hay cambio manual registrado que lo explique.
- [ ] **Ajustar el `daily_budget` de Beco:** sigue levemente sobre presupuesto (109.1%), patrón recurrente sin corregir.
- [ ] Retomar el A/B testing pendiente de los 5 nuevos copys en "Toma El control de tu pyme" (GT), documentado en el proyecto pero aún sin iniciar formalmente en esa campaña.
- [ ] **Usuario:** confirmar que el nuevo administrador agregado el 09-25 a las 9:07 AM GT (user id `3158599694341600`) es una adición esperada.
- [ ] **Usuario:** el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") sigue disparándose a las 23:50 GT en vez de después de medianoche — 15ª ocurrencia consecutiva documentada, causando que sus notas en `Daily notes/` queden mal etiquetadas con los datos del día anterior. Solo se puede corregir manualmente desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ; ningún agente automatizado tiene permiso para editarlo (rechazado explícitamente por el sistema en sesiones anteriores).

## 🔗 Enlaces Relacionados

- [[Daily notes/2026-09-25 - Resumen del Dia]] - Nota del día (corregida con el cierre confirmado; antes contenía por error datos casi-finales de 09-24)
- [[Daily notes/2026-09-26 - Resumen del Dia]] - Lectura casi-final registrada hoy por la otra rutina automatizada, consistente con este cierre confirmado
- [[Reports/2026-09-24 - Reporte Performance]] - Reporte del día anterior
- [[CLAUDE.md]] - Meta de CPL $6-7; A/B test de 5 copys mejorados pendiente de formalizar
- [[cloud.md]] - Dashboard principal

---
Generado por: Claude Code (Reporte Automatizado) + Meta Ads API
Cuenta: GT | Octopus Innovations (2530001557366648)
Fecha: 2026-09-25
Tags: #daily-note #performance #meta-ads #octopus
