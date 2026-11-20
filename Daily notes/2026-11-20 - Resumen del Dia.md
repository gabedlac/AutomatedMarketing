---
date: 2026-11-20
aliases: [resumen-2026-11-20]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-11-20

> [!warning] Nota sobre la fecha y los datos (mismo desajuste de zona horaria de rutinas anteriores)
> Esta rutina se ejecutó a las **05:52 UTC del 20-nov** (≈ 23:52 del 2026-11-19 en `America/Guatemala`, zona horaria de la cuenta `act_2530001557366648`). A esa hora el día local de la cuenta **todavía no cambiaba a 2026-11-20** (faltaban ~8 minutos): `date_preset=today` resolvió a **2026-11-19** y `date_preset=yesterday` resolvió a **2026-11-18** (datos finales, consistentes con [[Reports/2026-11-18 - Reporte Performance]]). Por lo tanto, los datos de "hoy" en esta nota corresponden en realidad al día **2026-11-19** (provisional, faltan ~8 minutos de cierre) y la comparación es contra **2026-11-18** (final, verificado). Se mantiene el nombre de archivo `2026-11-20` siguiendo el mismo patrón de rutinas anteriores (fecha del sistema al momento de ejecutarse) — mismo desajuste ya documentado en las notas del 18-nov y 19-nov. Es probable que una rutina posterior corrija esta nota con los números finales una vez cierre formalmente el día.
>
> **Hallazgo de higiene de repo corregido en esta rutina:** al iniciar, `HEAD` estaba detached en el commit `c1e75ed` ("Add Daily Performance Report - 2026-11-18"), 4 commits por delante de `main`/`origin/main` (que seguían en `23360d1`, el reporte del 16-nov). Esto significaba que las notas de `Daily notes/2026-11-18`, `Daily notes/2026-11-19`, `Reports/2026-11-17` y `Reports/2026-11-18` existían en el working tree pero **nunca se habían fusionado a `main` ni publicado a `origin`** por rutinas anteriores. Se verificó que era un fast-forward limpio (`main` ancestro directo de `HEAD`) y se corrigió: `git checkout main && git merge --ff-only c1e75ed && git push`. `main` y `origin/main` quedaron sincronizados en `c1e75ed` antes de continuar con esta nota.
>
> **Corrección posterior (rutina del 20-nov 13:08 UTC, 7:08am Guatemala — día ya cerrado formalmente):** las cifras de esta nota eran **provisionales** (faltaban ~8 min de cierre). Se verificaron contra `date_preset=yesterday` y un `time_range` explícito para 2026-11-19, ambos idénticos entre sí → datos finales confirmados. Se actualizó la tabla "Datos Clave del Día" con los números finales: gasto $67.08 → **$68.30** (+$1.22 por atribución tardía), CPL $9.58 → **$9.76**, CTR ~2.07% → **2.03%**, impresiones 9,560 → **9,740**; leads (7) y clicks (198) sin cambio. El detalle completo y verificado, incluyendo el desglose final por campaña, está en [[Reports/2026-11-19 - Reporte Performance]].
>
> **Segundo hallazgo de higiene de repo (rutina del 20-nov 13:08 UTC):** al iniciar esta corrección, `HEAD` volvía a estar detached, en el commit `27638ec` ("Add Daily Summary - 2026-11-20"), con la rama local `main` 5 commits por detrás (todavía en `23360d1`). A diferencia de rutinas anteriores, `origin/main` ya estaba sincronizado en `27638ec` — fue solo un desajuste de la copia local, no una falta de push. Se corrigió con `git fetch origin && git checkout main && git merge --ff-only origin/main`.

---

## 🎯 Campañas Revisadas

Se revisaron las 7 campañas activas de lead-gen + 1 de evento vía `ads_get_ad_entities` (nivel campaña, `date_preset=today`, equivalente a 2026-11-19 casi cerrado en zona horaria de la cuenta):

