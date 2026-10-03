---
date: 2026-10-02
aliases: [reporte-2026-10-02, performance-02-oct]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-10-02

> [!info] Datos de cierre confirmados
> Pull realizado la mañana del 2026-10-03 (rutina "Daily Meta Ads Performance Report - 7 AM Guatemala") con `date_preset=yesterday`, día ya cerrado completamente en horario de Guatemala (GMT-6). El total de cuenta a nivel `ad_account` cuadra exactamente con la suma de las 5 campañas activas (gasto $60.03, impresiones 10,814, clicks 189, y CPL blendeado $12.01 = $60.03 / 5 leads confirmados). El alcance de cuenta (8,590) es menor que la suma simple por campaña (8,720) por solape normal de audiencias. El activity log de la cuenta para la ventana 2026-10-02 00:00 GT – 2026-10-03 08:00 GT **no registra ningún evento, ni manual ni automático** — tercera ventana consecutiva sin ningún registro.

> [!note] Sobre `Daily notes/2026-10-03 - Resumen del Dia.md`
> Ese archivo (sin acento en "Dia") fue creado por la rutina distinta "Daily Summary - 11:50 PM Guatemala" (`trig_01DMJfrsQXaTY5KJntXisDPQ`), que se dispara a las 23:50 GT — antes de medianoche — por lo que documenta en realidad datos casi-finales de **2026-10-02** (el día que confirma este reporte), mal etiquetados como "10-03" por el mismo bug de zona horaria (22ª ocurrencia consecutiva). Esa lectura casi-final ya anticipaba el vuelco documentado aquí: CPL $11.85 (casi-final) → $12.01 (confirmado), 5 leads en ambas lecturas, gasto $59.25 → $60.03 — la ventana de atribución no sumó leads adicionales, solo un ligero ajuste de gasto (+1.3%). Este reporte genera además [[Daily notes/2026-10-02 - Resumen del Día]] **(con acento, archivo distinto)** como el resumen ejecutivo confirmado del día, sin sobrescribir la nota casi-final existente de la otra rutina.

## 📋 Resumen Ejecutivo

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| **CPL Promedio** | $12.01 USD | $6-7 | 🔴 +127.0% vs. meta, revierte por completo el mejor cierre de la serie (09-30→10-01: -56.6%) |
| **Gasto Total** | $60.03 USD | - | 🔴 +62.1% vs. 10-01 ($37.03) — el mayor gasto diario de toda la serie documentada |
| **Leads Totales** | 5 | 4-5/día | 🟡 Dentro del rango meta en volumen, pero -28.6% vs. 10-01 (7) |
| **CTR Promedio** | 1.75% | 3-4% | 🔴 Por debajo de meta, -7.4% vs. 10-01 (1.89%) |
| **CPC Promedio** | $0.32 USD | - | 🔻 +6.7% vs. 10-01 ($0.30) |
| **CPM Promedio** | $5.55 USD | - | 🟢 -3.3% vs. 10-01 ($5.74) |
| **Impresiones** | 10,814 | - | 🔺 +67.6% vs. 10-01 (6,451) |
| **Clicks** | 189 | - | 🔺 +54.9% vs. 10-01 (122) |
| **Alcance (Reach)** | 8,590 | - | 🔺 +69.6% vs. 10-01 (5,064) |
| **ROAS** | No aplica | - | Campañas Lead Gen sin tracking de valor de conversión |

**Nota:** Peor cierre confirmado desde el 2026-09-30 ($12.20 CPL). El CPL de cuenta casi se duplica (+127.0%) justo un día después de su mejor cierre histórico ($5.29 el 10-01), con gasto +62.1% y leads -28.6% — el peor escenario posible: más inversión, menos resultado. **Odoo Test** colapsa de 2 leads a cero tras ser el mejor performer del día anterior. **Toma El control de tu pyme**, la campaña ancla del proyecto, sale de meta con su peor CPL confirmado hasta ahora ($17.50) justo un día después de entrar a meta por primera vez. **Beco** y **Pyme El Salvador** retroceden con fuerza manteniendo 1 lead cada una. Solo **Pyme Colombia** mejora y cierra dentro de meta, con el mejor CTR de toda la cuenta.

## 🎯 Performance por Campaña (Ranked por CPL)

### 1. [[Pyme Colombia]] (COL) — Única campaña en verde, mejor CTR de la cuenta 🟢
```
CPL: $5.02 USD 🟢
Leads: 2
Gasto: $10.04 USD
Clicks: 48
CTR: 4.58% 🟢
CPC: $0.21 USD
CPM: $9.59 USD
Impresiones: 1,047
Reach: 843
```
**Status:** ACTIVE — Presupuesto/día: $7.50 (gasto = 133.9% del presupuesto)
**Insight:** Sube de 1 a 2 leads manteniéndose dentro de meta ($5.02 CPL) con el mejor CTR de toda la cuenta hoy (4.58%) — la única campaña que mejora y la única que cierra en verde. Sobrepasa su presupuesto diario configurado (133.9%), a diferencia del cierre de ayer donde cerró al 55.5%.

