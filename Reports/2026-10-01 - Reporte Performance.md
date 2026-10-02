---
date: 2026-10-01
aliases: [reporte-2026-10-01, performance-01-oct]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-10-01

> [!info] Datos de cierre confirmados
> Pull realizado la mañana del 2026-10-02 (rutina "Daily Meta Ads Performance Report - 7 AM Guatemala") con `date_preset=yesterday`, día ya cerrado completamente en horario de Guatemala (GMT-6). El total de cuenta a nivel `ad_account` cuadra exactamente con la suma de las 5 campañas activas (gasto $37.03, impresiones 6,451, clicks 122, y CPL blendeado $5.29 = $37.03 / 7 leads confirmados). El alcance de cuenta (5,064) es menor que la suma simple por campaña (5,332) por solape normal de audiencias. El activity log de la cuenta para la ventana 2026-10-01 00:00 GT – 2026-10-02 08:00 GT **no registra ningún evento, ni manual ni automático** — primera vez en toda la serie documentada sin ningún registro, ni siquiera la creación automática de audiencia personalizada por Meta que aparecía en ventanas anteriores.

> [!note] Sobre `Daily notes/2026-10-01 - Resumen del Dia.md`
> Ese archivo (sin acento en "Dia") fue creado por la rutina distinta "Daily Summary - 11:50 PM Guatemala" (`trig_01DMJfrsQXaTY5KJntXisDPQ`), que se dispara a las 23:50 GT — antes de medianoche — por lo que documenta en realidad datos casi-finales de **2026-09-30**, ya confirmados en [[Reports/2026-09-30 - Reporte Performance]]. La lectura casi-final de **2026-10-01** (el día que confirma este reporte) quedó registrada en `Daily notes/2026-10-02 - Resumen del Dia.md` por el mismo bug de zona horaria (21ª ocurrencia consecutiva confirmada en esa nota, cron sin cambios en `50 5 * * *` UTC desde su creación el 2026-08-28). Este reporte confirma esa lectura casi-final (CPL $5.19 → $5.29, 7 leads en ambas lecturas, gasto $36.31 → $37.03) y genera además [[Daily notes/2026-10-01 - Resumen del Día]] **(con acento, archivo distinto)** como el resumen ejecutivo confirmado del día que pide esta rutina, sin sobrescribir la nota casi-final existente de la otra rutina.

## 📋 Resumen Ejecutivo

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| **CPL Promedio** | $5.29 USD | $6-7 | 🟢 Dentro/por debajo de meta por primera vez en toda la serie confirmada, -56.6% vs. 09-30 ($12.20) |
| **Gasto Total** | $37.03 USD | - | 🟢 -24.1% vs. 09-30 ($48.78) |
| **Leads Totales** | 7 | 4-5/día | 🟢 Supera la meta, +75.0% vs. 09-30 (4) |
| **CTR Promedio** | 1.89% | 3-4% | 🔴 Por debajo de meta, pero +39.0% vs. 09-30 (1.36%) |
| **CPC Promedio** | $0.30 USD | - | 🟢 -37.5% vs. 09-30 ($0.48) |
| **CPM Promedio** | $5.74 USD | - | 🟢 -12.4% vs. 09-30 ($6.55) |
| **Impresiones** | 6,451 | - | 🔻 -13.3% vs. 09-30 (7,445) |
| **Clicks** | 122 | - | 🟢 +20.8% vs. 09-30 (101) |
| **Alcance (Reach)** | 5,064 | - | 🔻 -11.3% vs. 09-30 (5,712) |
| **ROAS** | No aplica | - | Campañas Lead Gen sin tracking de valor de conversión |

**Nota:** Mejor cierre confirmado de toda la serie documentada. El CPL de cuenta se desploma -56.6% a $5.29, la primera vez que el conjunto de la cuenta cierra dentro del rango meta $6-7. Los leads confirmados suben de 4 a 7 (+75.0%) con gasto -24.1% — más conversión con menos inversión. Las dos campañas que venían encadenando cierres consecutivos en cero (**Pyme Colombia** y **Odoo Test**) vuelven a generar leads, con Odoo Test como el mejor performer del día; **Toma El control de tu pyme** entra por primera vez dentro de meta; y aunque **Beco** retrocede desde su mejor cierre de ayer, se mantiene en el límite superior de meta. Solo **Pyme El Salvador** cierra fuera de rango, aunque con su mejor CPL documentado hasta ahora.

## 🎯 Performance por Campaña (Ranked por CPL)