| Campaña | Status | Gasto | Impresiones | Clicks | CTR | Leads | CPL |
|---|---|---|---|---|---|---|---|
| 🟢 GT \| Odoo \| CP \| Servicios | ACTIVE | $23.07 | 3,268 | 83 | 2.54% | 4 | **$5.77** |
| 🟢 PY \| Odoo \| CP \| Servicios | ACTIVE | $5.99 | 1,049 | 20 | 1.91% | 1 | $5.99 |
| 🟢 SLV \| Odoo \| CP \| Servicios | ACTIVE | $6.10 | 1,087 | 23 | 2.12% | 1 | $6.10 |
| 🟢 COL \| Odoo \| CP \| Servicios | ACTIVE | $7.11 | 622 | 13 | 2.09% | 1 | $7.11 |
| 🔴 PY \| Beco \| CP \| Conjuntos | ACTIVE | $7.06 | 1,125 | 15 | 1.33% | 0 | — (sin leads) |
| 🔴 SLV \| Beco \| CP \| Conjuntos | ACTIVE | $5.97 | 984 | 17 | 1.73% | 0 | — (sin leads) |
| 🔴 GT \| Beco \| CP \| Conjuntos | ACTIVE | $11.78 | 1,425 | 27 | 1.89% | 0 | — (sin leads) |
| ⚪ Evento: gestión de nómina (Odoo) | ACTIVE (EVENT_RESPONSES, no lead-gen) | sin datos | sin datos | sin datos | — | n/a | n/a |

**Resto de la cuenta — todo PAUSED** (13 campañas, sin cambios desde días anteriores): COL \| Beco \| CP \| Conjuntos, COL \| Odoo \| CP \| Servicios (versión de prueba anterior), 2x boosts de "Evento: Odoo en Acción", "[2026-08][Lead Generation][Odoo][COL] - Pyme Colombia", "...[USA] - Toma El control de tu pyme", "...[GT] - Toma El control de tu pyme", Accurate Partners - Loyalti, "...[GT] - Odoo Test", "...[GT] - Beco", Conversión Clientes Potenciales MX/PY, "...[SV] - Pyme El Salvador", 🟡 Conversión - Clientes Potenciales.

`ads_account_get_activity_logs` para el rango 2026-11-19 06:00 – 2026-11-20 06:30 UTC **no devolvió ningún evento** (ni cambios manuales ni el cargo automático de facturación de Meta, que todavía no ocurre porque el día local no ha cerrado). No se ejecutó ningún cambio de presupuesto, targeting ni creativo hoy.

---

## 📊 Análisis e Insights