### 2. [[Beco]] (GT) — Retrocede con fuerza, se aleja de meta 🔴
```
CPL: $13.44 USD 🔴
Leads: 1
Gasto: $13.44 USD
Clicks: 48
CTR: 1.44% 🔴
CPC: $0.28 USD
CPM: $4.03 USD
Impresiones: 3,333
Reach: 2,717
```
**Status:** ACTIVE — Presupuesto/día: $10.00 (gasto = 134.4% del presupuesto)
**Insight:** Sube de $7.23 a $13.44 CPL (+85.9%) manteniendo 1 lead, con gasto +85.9% ($7.23 → $13.44). Sobrepasa su presupuesto diario (134.4%), revirtiendo el cierre de ayer donde quedó al 72.3%.

### 3. [[Pyme El salvador]] (SV) — Retrocede, se mantiene fuera de meta 🔴
```
CPL: $14.00 USD 🔴
Leads: 1
Gasto: $14.00 USD
Clicks: 40
CTR: 1.54% 🔴
CPC: $0.35 USD
CPM: $5.39 USD
Impresiones: 2,595
Reach: 2,032
```
**Status:** ACTIVE — Presupuesto/día: $12.50 (gasto = 112.0% del presupuesto)
**Insight:** Sube de $9.83 a $14.00 CPL (+42.4%) manteniendo 1 lead, con gasto +42.4%. Sobrepasa su presupuesto diario (112.0%), a diferencia del 78.6% de ayer. Sigue siendo, junto con Beco y Toma El control, de las que más se alejan de meta.

### 4. [[Toma El control de tu pyme]] (GT) — Sale de meta con su peor CPL confirmado 🔴
```
CPL: $17.50 USD 🔴
Leads: 1
Gasto: $17.50 USD
Clicks: 46
CTR: 1.58% 🔴
CPC: $0.38 USD
CPM: $6.00 USD
Impresiones: 2,919
Reach: 2,365
```
**Status:** ACTIVE — Presupuesto del único ad set activo: N/D a nivel campaña (gasto = $17.50)
**Insight:** Es la campaña ancla del proyecto (CPL original $9.29). Un día después de entrar a meta por primera vez ($6.12 CPL confirmado, 2 leads el 10-01), se dispara a **$17.50 CPL con solo 1 lead** — su peor cierre confirmado hasta ahora, superando el $14.14 del 09-30. El gasto sube +42.9% ($12.24 → $17.50) sin ningún cambio manual registrado en el activity log. El A/B test de los 5 copys documentado en [[CLAUDE.md]] sigue sin iniciarse formalmente, y la urgencia de retomarlo es ahora máxima.

### 5. [[Odoo Test]] (GT) — Colapsa a cero leads tras ser el mejor performer de ayer 🔴
```
CPL: N/D (0 leads)
Leads: 0
Gasto: $5.05 USD
Clicks: 7
CTR: 0.76% 🔴
CPC: $0.72 USD
CPM: $5.49 USD
Impresiones: 920
Reach: 763
```
**Status:** ACTIVE — Presupuesto/día: $4.93 (gasto = 102.4% del presupuesto)
**Insight:** Fue el mejor performer de la cuenta ayer ($1.79 CPL, 2 leads, CTR 1.44%). Hoy cierra en cero leads con CTR 0.76% —menos de la mitad del de ayer— a pesar de gastar 42.6% más ($3.57 → $5.05). Repite el patrón "cero → positivo → cero" ya documentado en varios cierres anteriores de esta campaña, ahora en su versión más marcada.

### Campañas sin actividad (PAUSED, $0 gasto)
- Toma El control de tu pyme (USA)
- Accurate Partners - Loyalti - Nuevas Obligaciones - JUN 2026
- Conversión Clientes Potenciales - MX
- Conversión Clientes Potenciales - PY
- 🟡 CONVERSIÓN - CLIENTES POTENCIALES

## 🔄 Cambios de cuenta detectados (confirmado vía activity log)

- **Cero eventos registrados.** El activity log de la cuenta para la ventana 2026-10-02 00:00 GT – 2026-10-03 08:00 GT no registra ningún evento, ni manual ni automático — tercera ventana consecutiva sin ningún registro en la serie documentada. El vuelco negativo de hoy, igual que la mejora del 10-01, no tiene ningún correlato de cambio registrado en la cuenta; todo apunta a volatilidad de subasta/entrega o aprendizaje del algoritmo, no a una intervención del usuario o del sistema.

## 💡 Insights Clave

