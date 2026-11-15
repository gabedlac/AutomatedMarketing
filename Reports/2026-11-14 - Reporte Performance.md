---
date: 2026-11-14
aliases: [reporte-2026-11-14, performance-14-nov]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-11-14

> [!info] Nota sobre esta nota
> Generado el 2026-11-15 vía `ads_get_ad_entities` (`date_preset=yesterday`) para `act_2530001557366648` (GT | Octopus Innovations), que da el cierre final y atribuido de 2026-11-14. El archivo [[Daily notes/2026-11-14 - Resumen del Dia]] ya existía con cifras distintas (generadas el mismo 11-14 con `date_preset=today`, datos parciales por el lag normal de atribución de Meta); esta nota y la corrección aplicada a ese archivo usan los números de cierre confirmados abajo como la versión de referencia.
>
> **A diferencia de los cierres anteriores documentados en el vault (que mejoraron frente a la lectura intradía), el cierre de 2026-11-14 empeoró:** leads cayeron de 14 (intradía) a 8 (cierre), y el CPL subió de $5.35 a $9.01. Ver Insight #1 para detalle.

## 📋 Resumen Ejecutivo

| Métrica (blendeada, 7 campañas lead-gen) | Valor 2026-11-14 | Meta | Status |
|---|---|---|---|
| CPL Promedio | **$9.01** | $6-7 | 🔴 Sobre meta — el peor cierre confirmado de la serie reciente |
| Gasto Total (lead-gen) | $72.06 | - | — |
| Leads Totales | 8 | 4-5/día | 🟢 Por encima de la meta diaria, pero el cierre más bajo de la serie reciente |
| CTR Promedio | 2.05% | 3-4% | 🟡 Bajo meta, retrocede levemente vs. el cierre anterior (2.12%) |
| Impresiones (lead-gen) | 8,618 | - | — |
| Clicks (lead-gen) | 177 | - | — |
| ROAS | No aplica | - | Lead-gen sin pixel de valor de compra configurado |

**Lectura rápida:** el cierre confirmado de 2026-11-14 es el **peor día de la cuenta en la serie reciente documentada en el vault** — CPL blendeado de **$9.01** (por encima de la meta $6-7) con solo **8 leads**, muy por debajo del pico de 15 leads del cierre de 11-13. Esto es notable porque **invierte el patrón habitual**: en los cierres anteriores (ej. 11-13), el dato confirmado siempre mejoraba frente a la lectura intradía por el lag de atribución de Meta. Aquí ocurrió lo contrario — la lectura intradía del propio 11-14 (`date_preset=today`) había reportado 14 leads y CPL $5.35, y el cierre confirmado los revirtió a 8 leads y CPL $9.01. Incluso impresiones (9,523→8,618) y clicks (201→177) bajaron, lo cual es inusual porque normalmente solo pueden mantenerse o subir al cerrar el día — ver Insight #1.

## 🎯 Performance por Campaña (2026-11-14, ranked por CPL)

| # | Campaña | Status | Gasto | Impresiones | Clicks | CTR | Leads | CPL |
|---|---|---|---|---|---|---|---|---|
| 1 | SLV \| Odoo \| CP \| Servicios | 🟢 ACTIVE | $6.94 | 920 | 26 | 2.83% | 3 | **$2.31** |
| 2 | PY \| Odoo \| CP \| Servicios | 🟡 ACTIVE | $5.88 | 863 | 21 | 2.43% | 1 | $5.88 |
| 3 | PY \| Beco \| CP \| Conjuntos | 🟡 ACTIVE | $6.19 | 990 | 17 | 1.72% | 1 | $6.19 |
| 4 | GT \| Odoo \| CP \| Servicios | 🟡 ACTIVE | $25.70 | 2,971 | 56 | 1.88% | 3 | $8.57 |
| 5 | COL \| Odoo \| CP \| Servicios | 🔴 ACTIVE | $6.96 | 541 | 11 | 2.03% | 0 | — (sin leads) |
| 6 | GT \| Beco \| CP \| Conjuntos | 🔴 ACTIVE | $14.01 | 1,553 | 36 | 2.32% | 0 | — (sin leads) |
| 7 | SLV \| Beco \| CP \| Conjuntos | 🔴 ACTIVE | $6.38 | 780 | 10 | 1.28% | 0 | — (sin leads) |
| — | Evento: gestión de nómina (Odoo) | ⚪ ACTIVE (Event Responses, no lead-gen) | sin datos* | sin datos* | sin datos* | —* | n/a | n/a |

\* La API no devolvió gasto/impresiones/clicks para esta campaña bajo `date_preset=yesterday`, igual que el día anterior (11-13) — ya es el tercer día consecutivo sin datos para esta campaña (11-13, 11-14, 11-15 según la lectura intradía de hoy). Refuerza la sospecha de que la campaña está pausada, agotó presupuesto/calendario o hay una anomalía de reporte persistente; se recomienda verificar directamente en Ads Manager.

