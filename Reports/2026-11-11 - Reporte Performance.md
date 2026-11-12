---
date: 2026-11-11
aliases: [reporte-2026-11-11, performance-11-nov]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-11-11

> [!info] Nota sobre esta nota
> Generado el 2026-11-12 vía `ads_get_ad_entities` (`date_preset=yesterday`) para `act_2530001557366648` (GT | Octopus Innovations), que da el cierre final y atribuido de 2026-11-11. El archivo [[Daily notes/2026-11-11 - Resumen del Dia]] ya existía con cifras distintas (generadas el mismo 11-11, probablemente con datos parciales/no cerrados todavía); esta nota y la actualización de ese archivo usan los números de cierre confirmados abajo como la versión de referencia.

## 📋 Resumen Ejecutivo

| Métrica (blendeada, 7 campañas lead-gen) | Valor 2026-11-11 | Meta | Status |
|---|---|---|---|
| CPL Promedio | $8.10 USD | $6-7 | 🟡 Por encima de meta, pero mejora fuerte vs. 11-10 ($11.44) |
| Gasto Total (lead-gen) | $80.98 USD | - | — |
| Gasto Total de cuenta (incl. evento) | $86.98 USD | - | — |
| Leads Totales | 10 | 4-5/día | 🟢 El doble de la meta diaria |
| CTR Promedio | 1.48% | 3-4% | 🔴 Muy por debajo de meta |
| Impresiones (lead-gen) | 11,296 | - | — |
| Clicks (lead-gen) | 167 | - | — |
| ROAS | No aplica | - | Lead-gen sin pixel de valor de compra configurado |

**Lectura rápida:** el CPL blendeado mejoró de forma marcada frente al día anterior — de $11.44 (2026-11-10) a **$8.10**, acercándose a la meta $6-7 — con 10 leads (el mejor día de la semana reciente) y un gasto menor (-21% vs. 11-10). El CTR se mantiene estructuralmente bajo (1.48% vs meta 3-4%), sin cambios relevantes.

## 🎯 Performance por Campaña (2026-11-11, ranked por CPL)

| # | Campaña | Status | Gasto | Impresiones | Clicks | CTR | Leads | CPL |
|---|---|---|---|---|---|---|---|---|
| 1 | SLV \| Odoo \| CP \| Servicios | 🟢 ACTIVE | $8.66 | 1,374 | 21 | 1.53% | 3 | **$2.89** |
| 2 | GT \| Odoo \| CP \| Servicios | 🟢 ACTIVE | $33.28 | 4,368 | 80 | 1.83% | 6 | $5.55 |
| 3 | PY \| Beco \| CP \| Conjuntos | 🟡 ACTIVE | $6.09 | 1,053 | 6 | 0.57% | 1 | $6.09 |
| 4 | COL \| Odoo \| CP \| Servicios | 🔴 ACTIVE | $7.04 | 661 | 7 | 1.06% | 0 | — (sin leads) |
| 5 | SLV \| Beco \| CP \| Conjuntos | 🔴 ACTIVE | $6.09 | 1,020 | 8 | 0.78% | 0 | — (sin leads) |
| 6 | GT \| Beco \| CP \| Conjuntos | 🔴 ACTIVE | $14.72 | 1,985 | 34 | 1.71% | 0 | — (sin leads) |
| 7 | PY \| Odoo \| CP \| Servicios | 🔴 ACTIVE | $5.10 | 835 | 11 | 1.32% | 0 | — (sin leads) |
| — | Evento: gestión de nómina (Odoo) | ⚪ ACTIVE (Event Responses, no lead-gen) | $6.00 | 10,772 | 250 | 2.32% | n/a (58 RSVP) | n/a |

**Resto de la cuenta — todo PAUSED, sin cambios (confirmado con `ads_account_get_activity_logs`, vacío para 2026-11-11):** "[2026-08][Lead Generation][Odoo][GT] - Toma El control de tu pyme" ⚠️ (campaña ancla de [[CLAUDE.md]], sigue sin reactivarse), "...[USA]", "...[COL] - Pyme Colombia", "...[SV] - Pyme El Salvador", "...[GT] - Beco", "...[GT] - Odoo Test", COL Odoo/Beco (versión anterior), ambos boosts de "Evento: Odoo en Acción", Accurate Partners - Loyalti, Conversión Clientes Potenciales MX/PY, 🟡 Conversión - Clientes Potenciales.

