---
date: 2026-11-13
aliases: [resumen-2026-11-13]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-11-13

> [!warning] Corrección aplicada el 2026-11-14 (cifras de cierre)
> Este archivo se generó originalmente el propio 11-13 vía `ads_get_ad_entities` (`date_preset=today`), con datos parciales por el lag normal de atribución de Meta. El 2026-11-14 se consultó el cierre confirmado (`date_preset=yesterday`) y las cifras de abajo fueron **actualizadas para reflejar el cierre real**, que resultó notablemente mejor que la lectura intradía (15 leads vs. 8 reportados originalmente; CPL $5.05 vs. $9.03). Ver detalle completo en [[Reports/2026-11-13 - Reporte Performance]]. El original parcial queda documentado ahí mismo para comparación.

---

## 🎯 Campañas Revisadas (cifras de cierre confirmadas el 2026-11-14)

Se revisaron las 7 campañas activas de lead-gen + 1 de evento vía `ads_get_ad_entities` (nivel campaña, `date_preset=yesterday` desde el 2026-11-14):

| Campaña | Status | Gasto | Impresiones | Clicks | CTR | Leads | CPL |
|---|---|---|---|---|---|---|---|
| 🟢 GT \| Odoo \| CP \| Servicios | ACTIVE | $25.96 | 3,066 | 67 | 2.19% | 6 | **$4.33** |
| 🟢 SLV \| Odoo \| CP \| Servicios | ACTIVE | $5.87 | 813 | 17 | 2.09% | 2 | $2.94 |
| 🟢 PY \| Beco \| CP \| Conjuntos | ACTIVE | $7.70 | 1,292 | 33 | 2.55% | 2 | $3.85 |
| 🟢 PY \| Odoo \| CP \| Servicios | ACTIVE | $5.43 | 820 | 16 | 1.95% | 2 | **$2.72** |
| 🟡 COL \| Odoo \| CP \| Servicios | ACTIVE | $7.32 | 615 | 8 | 1.30% | 1 | $7.32 |
| 🟡 GT \| Beco \| CP \| Conjuntos | ACTIVE | $15.33 | 1,856 | 41 | 2.21% | 2 | $7.67 |
| 🔴 SLV \| Beco \| CP \| Conjuntos | ACTIVE | $8.19 | 1,190 | 23 | 1.93% | 0 | — (sin leads) |
| ⚪ Evento: gestión de nómina (Odoo) | ACTIVE (EVENT_RESPONSES, no lead-gen) | sin datos* | sin datos* | sin datos* | —* | n/a | n/a |

\* La consulta de cierre no devolvió gasto/impresiones para esta campaña el 11-13 (confirmado con consulta directa por ID); la lectura intradía original sí mostraba actividad ($2.89 / 5,816 impresiones / 128 clicks). Se recomienda verificar en Ads Manager.

**Resto de la cuenta — todo PAUSED, sin cambios**: "[2026-08][Lead Generation][Odoo][GT/USA] - Toma El control de tu pyme", COL Odoo/Beco (versión anterior), ambos boosts de "Evento: Odoo en Acción", "...[COL] - Pyme Colombia", "...[SV] - Pyme El Salvador", "...[GT] - Beco", "...[GT] - Odoo Test", Accurate Partners - Loyalti, Conversión Clientes Potenciales MX/PY, 🟡 Conversión - Clientes Potenciales.

No se ejecutó ningún cambio de presupuesto, targeting ni creativo el 11-13 — ni desde esta rutina ni manualmente en Ads Manager (confirmado con `ads_account_get_activity_logs` el día de la ejecución original).

---

## 📊 Análisis e Insights (actualizado con cifras de cierre)

1. **Mejor cierre confirmado de la cuenta hasta ahora:** el CPL blendeado real de 2026-11-13 fue **$5.05** (no $9.03 como se reportó intradía), con **15 leads** (no 8) — supera incluso el mejor día previo documentado (11-09, CPL $5.15). Esta es la corrección más significativa registrada hasta ahora entre lectura parcial y cierre.
2. **PY | Odoo rompió su racha de 3 días en cero:** la lectura intradía la reportaba en 0 leads por tercer día consecutivo; el cierre confirma **2 leads** ese mismo día con el mejor CPL de la cuenta ($2.72). La preocupación levantada en la versión original de esta nota ya no aplica.
3. **GT | Odoo** duplicó su resultado real frente a la lectura intradía: de 3 a 6 leads con el mismo gasto ($25.96), CPL de $4.33 — vuelve a ser el principal motor de volumen de la cuenta.
4. **SLV | Odoo** también mejoró en el cierre: de 1 a 2 leads, CPL de $7.00 a $2.94 — la campaña más eficiente del día junto con PY Odoo.
5. **Solo 1 de 7 campañas lead-gen cerró en cero (SLV | Beco)** — la mejor amplitud de cobertura de leads en la serie reciente.
6. **CTR blendeado de cierre: 2.12%** (vs. 1.86% reportado intradía) — mejora gradual sostenida, aunque sigue por debajo de la meta 3-4%. El diagnóstico de [[CLAUDE.md]] sobre copys genéricos sin urgencia sigue vigente.
7. **Lección operativa:** las lecturas `date_preset=today` siguen subestimando leads de forma significativa (en este caso casi a la mitad) por el lag de atribución de Meta. Se recomienda no tomar decisiones de pausa/presupuesto basadas únicamente en datos intradía.
8. No se detectó investigación externa de competencia o tendencias de mercado adicional en esta corrección.