### 1. [[Odoo Test]] (GT) — Mejor performer del día, revierte el patrón de ceros 🟢
```
CPL: $1.79 USD 🟢
Leads: 2
Gasto: $3.57 USD
Clicks: 9
CTR: 1.44% 🔴
CPC: $0.40 USD
CPM: $5.71 USD
Impresiones: 625
Reach: 525
```
**Status:** ACTIVE — Presupuesto/día: $4.93 (gasto = 72.4% del presupuesto)
**Insight:** Rompe el ciclo "cero → positivo → cero" documentado en varios cierres previos: pasa de 0 a 2 leads con el mejor CPL de toda la cuenta hoy. Sin ningún cambio manual registrado en el activity log (que está completamente vacío esta ventana).

### 2. [[Pyme Colombia]] (COL) — Rompe el "doble cero" confirmado 🟢
```
CPL: $4.16 USD 🟢
Leads: 1
Gasto: $4.16 USD
Clicks: 21
CTR: 4.04% 🟢
CPC: $0.20 USD
CPM: $8.00 USD
Impresiones: 520
Reach: 439
```
**Status:** ACTIVE — Presupuesto/día: $7.50 (gasto = 55.5% del presupuesto)
**Insight:** Tras dos cierres confirmados consecutivos en cero (09-29 y 09-30), vuelve a convertir con el mejor CTR de toda la cuenta (4.04%) y CPL dentro de meta — resuelve, al menos por hoy, la preocupación de tracking/pixel señalada en los dos reportes anteriores.

### 3. [[Toma El control de tu pyme]] (GT) — Entra a meta por primera vez 🟢
```
CPL: $6.12 USD 🟢
Leads: 2
Gasto: $12.24 USD
Clicks: 51
CTR: 2.26% 🔴
CPC: $0.24 USD
CPM: $5.42 USD
Impresiones: 2,258
Reach: 1,860
```
**Status:** ACTIVE — Presupuesto del único ad set activo: N/D a nivel campaña (gasto = $12.24)
**Insight:** Es la campaña ancla del proyecto (CPL original $9.29, y que venía cerrando entre $13.80-$14.14 en los últimos cierres confirmados). Cae a $6.12 CPL con 2 leads, su mejor cierre confirmado y la primera vez dentro del rango meta $6-7. El A/B test de los 5 copys documentado en [[CLAUDE.md]] sigue sin iniciarse formalmente, por lo que la mejora no puede atribuirse a esa intervención pendiente.

### 4. [[Beco]] (GT) — Retrocede desde su mejor cierre pero se mantiene en el límite de meta 🟡
```
CPL: $7.23 USD 🟡
Leads: 1
Gasto: $7.23 USD
Clicks: 18
CTR: 1.11% 🔴
CPC: $0.40 USD
CPM: $4.48 USD
Impresiones: 1,615
Reach: 1,374
```
**Status:** ACTIVE — Presupuesto/día: $10.00 (gasto = 72.3% del presupuesto)
**Insight:** Tras su mejor cierre confirmado de ayer ($4.88 CPL, 2 leads), retrocede a 1 lead y $7.23 CPL (+48.2%) — justo en el borde superior del rango meta $6-7, no una caída seria.

### 5. [[Pyme El salvador]] (SV) — Mejora con fuerza pero sigue fuera de meta 🔴
```
CPL: $9.83 USD 🔴
Leads: 1
Gasto: $9.83 USD
Clicks: 23
CTR: 1.61% 🔴
CPC: $0.43 USD
CPM: $6.86 USD
Impresiones: 1,433
Reach: 1,134
```
**Status:** ACTIVE — Presupuesto/día: $12.50 (gasto = 78.6% del presupuesto)
**Insight:** Baja de $14.04 a $9.83 CPL (-30.0%), su mejor cierre confirmado hasta ahora, aunque todavía fuera del rango meta $6-7. Única campaña activa que cierra el día fuera de meta.

### Campañas sin actividad (PAUSED, $0 gasto)
- Toma El control de tu pyme (USA)
- Accurate Partners - Loyalti - Nuevas Obligaciones - JUN 2026
- Conversión Clientes Potenciales - MX
- Conversión Clientes Potenciales - PY
- 🟡 CONVERSIÓN - CLIENTES POTENCIALES

## 🔄 Cambios de cuenta detectados (confirmado vía activity log)

- **Cero eventos registrados.** El activity log de la cuenta para la ventana 2026-10-01 00:00 GT – 2026-10-02 08:00 GT no registra ningún evento, ni manual ni automático — primera vez en toda la serie documentada sin ningún registro (todas las ventanas anteriores al menos mostraban la creación automática de audiencia personalizada por Meta). La mejora generalizada de la cuenta no tiene ningún correlato de cambio registrado; todo apunta a una variación favorable de subasta/entrega o aprendizaje del algoritmo, no a una intervención del usuario o del sistema.

## 💡 Insights Clave