## 💡 Insights Clave

1. **Mejora de fondo, no solo ruido de atribución:** 10 leads con $80.98 de gasto lead-gen (-21% vs 11-10) da un CPL de $8.10, el mejor cierre confirmado desde el 11-09 ($5.15). La mejora viene sobre todo de **GT | Odoo**, que pasó de 2 leads/$34.19 (11-10) a **6 leads/$33.28** (11-11) con gasto casi idéntico — volvió a ser el motor de la cuenta en vez de su mayor lastre.
2. **SLV | Odoo** sigue siendo la campaña más eficiente de la cuenta por tercer día consecutivo: CPL $2.89 (vs $3.44 el 11-10), 3 leads.
3. **4 de 7 campañas lead-gen cerraron el día sin ningún lead** (COL Odoo, SLV Beco, GT Beco, PY Odoo) pese a gasto sostenido (~$5-15/día cada una) — el mismo patrón de alerta de días anteriores. PY Odoo lleva ya 2 días consecutivos en cero.
4. **CTR sigue estructuralmente bajo** (1.48% vs meta 3-4%), prácticamente sin cambio frente a 11-10 (1.53%) — el diagnóstico de [[CLAUDE.md]] sobre copys genéricos sin urgencia sigue vigente para las 7 campañas activas, que nunca recibieron el A/B test de los 5 copys nuevos (ese test seguía pensado para la campaña GT pausada "Toma El control de tu pyme").
5. **ROAS no aplica** — cuenta 100% lead-gen sin pixel de valor de compra configurado para estas campañas.
6. **Discrepancia de datos detectada:** la nota [[Daily notes/2026-11-11 - Resumen del Dia]], generada el mismo 11-11 con `date_preset=today`, mostraba cifras más altas de gasto (ej. GT Odoo $33.30 con solo 2 leads) para la misma fecha. Esta nota usa el cierre confirmado al día siguiente (`date_preset=yesterday` desde el 11-12), que es la fuente más confiable por el lag normal de atribución de Meta; se corrigió el archivo de Daily notes para que ambos coincidan.

## ✅ Recomendaciones Accionables

- [ ] **Investigar qué cambió en GT | Odoo** entre el 11-10 y el 11-11 (mismo gasto, leads de 2→6) para intentar replicarlo — podría ser variación normal o un cambio real de audiencia/entrega que conviene entender antes de tocar presupuesto.
- [ ] Revisar landing page y formulario de **PY | Odoo** (2 días consecutivos en cero leads) antes de seguir gastando ~$5/día ahí sin resultados.
- [ ] Evaluar pausar o reestructurar **COL | Odoo**, **SLV | Beco** y **GT | Beco** si no generan ningún lead un día más — juntas representan ~$28/día sin conversión hoy.
- [ ] Ejecutar por fin el A/B test de los 5 copys nuevos documentado en [[CLAUDE.md]] — pero aplicado a las 7 campañas país×producto activas (no a la campaña GT original, que sigue pausada), ya que el CTR bajo (1.48%) es un síntoma transversal a toda la estructura actual.
- [ ] Decidir con el usuario si la campaña histórica "[2026-08][Lead Generation][Odoo][GT] - Toma El control de tu pyme" se reactiva, se reemplaza formalmente por "GT | Odoo | CP | Servicios", o se archiva — sigue pausada desde hace varios días y las tareas activas de [[CLAUDE.md]] todavía la referencian.

## 🔗 Seguimiento

- Daily note del día: [[Daily notes/2026-11-11 - Resumen del Dia]]
- Reporte anterior: [[Reports/2026-11-10 - Reporte Performance]]
- Contexto de cuenta y metas: [[CLAUDE.md]]

#daily-note #performance #meta-ads #octopus