- **El CPL de cuenta sube +127.0% a $12.01** — revierte por completo el mejor cierre confirmado de toda la serie ($5.29 el 10-01), regresando casi al nivel del peor cierre reciente ($12.20 el 09-30).
- **Los leads confirmados caen de 7 a 5 (-28.6%) con un gasto +62.1%** ($37.03 → $60.03) — el peor escenario posible: más inversión y menos resultado, lo opuesto al patrón del 10-01.
- **Solo 1 de 5 campañas activas cierra dentro de meta hoy** (Pyme Colombia), frente a 3 de 5 ayer (Odoo Test, Pyme Colombia, Toma El control) — la peor composición desde el 09-30.
- **4 de 5 campañas activas sobrepasan su `daily_budget` configurado** (102.4%-134.4%), justo el día de peor conversión de la cuenta — a diferencia de ayer, cuando las 5 cerraron por debajo de presupuesto (55.5%-78.6%). El sobregasto coincide con el peor día de conversión, sugiriendo que el algoritmo gastó más persiguiendo resultados que no llegaron.
- **Odoo Test y "Toma El control de tu pyme" concentran el deterioro**: el primero pasa de 2 leads a cero, el segundo pasa de su mejor cierre histórico a su peor, ambos sin ningún cambio manual registrado.
- **CTR de cuenta baja a 1.75% (-7.4% vs. 10-01)**, mientras CPC sube levemente (+6.7%) y CPM baja (-3.3%) — el deterioro está concentrado en la conversión a lead, no en el costo de la subasta en sí.
- **Cero eventos en el activity log en 24 horas**, tercera ventana consecutiva sin ningún registro — el vuelco de hoy, igual que la mejora de ayer, sigue sin una causa operativa visible en los datos de cuenta disponibles.
- **Este cierre confirma, con un ajuste menor de gasto, la lectura casi-final documentada en [[Daily notes/2026-10-03 - Resumen del Dia]]:** CPL confirmado $12.01 vs. $11.85 casi-final, 5 leads en ambas lecturas, gasto $60.03 vs. $59.25 casi-final.

## ✅ Recomendaciones Accionables

- [ ] **Investigar a fondo por qué "Toma El control de tu pyme" (GT) se dispara a su peor CPL confirmado ($17.50)** justo un día después de entrar a meta por primera vez — descartar causas operativas (pixel, tracking de leads, cambios de audiencia/aprendizaje de algoritmo) antes de asumir volatilidad normal.
- [ ] **Priorizar de inmediato el A/B testing pendiente de los 5 copys mejorados** en "Toma El control de tu pyme" (GT), documentado en [[CLAUDE.md]] desde 2026-08-24 pero aún sin iniciar formalmente — la urgencia es máxima tras el peor cierre histórico confirmado de esta campaña.
- [ ] **Revisar el tercer ciclo "cero → positivo → cero" de Odoo Test**, hoy con el peor CTR confirmado (0.76%) — evaluar una revisión dedicada de creativo/targeting en vez de seguir monitoreando pasivamente.
- [ ] **Revisar por qué 4 de 5 campañas sobrepasaron su `daily_budget` configurado hoy** (102.4%-134.4%), justo el día de peor conversión de la cuenta — confirmar si conviene ajustar presupuestos o pacing.
- [ ] **Dar seguimiento a Pyme Colombia**, única campaña en verde hoy (CPL $5.02, CTR 4.58%, mejor de la cuenta) y la única con más leads que ayer — evaluar si amerita más presupuesto dado que es la más eficiente.
- [ ] **Usuario:** el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") sigue disparándose a las 23:50 GT en vez de después de medianoche — 22ª ocurrencia consecutiva confirmada vía `list_triggers` (cron sin cambios desde su creación el 2026-08-28), causando que sus notas en `Daily notes/` queden mal etiquetadas con los datos del día anterior. Solo se puede corregir manualmente desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ; ningún agente automatizado tiene permiso para editarlo.

## 🔗 Enlaces Relacionados

- [[Daily notes/2026-10-02 - Resumen del Día]] - Resumen ejecutivo confirmado del día generado por esta misma rutina
- [[Daily notes/2026-10-03 - Resumen del Dia]] - Lectura casi-final registrada anoche por la otra rutina automatizada (mal etiquetada como "10-03"), consistente con este cierre confirmado
- [[Reports/2026-10-01 - Reporte Performance]] - Reporte del día anterior
- [[CLAUDE.md]] - Meta de CPL $6-7 (fuera de meta hoy, +127.0%); A/B test de 5 copys mejorados pendiente de formalizar en "Toma El control de tu pyme", ahora urgente
- [[cloud.md]] - Dashboard principal

---
Generado por: Claude Code (Reporte Automatizado) + Meta Ads API
Cuenta: GT | Octopus Innovations (2530001557366648)
Fecha: 2026-10-02
Tags: #daily-note #performance #meta-ads #octopus