1. **Patrón claro por línea de producto, no por geografía:** las 4 campañas de **Odoo | Servicios** (GT, PY, SLV, COL) generaron leads hoy (4, 1, 1 y 1 respectivamente); las 3 campañas de **Beco | Conjuntos** (PY, SLV, GT) quedaron **todas en cero leads** simultáneamente. Es la primera vez que se observa esta división tan limpia por producto en lugar de por país — merece revisión de creativo/oferta de la línea Beco en las tres geografías a la vez.
2. **GT \| Odoo revierte con fuerza su racha negativa de 3 días:** tras caer de 9→4→2 leads (16, 17, 18-nov) con CPL subiendo $3.56→$7.82→$12.53, hoy repunta a **4 leads / $5.89 CPL** (final, verificado; -53.0% de CPL vs. ayer), su mejor resultado desde el 17-nov y la campaña con mejor performance de la cuenta hoy. Rompe la tendencia de deterioro que se venía señalando como acción pendiente.
3. **GT \| Beco cae a cero tras su peor CPL registrado:** de 1 lead/$15.43 CPL ayer (el peor CPL individual de la cuenta) a 0 leads hoy — segunda señal negativa consecutiva, ya no parece ruido de un solo día.
4. **PY \| Beco no sostiene su recuperación:** había roto una racha de 2+ días en cero con 2 leads/$4.32 CPL ayer; hoy vuelve a 0 leads — confirma que fue un repunte puntual, no una tendencia.
5. **COL \| Odoo se recupera:** de 0 leads ayer a 1 lead hoy ($7.11 CPL, dentro de meta).
6. **SLV \| Beco sigue en cero por segundo día consecutivo** — ya no es un evento aislado, requiere revisión de creativo/audiencia.
7. **CPL blendeado mejora con fuerza:** 7 leads con $68.30 de gasto (final, verificado) → CPL blendeado **$9.76**, -13.2% vs. los $11.24 (final) del 18-nov, aunque sigue por encima del rango meta $6-7.
8. **Leads totales se mantienen en 7**, igual que ayer, pero con una distribución muy distinta: ayer repartidos entre 5 campañas (2 en cero), hoy concentrados en 4 campañas (3 en cero) — mayor concentración de riesgo en GT \| Odoo.
9. **CTR blendeado mejora a 2.03%** (final, verificado; vs. 1.81% final de ayer, +12.2%), impulsado principalmente por GT \| Odoo (2.48%) y SLV/COL \| Odoo (>2%); sigue por debajo de la meta 3-4%.
10. **`ads_insights_anomaly_signal` no detectó anomalías** (solapamiento de subasta, fatiga de creativo o audiencia estrecha) en los ad sets analizados.
11. **Campaña de evento sigue sin datos** ("Evento: gestión de nómina (Odoo)" ACTIVE, sin gasto/impresiones/clicks reportados por ~7º día consecutivo). `ads_get_errors` no devolvió ningún error de entrega bloqueante.
12. No hubo ninguna otra sesión de Claude Code activa en la cuenta hoy aparte de esta rutina, y no se realizó investigación externa de competencia o tendencias de mercado.
13. **Dato ya cerrado y verificado:** como se explica en la nota de advertencia arriba, los números de esta nota eran provisionales (faltaban ~8 minutos de cierre) y fueron corregidos con los datos finales en esta misma rutina (20-nov, 7:08am Guatemala); la variación final fue menor (+$1.22 en gasto, CPL $9.58→$9.76, CTR ~2.07%→2.03%, leads y clicks sin cambio). El detalle completo y el desglose final por campaña están en [[Reports/2026-11-19 - Reporte Performance]].

---

## ✏️ Cambios Realizados

Ninguno en Meta Ads. Solo se hizo lectura/análisis (`ads_get_ad_entities`, `ads_account_get_activity_logs`, `ads_insights_anomaly_signal`, `ads_get_errors`); no se modificó presupuesto, targeting, copy ni creativo de ninguna campaña desde esta rutina ni se detectaron cambios manuales en Ads Manager (sin eventos registrados en el log de actividad del día).

**Cambio técnico/de repositorio:** se corrigió el `HEAD` detached descrito en la nota de advertencia (fast-forward de `main` a `c1e75ed` + push a `origin/main`), dejando el repositorio sincronizado antes de crear esta nota.

---

## 🔬 Investigación Realizada

- Se consultó `ads_get_ad_entities` (nivel campaña y cuenta, `act_2530001557366648`) con `date_preset=today` y `date_preset=yesterday`, y se verificó la zona horaria real de la cuenta (`timezone_name=America/Guatemala`) para confirmar a qué día calendario corresponde cada dato.
- Se consultó `ads_account_get_activity_logs` para el rango 2026-11-19 06:00 – 2026-11-20 06:30 UTC: sin resultados (ni cambios manuales ni facturación automática, consistente con que el día local aún no cerró).
- Se ejecutó `ads_insights_anomaly_signal` sobre la cuenta: sin anomalías de solapamiento de subasta, fatiga de creativo o audiencia estrecha.
- Se ejecutó `ads_get_errors` sobre la campaña de evento sin delivery: sin errores bloqueantes de publicación.
- Se comparó campaña por campaña contra los datos finales verificados de [[Reports/2026-11-18 - Reporte Performance]] para identificar el patrón por línea de producto (Odoo vs. Beco) descrito en Insights.
- Se auditó `git status`/`git log`/`git branch -a`: se detectó y corrigió un `HEAD` detached 4 commits por delante de `main`/`origin/main` (ver advertencia arriba); tras la corrección, repo limpio y sincronizado.
- No se realizó investigación externa de competencia ni tendencias de mercado.

