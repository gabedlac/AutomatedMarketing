---
date: 2026-11-13
aliases: [reporte-2026-11-13, performance-13-nov]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-11-13

> [!info] Nota sobre esta nota
> Generado el 2026-11-14 vía `ads_get_ad_entities` (`date_preset=yesterday`) para `act_2530001557366648` (GT | Octopus Innovations), que da el cierre final y atribuido de 2026-11-13. El archivo [[Daily notes/2026-11-13 - Resumen del Dia]] ya existía con cifras distintas (generadas el mismo 11-13 con `date_preset=today`, datos parciales por el lag normal de atribución de Meta); esta nota y la corrección aplicada a ese archivo usan los números de cierre confirmados abajo como la versión de referencia.

## 📋 Resumen Ejecutivo

| Métrica (blendeada, 7 campañas lead-gen) | Valor 2026-11-13 | Meta | Status |
|---|---|---|---|
| CPL Promedio | **$5.05 USD** | $6-7 | 🟢 Por debajo de meta — mejor cierre confirmado de la serie reciente |
| Gasto Total (lead-gen) | $75.80 USD | - | — |
| Gasto Total de cuenta (incl. evento) | $75.80 USD | - | — (sin gasto registrado en la campaña de evento este día, ver Notas) |
| Leads Totales | 15 | 4-5/día | 🟢 Triple de la meta diaria — mejor día confirmado hasta ahora |
| CTR Promedio | 2.12% | 3-4% | 🟡 Mejora sostenida, aún bajo meta |
| Impresiones (lead-gen) | 9,652 | - | — |
| Clicks (lead-gen) | 205 | - | — |
| ROAS | No aplica | - | Lead-gen sin pixel de valor de compra configurado |

**Lectura rápida:** el cierre confirmado de 2026-11-13 es el mejor día de la cuenta en la serie reciente — CPL blendeado de **$5.05** (dentro de meta, por debajo incluso del rango $6-7) con **15 leads**, el valor más alto registrado hasta ahora. Esto contrasta fuertemente con la lectura parcial del mismo día (generada con `date_preset=today`), que había reportado solo 8 leads y un CPL de $9.03 — una subestimación severa causada por el lag de atribución de Meta (los leads completan su atribución horas o incluso 1-2 días después del clic).

## 🎯 Performance por Campaña (2026-11-13, ranked por CPL)

| # | Campaña | Status | Gasto | Impresiones | Clicks | CTR | Leads | CPL |
|---|---|---|---|---|---|---|---|---|
| 1 | PY \| Odoo \| CP \| Servicios | 🟢 ACTIVE | $5.43 | 820 | 16 | 1.95% | 2 | **$2.72** |
| 2 | SLV \| Odoo \| CP \| Servicios | 🟢 ACTIVE | $5.87 | 813 | 17 | 2.09% | 2 | $2.94 |
| 3 | PY \| Beco \| CP \| Conjuntos | 🟢 ACTIVE | $7.70 | 1,292 | 33 | 2.55% | 2 | $3.85 |
| 4 | GT \| Odoo \| CP \| Servicios | 🟢 ACTIVE | $25.96 | 3,066 | 67 | 2.19% | 6 | $4.33 |
| 5 | COL \| Odoo \| CP \| Servicios | 🟡 ACTIVE | $7.32 | 615 | 8 | 1.30% | 1 | $7.32 |
| 6 | GT \| Beco \| CP \| Conjuntos | 🟡 ACTIVE | $15.33 | 1,856 | 41 | 2.21% | 2 | $7.67 |
| 7 | SLV \| Beco \| CP \| Conjuntos | 🔴 ACTIVE | $8.19 | 1,190 | 23 | 1.93% | 0 | — (sin leads) |
| — | Evento: gestión de nómina (Odoo) | ⚪ ACTIVE (Event Responses, no lead-gen) | $0.00* | 0* | 0* | —* | n/a | n/a |

\* La API no devolvió gasto/impresiones/clicks para esta campaña bajo `date_preset=yesterday` (se confirmó con una consulta directa por `object_ids`). La lectura parcial del mismo día había reportado $2.89 / 5,816 impresiones / 128 clicks — se recomienda verificar en Ads Manager si la campaña realmente no generó gasto atribuido a 11-13 en el cierre, o si es una limitación de la API para este tipo de campaña.

**Resto de la cuenta — todo PAUSED, sin cambios** (confirmado con `ads_account_get_activity_logs`, consultado para 2026-11-14 sin entradas aún): "[2026-08][Lead Generation][Odoo][GT/USA] - Toma El control de tu pyme" ⚠️ (campaña ancla de [[CLAUDE.md]], sigue sin reactivarse), COL Odoo/Beco (versión anterior), ambos boosts de "Evento: Odoo en Acción", "...[COL] - Pyme Colombia", "...[SV] - Pyme El Salvador", "...[GT] - Beco", "...[GT] - Odoo Test", Accurate Partners - Loyalti, Conversión Clientes Potenciales MX/PY, 🟡 Conversión - Clientes Potenciales.

