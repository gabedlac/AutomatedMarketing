---
date: 2026-11-14
aliases: [resumen-2026-11-14]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-11-14

> [!warning] Corrección aplicada el 2026-11-15 (cifras de cierre)
> Este archivo se generó originalmente el propio 11-14 vía `ads_get_ad_entities` (`date_preset=today`), con datos parciales por el lag normal de atribución de Meta. El 2026-11-15 se consultó el cierre confirmado (`date_preset=yesterday`) y las cifras de abajo fueron **actualizadas para reflejar el cierre real**, que resultó **peor** que la lectura intradía (8 leads vs. 14 reportados originalmente; CPL $9.01 vs. $5.35) — el primer caso documentado en el vault donde el cierre empeora en vez de mejorar. Ver detalle completo en [[Reports/2026-11-14 - Reporte Performance]].

---

## 🎯 Campañas Revisadas (cifras de cierre confirmadas el 2026-11-15)

Se revisaron las 7 campañas activas de lead-gen + 1 de evento vía `ads_get_ad_entities` (nivel campaña, `date_preset=yesterday` desde el 2026-11-15):

| Campaña | Status | Gasto | Impresiones | Clicks | CTR | Leads | CPL |
|---|---|---|---|---|---|---|---|
| 🟢 SLV \| Odoo \| CP \| Servicios | ACTIVE | $6.94 | 920 | 26 | 2.83% | 3 | **$2.31** |
| 🟡 PY \| Odoo \| CP \| Servicios | ACTIVE | $5.88 | 863 | 21 | 2.43% | 1 | $5.88 |
| 🟡 PY \| Beco \| CP \| Conjuntos | ACTIVE | $6.19 | 990 | 17 | 1.72% | 1 | $6.19 |
| 🟡 GT \| Odoo \| CP \| Servicios | ACTIVE | $25.70 | 2,971 | 56 | 1.88% | 3 | $8.57 |
| 🔴 COL \| Odoo \| CP \| Servicios | ACTIVE | $6.96 | 541 | 11 | 2.03% | 0 | — (sin leads) |
| 🔴 GT \| Beco \| CP \| Conjuntos | ACTIVE | $14.01 | 1,553 | 36 | 2.32% | 0 | — (sin leads) |
| 🔴 SLV \| Beco \| CP \| Conjuntos | ACTIVE | $6.38 | 780 | 10 | 1.28% | 0 | — (sin leads) |
| ⚪ Evento: gestión de nómina (Odoo) | ACTIVE (EVENT_RESPONSES, no lead-gen) | sin datos* | sin datos* | sin datos* | —* | n/a | n/a |

\* La consulta de cierre no devolvió gasto/impresiones para esta campaña el 11-14, igual que el día anterior (11-13) — tercer día consecutivo sin datos. Se recomienda verificar en Ads Manager.

**Resto de la cuenta — todo PAUSED, sin cambios**: "[2026-08][Lead Generation][Odoo][GT/USA] - Toma El control de tu pyme", COL Odoo/Beco (versión anterior), ambos boosts de "Evento: Odoo en Acción", "...[COL] - Pyme Colombia", "...[SV] - Pyme El Salvador", "...[GT] - Beco", "...[GT] - Odoo Test", Accurate Partners - Loyalti, Conversión Clientes Potenciales MX/PY, 🟡 Conversión - Clientes Potenciales.

No se ejecutó ningún cambio de presupuesto, targeting ni creativo el 11-14 — ni desde esta rutina ni manualmente en Ads Manager (confirmado con `ads_account_get_activity_logs` para 2026-11-14 00:00–23:59 GT: array vacío).

---

## 📊 Análisis e Insights (actualizado con cifras de cierre)

1. **El cierre confirmado revirtió el resultado: 2026-11-14 fue en realidad el peor día de CPL blendeado de la serie reciente, no el mejor.** El cierre real generó 8 leads (no 14) con $72.06 de gasto (no $74.92) → CPL blendeado de **$9.01** (no $5.35) — por encima de la meta $6-7, y el peor cierre confirmado documentado en el vault hasta ahora.
2. **Es el primer caso documentado donde el cierre empeora frente a la lectura intradía.** En días anteriores (ej. 11-13: 8→15 leads, $9.03→$5.05 CPL) el lag de atribución de Meta siempre sumaba leads al confirmar. Aquí la lectura intradía reportó 14 leads y el cierre los redujo a 8 — y hasta impresiones (9,523→8,618) y clicks (201→177) bajaron, algo inusual. Se recomienda verificar en Ads Manager si hubo leads descalificados o clics filtrados por calidad.
3. **PY | Odoo no sostuvo su recuperación:** la lectura intradía la reportaba con 2 leads tras romper su racha negativa; el cierre confirma solo **1 lead** (CPL $5.88, no $2.71).
4. **Tres campañas cerraron en cero, no solo una:** COL Odoo y GT Beco, que la lectura intradía reportaba con 1 y 2 leads respectivamente, cerraron en 0 — se suman a SLV Beco. GT Beco es el caso más notorio: $14.01 de gasto sin ningún lead confirmado.
5. **GT | Odoo retrocedió en el cierre:** de 5 leads (intradía) a 3 leads confirmados, CPL de $5.09 a $8.57 — pasó de estar dentro de meta a superarla ampliamente.
6. **SLV | Odoo fue la única campaña que mejoró en el cierre:** de 2 a 3 leads, CPL de $2.93 a **$2.31** — la más eficiente de la cuenta por segundo día consecutivo.
7. **CTR blendeado de cierre: 2.05%** (vs. 2.11% reportado intradía), rompiendo la racha de 3 días de mejora consecutiva. Sigue por debajo de la meta 3-4%.
8. **Campaña de evento sigue sin datos:** tercer día consecutivo (11-13, 11-14, y la lectura intradía de 11-15) sin gasto, impresiones ni clicks para "Evento: gestión de nómina (Odoo)" — refuerza la sospecha de pausa de presupuesto, fin de campaña o anomalía de reporte persistente.
9. No se detectó investigación externa de competencia o tendencias de mercado adicional en esta corrección.