---

## ✏️ Cambios Realizados

Ninguno el 11-13. Solo se hizo lectura/análisis (`ads_get_ad_entities`, `ads_account_get_activity_logs`); no se modificó presupuesto, targeting, copy ni creativo de ninguna campaña. El 2026-11-14 solo se corrigieron las cifras de este archivo con los datos de cierre confirmados.

---

## 🔬 Investigación Realizada

- 11-13 (original): `ads_get_ad_entities` (`date_preset=today`) y `ads_account_get_activity_logs` (sin entradas).
- 11-14 (corrección): `ads_get_ad_entities` (`date_preset=yesterday`) para confirmar el cierre atribuido de 2026-11-13; consulta adicional por `object_ids` para verificar la falta de datos de la campaña de evento.
- Se generó el Reporte Performance faltante de 2026-11-13: [[Reports/2026-11-13 - Reporte Performance]].
- Se detectó y corrigió un estado de `git` con HEAD detached (2 commits sin publicar); se restableció la rama `main` y se verificó que ya estaba sincronizada con `origin/main`.

---

## 📊 Datos Clave del Día (cifras de cierre)

| Métrica (blendeada, 7 campañas lead-gen) | 2026-11-13 (cierre) | 2026-11-13 (lectura intradía, obsoleta) | 2026-11-12 (día anterior, intradía) | Meta | Status |
|---|---|---|---|---|---|
| CPL Promedio | **$5.05** | $9.03 | $7.98 | $6-7 | 🟢 Por debajo de meta |
| Gasto Total (lead-gen) | $75.80 | $72.22 | $79.80 | - | — |
| Leads Totales | **15** | 8 | 10 | 4-5/día | 🟢 Triple de la meta diaria |
| CTR Promedio | 2.12% | 1.86% | 1.49% | 3-4% | 🟡 Mejora sostenida, bajo meta |
| Impresiones (lead-gen) | 9,652 | 9,744 | 11,105 | - | — |
| Clicks (lead-gen) | 205 | 181 | 166 | - | — |
| Campañas activas sin ningún lead | 1 (SLV Beco) | 2 (PY Odoo, SLV Beco) | 4 | - | 🟢 Mejor amplitud de la serie reciente |
| Mejor campaña del día | PY Odoo ($2.72 CPL, 2 leads) | PY Beco ($3.29 CPL, 2 leads) | GT Odoo ($5.47 CPL, 6 leads) | - | — |
| Cambios de campaña ejecutados | 0 | 0 | 0 | - | - |

---

## 📋 Proximas Acciones

- [ ] Tratar las lecturas `date_preset=today` como provisionales únicamente — este día mostró una subestimación de casi el 50% en leads frente al cierre. Evitar decisiones basadas solo en datos intradía.
- [ ] Investigar qué impulsó el salto real en GT | Odoo (3→6 leads) y SLV | Odoo (1→2 leads) entre la lectura intradía y el cierre — entender si es solo atribución tardía o también mejora de entrega.
- [ ] Dar seguimiento a **SLV | Beco**, única campaña en cero el 11-13, y vigilar el patrón de volatilidad día-por-día ya observado en reportes anteriores.
- [ ] Verificar en Ads Manager el gasto real de "Evento: gestión de nómina (Odoo)" para el 11-13 — la consulta de cierre no devolvió datos para esta campaña.
- [ ] Ejecutar por fin el A/B test de los 5 copys nuevos documentado en [[CLAUDE.md]], aplicado a las 7 campañas país×producto activas — el CTR (2.12%) sigue por debajo de meta pese a la mejora gradual.
- [ ] Decidir con el usuario el futuro de la campaña histórica pausada "Toma El control de tu pyme" (reactivar, reemplazar formalmente, o archivar).

---

## 🔗 Enlaces

- [[Reports/2026-11-13 - Reporte Performance]] — reporte de cierre completo generado el 2026-11-14.
- [[Reports/2026-11-11 - Reporte Performance]] — último reporte de cierre previo en el vault (no existe reporte propio de 2026-11-12).
- [[Daily notes/2026-11-12 - Resumen del Dia]] — resumen del día anterior.
- Tags: #daily-note #summary #meta-ads #octopus