- **El CPL de cuenta cae -56.6% a $5.29** — el mejor resultado de toda la serie documentada y la primera vez que el conjunto de la cuenta cierra dentro de la meta $6-7, confirmando la lectura casi-final de anoche (CPL $5.19).
- **Los leads confirmados suben de 4 a 7 (+75.0%) con gasto -24.1%** ($48.78 → $37.03) — más conversión con menos inversión, el patrón opuesto al observado en cierres anteriores.
- **5 de 5 campañas activas cierran con al menos 1 lead hoy**, y 3 de 5 (Odoo Test, Pyme Colombia, Toma El control) cierran por debajo de la meta $6-7 — la mejor composición de toda la serie confirmada.
- **Pyme Colombia y Odoo Test rompen sus respectivas rachas de cero leads** el mismo día, resolviendo (al menos por hoy) la preocupación de tracking/pixel señalada en los dos reportes anteriores.
- **"Toma El control de tu pyme", la campaña ancla del proyecto, entra a meta por primera vez** ($6.12 CPL) sin que el A/B test de copys pendiente en [[CLAUDE.md]] se haya iniciado formalmente.
- **CTR de cuenta sube a 1.89% (+39.0% vs. 09-30)** y CPC/CPM bajan con fuerza (-37.5% y -12.4% respectivamente) — mejora generalizada de eficiencia de subasta, no solo de conversión a lead.
- **Cero eventos en el activity log en 24 horas**, a diferencia de todas las ventanas anteriores (que al menos registraban la creación automática de audiencia personalizada por Meta) — la mejora no tiene ningún correlato de cambio registrado en la cuenta.
- **Ninguna campaña cierra con sobregasto hoy** (55.5%-78.6% del presupuesto diario configurado) — a diferencia de cierres anteriores con sobregasto puntual.
- **Este cierre confirma, con un ajuste menor de gasto, la lectura casi-final documentada en [[Daily notes/2026-10-02 - Resumen del Dia]]:** CPL confirmado $5.29 vs. $5.19 casi-final, 7 leads en ambas lecturas, gasto $37.03 vs. $36.31 casi-final — la ventana de atribución no sumó leads adicionales, solo un ligero ajuste de gasto (+2.0%).

## ✅ Recomendaciones Accionables

- [ ] **Investigar qué impulsó la mejora generalizada** (CPL -56.6%, CTR +39.0%, sin ningún evento en el activity log) antes de asumir que es solo volatilidad de subasta — revisar si hay señales de aprendizaje de algoritmo o cambios de calidad de audiencia no capturados por el activity log estándar.
- [ ] **Confirmar si Pyme Colombia y Odoo Test sostienen su regreso a conversión** en el próximo cierre antes de descartar definitivamente la preocupación de tracking/pixel señalada en los dos reportes anteriores.
- [ ] **Dar seguimiento a "Toma El control de tu pyme"** tras su primer cierre confirmado dentro de meta ($6.12 CPL) — decidir si todavía amerita el A/B test de 5 copys pendiente en [[CLAUDE.md]] o si conviene documentar primero qué causó esta mejora orgánica antes de introducir una variable nueva.
- [ ] **Evaluar escalar el presupuesto de Odoo Test y Pyme Colombia**, hoy los mejores performers y ambos con margen de presupuesto no utilizado (72.4% y 55.5% respectivamente).
- [ ] **Seguir monitoreando a Pyme El Salvador**, única campaña fuera de meta hoy pese a su mejor cierre confirmado (-30.0% de CPL) — seguir la tendencia de mejora antes de intervenir.
- [ ] **Usuario:** el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") sigue disparándose a las 23:50 GT en vez de después de medianoche — 21ª ocurrencia consecutiva confirmada vía `list_triggers` (cron sin cambios desde su creación el 2026-08-28), causando que sus notas en `Daily notes/` queden mal etiquetadas con los datos del día anterior. Solo se puede corregir manualmente desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ; ningún agente automatizado tiene permiso para editarlo.

## 🔗 Enlaces Relacionados

- [[Daily notes/2026-10-01 - Resumen del Día]] - Resumen ejecutivo confirmado del día generado por esta misma rutina
- [[Daily notes/2026-10-02 - Resumen del Dia]] - Lectura casi-final registrada anoche por la otra rutina automatizada (mal etiquetada como "10-02"), consistente con este cierre confirmado
- [[Reports/2026-09-30 - Reporte Performance]] - Reporte del día anterior
- [[CLAUDE.md]] - Meta de CPL $6-7 (dentro de meta hoy por primera vez a nivel de cuenta); A/B test de 5 copys mejorados pendiente de formalizar en "Toma El control de tu pyme"
- [[cloud.md]] - Dashboard principal

---
Generado por: Claude Code (Reporte Automatizado) + Meta Ads API
Cuenta: GT | Octopus Innovations (2530001557366648)
Fecha: 2026-10-01
Tags: #daily-note #performance #meta-ads #octopus