---

## ✏️ Cambios Realizados

Ninguno el 11-14. Solo se hizo lectura/análisis (`ads_get_ad_entities`, `ads_account_get_activity_logs`); no se modificó presupuesto, targeting, copy ni creativo de ninguna campaña. El 2026-11-15 solo se corrigieron las cifras de este archivo con los datos de cierre confirmados.

---

## 🔬 Investigación Realizada

- 11-14 (original): `ads_get_ad_entities` (`date_preset=today`) y `ads_account_get_activity_logs` (sin entradas).
- 11-15 (corrección): `ads_get_ad_entities` (`date_preset=yesterday`) para confirmar el cierre atribuido de 2026-11-14; `ads_account_get_activity_logs` para 2026-11-14 00:00–23:59 GT (sin entradas, confirma que la caída no se debió a cambios manuales en la cuenta).
- Se generó el Reporte Performance faltante de 2026-11-14: [[Reports/2026-11-14 - Reporte Performance]].
- Se detectó y corrigió un estado de `git` con HEAD detached y la rama local `main` desactualizada (4 commits detrás de `origin/main`); se restableció por fast-forward sin pérdida de historial.

---

## 📊 Datos Clave del Día (cifras de cierre)

| Métrica (blendeada, 7 campañas lead-gen) | 2026-11-14 (cierre) | 2026-11-14 (lectura intradía, obsoleta) | 2026-11-13 (día anterior, cierre) | Meta | Status |
|---|---|---|---|---|---|
| CPL Promedio | **$9.01** | $5.35 | $5.05 | $6-7 | 🔴 Sobre meta — peor cierre confirmado de la serie |
| Gasto Total (lead-gen) | $72.06 | $74.92 | $75.80 | - | — |
| Leads Totales | **8** | 14 | 15 | 4-5/día | 🟢 Sobre meta diaria, pero el cierre más bajo registrado |
| CTR Promedio | 2.05% | 2.11% | 2.12% | 3-4% | 🟡 Retrocede levemente, bajo meta |
| Impresiones (lead-gen) | 8,618 | 9,523 | 9,652 | - | — |
| Clicks (lead-gen) | 177 | 201 | 205 | - | — |
| Campañas activas sin ningún lead | 3 (COL Odoo, GT Beco, SLV Beco) | 1 (SLV Beco) | 1 (SLV Beco) | - | 🔴 Empeoró |
| Mejor campaña del día | SLV Odoo ($2.31 CPL, 3 leads) | PY Odoo ($2.71 CPL, 2 leads) | PY Odoo ($2.72 CPL, 2 leads) | - | — |
| Cambios de campaña ejecutados | 0 | 0 | 0 | - | - |

---

## 📋 Proximas Acciones

- [ ] **Verificar en Ads Manager si hubo leads descalificados o clics filtrados por calidad para 2026-11-14** — primer caso documentado donde el cierre empeora frente a la lectura intradía.
- [ ] Revisar con prioridad **GT | Beco** y **COL | Odoo**, que pasaron de tener leads en la lectura intradía a cero en el cierre.
- [ ] Dar seguimiento a **GT | Odoo** (CPL subió de $5.09 a $8.57 en el cierre) para distinguir ruido de un solo día de una tendencia negativa real.
- [ ] Verificar en Ads Manager el estado de "Evento: gestión de nómina (Odoo)" — ya acumula 3 días consecutivos sin gasto/métricas reportadas.
- [ ] Mantener el seguimiento a **SLV | Odoo**, única campaña con mejora sostenida dos días consecutivos ($2.93→$2.31 CPL).
- [ ] Ejecutar por fin el A/B test de los 5 copys nuevos documentado en [[CLAUDE.md]], aplicado a las 7 campañas país×producto activas — el CTR (2.05%) sigue por debajo de la meta 3-4%.
- [ ] Decidir con el usuario el futuro de la campaña histórica pausada "Toma El control de tu pyme" (reactivar, reemplazar formalmente por las campañas país×producto activas, o archivar).

---

## 🔗 Enlaces

- [[Reports/2026-11-14 - Reporte Performance]] — reporte de cierre completo generado el 2026-11-15.
- [[Reports/2026-11-13 - Reporte Performance]] — reporte de cierre previo en el vault.
- [[Daily notes/2026-11-13 - Resumen del Dia]] — resumen del día anterior.
- Tags: #daily-note #summary #meta-ads #octopus