## 💡 Insights Clave

1. **Mejor cierre confirmado de la cuenta hasta ahora:** CPL $5.05 con 15 leads supera incluso el mejor día previo mencionado en reportes anteriores (11-09, CPL $5.15). El gasto lead-gen ($75.80) se mantuvo cerca del promedio de días recientes, por lo que la mejora vino de volumen de leads, no de recorte de presupuesto.
2. **La lectura parcial del mismo día subestimó gravemente el resultado:** el Daily note generado el propio 11-13 (`date_preset=today`) reportó 8 leads / CPL $9.03; el cierre confirmado es 15 leads / CPL $5.05. Casi todas las campañas terminaron con más leads de los que mostraba la lectura intradía — en particular **GT | Odoo** (3→6 leads) y **SLV | Odoo** (1→2 leads, CPL de $7.00 a $2.94). Esto confirma el patrón de lag de atribución ya documentado el 11-11 y refuerza que las lecturas `today` deben tratarse como provisionales.
3. **PY | Odoo rompió su racha de ceros:** el Daily note del 11-13 la reportaba en 0 leads por tercer día consecutivo (11-11 a 11-13); el cierre confirmado muestra **2 leads** ese mismo día, con el mejor CPL de la cuenta ($2.72). La "crisis" de 3 días sin leads reportada en tiempo real no era correcta — se corrige en el Daily note.
4. **Solo 1 de 7 campañas lead-gen cerró en cero (SLV | Beco)** — la mejor amplitud de cobertura de leads en la serie reciente (vs. 2-4 campañas en cero en días anteriores).
5. **CTR blendeado sigue mejorando de forma gradual:** 2.12% (vs. 1.86% el 11-12 intradía, y ~1.5% en días previos), aunque todavía por debajo de la meta 3-4%. El diagnóstico de [[CLAUDE.md]] sobre copys genéricos sin urgencia sigue vigente — las 7 campañas activas nunca recibieron el A/B test de los 5 copys nuevos (pensado originalmente para la campaña GT pausada "Toma El control de tu pyme").
6. **Dato faltante en la campaña de evento:** la consulta de cierre no devolvió gasto/impresiones para "Evento: gestión de nómina" en 11-13, a diferencia de la lectura intradía que sí mostraba actividad. No afecta las métricas blendeadas de lead-gen (que excluyen esta campaña), pero se señala como punto a verificar.
7. **ROAS no aplica** — cuenta 100% lead-gen sin pixel de valor de compra configurado para estas campañas.

## ✅ Recomendaciones Accionables

- [ ] **Tratar las lecturas `date_preset=today` como provisionales únicamente** — este reporte confirma que pueden subestimar leads en 40-90% frente al cierre del día siguiente. Evitar decisiones de pausa/presupuesto basadas solo en datos intradía (como casi ocurrió con PY | Odoo).
- [ ] **Investigar la causa del salto en GT | Odoo** (3→6 leads intradía→cierre) y **SLV | Odoo** (1→2) para entender si es solo atribución tardía o también una mejora real de entrega — podría ayudar a replicar el patrón.
- [ ] Revisar **SLV | Beco**, única campaña en cero este día, y vigilar si repite el patrón de volatilidad día-por-día ya observado (0↔1 lead) en reportes anteriores.
- [ ] Verificar en Ads Manager el gasto real de "Evento: gestión de nómina (Odoo)" para 2026-11-13 — la discrepancia entre lectura intradía y cierre sugiere revisar si hay un problema de datos específico de esa campaña.
- [ ] Ejecutar por fin el A/B test de los 5 copys nuevos documentado en [[CLAUDE.md]], aplicado a las 7 campañas país×producto activas, dado que el CTR (2.12%) sigue por debajo de la meta 3-4% pese a la mejora gradual.
- [ ] Decidir con el usuario si la campaña histórica "[2026-08][Lead Generation][Odoo][GT] - Toma El control de tu pyme" se reactiva, se reemplaza formalmente por las campañas país×producto activas, o se archiva — sigue pausada y las tareas activas de [[CLAUDE.md]] todavía la referencian.

## 🔗 Seguimiento

- Daily note del día (corregido con cifras de cierre): [[Daily notes/2026-11-13 - Resumen del Dia]]
- Reporte anterior disponible: [[Reports/2026-11-11 - Reporte Performance]] (no existe reporte propio de 2026-11-12 en el vault)
- Contexto de cuenta y metas: [[CLAUDE.md]]

#daily-note #performance #meta-ads #octopus