**Resto de la cuenta — todo PAUSED, sin cambios** (confirmado con `ads_account_get_activity_logs` para 2026-11-14 00:00–23:59 GT: array vacío, sin entradas): "[2026-08][Lead Generation][Odoo][GT/USA] - Toma El control de tu pyme" ⚠️ (campaña ancla de [[CLAUDE.md]], sigue sin reactivarse), COL Odoo/Beco (versión anterior), ambos boosts de "Evento: Odoo en Acción", "...[COL] - Pyme Colombia", "...[SV] - Pyme El Salvador", "...[GT] - Beco", "...[GT] - Odoo Test", Accurate Partners - Loyalti, Conversión Clientes Potenciales MX/PY, 🟡 Conversión - Clientes Potenciales.

## 💡 Insights Clave

1. **El cierre confirmado invirtió el patrón habitual y resultó peor que la lectura intradía — el primer caso así documentado en el vault.** En los cierres anteriores (ej. 11-13: 8→15 leads, $9.03→$5.05 CPL), el lag de atribución de Meta siempre sumaba leads adicionales al confirmar el día. Aquí ocurrió lo contrario: 14→8 leads, $5.35→$9.01 CPL. Impresiones (9,523→8,618) y clicks (201→177) también bajaron, algo que normalmente no debería pasar al cerrar el día. Esto sugiere una posible depuración de tráfico/leads inválidos por parte de Meta al finalizar la atribución, o una anomalía de datos — se recomienda verificar en Ads Manager si hay leads descalificados o clics filtrados por calidad para 2026-11-14.
2. **Peor cierre confirmado de la cuenta en la serie reciente:** CPL $9.01 supera incluso el peor dato intradía documentado anteriormente ($9.03 del 11-13, que terminó corrigiéndose a $5.05). Es la primera vez que un cierre confirmado queda por encima de $9.
3. **Tres campañas cayeron a cero leads en el cierre, todas con lead en la lectura intradía:** COL Odoo (1→0), GT Beco (2→0) y PY Beco (2→1, no llegó a cero pero cayó). GT Beco es el caso más notorio: gastó $14.01 sin ningún lead confirmado, el mayor gasto sin conversión del día.
4. **GT | Odoo, el mayor volumen de la cuenta, retrocedió en el cierre:** de 5 leads (intradía) a 3 leads confirmados, con CPL subiendo de $5.09 a $8.57 — pasó de estar dentro de meta a superarla ampliamente.
5. **SLV | Odoo fue la única campaña que mejoró en el cierre:** de 2 a 3 leads, con el mejor CPL de la cuenta ($2.31, vs $2.93 intradía) — segundo día consecutivo como la campaña más eficiente.
6. **CTR blendeado retrocede levemente a 2.05%** (vs. 2.12% del cierre de 11-13), rompiendo la racha de mejora gradual documentada en reportes previos. Sigue por debajo de la meta 3-4%; el diagnóstico de [[CLAUDE.md]] sobre copys genéricos sin urgencia sigue vigente — las 7 campañas activas nunca recibieron el A/B test de los 5 copys nuevos.
7. **ROAS no aplica** — cuenta 100% lead-gen sin pixel de valor de compra configurado para estas campañas.

## ✅ Recomendaciones Accionables

- [ ] **Verificar en Ads Manager si hubo leads descalificados o clics filtrados por calidad para 2026-11-14** — es el primer día documentado en que el cierre confirmado empeora frente a la lectura intradía, lo contrario del patrón de lag de atribución visto hasta ahora.
- [ ] **Revisar con prioridad GT | Beco y COL | Odoo**, que pasaron de tener leads en la lectura intradía a cero en el cierre — confirmar si es un problema de atribución o una señal real de fatiga de creativo/audiencia.
- [ ] **Dar seguimiento a GT | Odoo** (CPL subió de $5.09 a $8.57 en el cierre) para distinguir entre ruido de un solo día y una tendencia negativa real.
- [ ] Verificar en Ads Manager el estado de "Evento: gestión de nómina (Odoo)" — ya acumula 3 días consecutivos sin gasto/métricas reportadas.
- [ ] Mantener el seguimiento a **SLV | Odoo**, única campaña con mejora sostenida dos días consecutivos ($2.93→$2.31 CPL) — candidata a incremento de presupuesto si la tendencia se confirma.
- [ ] Ejecutar por fin el A/B test de los 5 copys nuevos documentado en [[CLAUDE.md]], aplicado a las 7 campañas país×producto activas, dado que el CTR (2.05%) sigue por debajo de la meta 3-4%.
- [ ] Decidir con el usuario si la campaña histórica "[2026-08][Lead Generation][Odoo][GT] - Toma El control de tu pyme" se reactiva, se reemplaza formalmente por las campañas país×producto activas, o se archiva.

## 🔗 Seguimiento

- Daily note del día (corregido con cifras de cierre): [[Daily notes/2026-11-14 - Resumen del Dia]]
- Reporte anterior disponible: [[Reports/2026-11-13 - Reporte Performance]]
- Contexto de cuenta y metas: [[CLAUDE.md]]

#daily-note #performance #meta-ads #octopus