---

## 📊 Datos Clave del Día

| Métrica (blendeada, 7 campañas lead-gen) | 2026-11-19 (final, verificado) | 2026-11-18 (final, verificado) | Meta | Status |
|---|---|---|---|---|
| CPL Promedio | **$9.76** | $11.24 | $6-7 | 🟡 Mejora fuerte (-13.2%) pero sigue fuera de meta |
| Gasto Total (lead-gen) | $68.30 | $78.69 | - | — |
| Leads Totales | 7 | 7 | 4-5/día | 🟢 Igual que ayer, por encima de meta |
| CTR Promedio | 2.03% | 1.81% | 3-4% | 🟡 Mejora (+12.2%), sigue bajo meta |
| Impresiones (lead-gen) | 9,740 | 11,632 | - | — |
| Clicks (lead-gen) | 198 | 211 | - | — |
| Campañas activas sin ningún lead | 3 (PY Beco, SLV Beco, GT Beco — todas Beco) | 2 (COL Odoo, SLV Beco) | - | 🔴 Empeoró en cantidad, pero concentrado 100% en línea Beco |
| Mejor campaña del día | GT Odoo ($5.89 CPL, 4 leads) | PY Beco ($4.32 CPL, 2 leads) | - | — |
| Cambios de campaña ejecutados hoy | 0 | 0 | - | — |

---

## 📋 Proximas Acciones

- [x] Confirmar al cierre formal del 2026-11-19 si el CPL ($9.58) y el reparto de leads (3 campañas Beco en cero) se mantienen con los números finales — confirmado, variación menor (CPL final $9.76, CTR final 2.03%, leads sin cambio). Generado `Reports/2026-11-19 - Reporte Performance.md`.
- [ ] **Nuevo — prioridad alta:** investigar por qué las 3 campañas de la línea **Beco \| Conjuntos** (PY, SLV, GT) cayeron a cero leads el mismo día — revisar creativo/oferta compartida de esa línea de producto, ya que el patrón es por producto y no por geografía.
- [ ] Confirmar si la recuperación de **GT \| Odoo** (4 leads/$5.77 CPL) se sostiene mañana o fue un repunte puntual tras 3 días de deterioro.
- [ ] Monitorear **SLV \| Beco**, ya en cero leads por segundo día consecutivo.
- [ ] Verificar en Ads Manager por qué "Evento: gestión de nómina (Odoo)" sigue sin reportar gasto ni métricas (~7 días), aunque sin errores de entrega — confirmar `start_time`, presupuesto o calendario.
- [ ] Seguir trabajando el CTR blendeado (2.07% vs meta 3-4%) con pruebas A/B de creativo, priorizando evaluación por CTR antes de CPL.
- [ ] Pendiente heredado: decidir el futuro de las ~13 campañas históricas pausadas (Toma El control de tu pyme, Pyme Colombia, Pyme El Salvador, etc.) — reactivar, reemplazar formalmente o archivar.

---

## 🔗 Enlaces

- [[Daily notes/2026-11-19 - Resumen del Dia]] — nota del día anterior (documenta en realidad el 2026-11-18, por el mismo desajuste de zona horaria).
- [[Reports/2026-11-19 - Reporte Performance]] — reporte final y verificado de este mismo día (corrige las cifras provisionales de esta nota).
- [[Reports/2026-11-18 - Reporte Performance]] — reporte final y verificado del día anterior, usado como base de comparación en esta nota.
- Tags: #daily-note #summary #meta-ads #octopus
