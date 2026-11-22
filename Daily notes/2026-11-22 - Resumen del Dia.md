---
date: 2026-11-22
aliases: [resumen-2026-11-22]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-11-22

> [!warning] Nota sobre la fecha y los datos (mismo desajuste de zona horaria de rutinas anteriores)
> Esta rutina se ejecutó a las **~05:52 UTC del 22-nov** (≈ 23:52 del 2026-11-21 en `America/Guatemala`, zona horaria de la cuenta `act_2530001557366648`). A esa hora el día local de la cuenta **todavía no cambiaba a 2026-11-22**: `date_preset=today` resolvió a **2026-11-21** (provisional, faltan ~8 minutos de cierre) y `date_preset=yesterday` resolvió a **2026-11-20**. Por lo tanto, los datos de "hoy" en esta nota corresponden en realidad al día **2026-11-21** (provisional) y la comparación es contra **2026-11-20** (final, verificado en [[Reports/2026-11-20 - Reporte Performance]]). Se mantiene el nombre de archivo `2026-11-22` siguiendo el mismo patrón de rutinas anteriores (fecha del sistema al momento de ejecutarse) — mismo desajuste ya documentado en las notas del 18 al 21-nov.
>
> **Drift de atribución tardía detectado al validar contra el reporte final del 20-nov:** al re-consultar `date_preset=yesterday` (2026-11-20) hoy, el gasto total subió de $84.68 (final reportado) a **$84.98** (+$0.30) y las impresiones de 10,976 a **11,039** (+63); leads, clicks y CPL por campaña no cambiaron. Es un ajuste menor, consistente con el mismo patrón de atribución tardía ya documentado en notas anteriores (18→19, 19→20-nov); no se corrige el reporte ya publicado del 20-nov por ser una diferencia marginal (+0.35%).
>
> **Hallazgo de higiene de repo corregido en esta rutina:** al iniciar, `HEAD` estaba detached en el commit `8b20c6d` ("Add Daily Performance Report - 2026-11-20"), con la rama local `main` 8 commits por detrás (todavía en `23360d1`, el reporte del 16-nov), aunque `origin/main` ya estaba sincronizado en `8b20c6d` tras `git fetch`. Se verificó que era un fast-forward limpio (`origin/main` ancestro directo de `HEAD`) y se corrigió: `git checkout main && git merge --ff-only 8b20c6d` (repo quedó "up to date with origin/main", confirmando que solo era un desajuste de la copia local, no una falta de push).

---

## 🎯 Campañas Revisadas

Se revisaron las 7 campañas activas de lead-gen + 1 de evento vía `ads_get_ad_entities` (nivel campaña, `date_preset=today` → día real 2026-11-21, provisional):

| Campaña | Status | Gasto | Impresiones | Clicks | CTR | Leads | CPL |
|---|---|---|---|---|---|---|---|
| 🟢 COL \| Odoo \| CP \| Servicios | ACTIVE | $5.92 | 451 | 14 | 3.10% | 3 | **$1.97** |
| 🟢 SLV \| Odoo \| CP \| Servicios | ACTIVE | $7.37 | 1,163 | 29 | 2.49% | 4 | **$1.84** |
| 🟡 GT \| Beco \| CP \| Conjuntos | ACTIVE | $14.53 | 1,730 | 34 | 1.97% | 2 | $7.27 |
| 🟡 GT \| Odoo \| CP \| Servicios | ACTIVE | $31.82 | 4,855 | 76 | 1.57% | 4 | $7.96 |
| 🔴 PY \| Beco \| CP \| Conjuntos | ACTIVE | $6.35 | 829 | 17 | 2.05% | 0 | — (sin leads, 3er día) |
| 🔴 PY \| Odoo \| CP \| Servicios | ACTIVE | $8.03 | 1,056 | 11 | 1.04% | 0 | — (sin leads, 3er día) |
| 🔴 SLV \| Beco \| CP \| Conjuntos | ACTIVE | $7.04 | 934 | 14 | 1.50% | 0 | — (sin leads, 3er día) |
| ⚪ Evento: El futuro de la gestión de nómina (Odoo) | ACTIVE (EVENT_RESPONSES, no lead-gen) | $0.00 | 0 | 0 | — | n/a | n/a |

**Resto de la cuenta — todo PAUSED** (14 campañas, sin cambios desde días anteriores): COL \| Beco \| CP \| Conjuntos, COL \| Odoo \| CP \| Servicios (versión de prueba anterior), 2x boosts de "Evento: Odoo en Acción", "[2026-08][Lead Generation][Odoo][COL] - Pyme Colombia", "...[USA] - Toma El control de tu pyme", "...[GT] - Toma El control de tu pyme", Accurate Partners - Loyalti, "...[GT] - Odoo Test", "...[GT] - Beco", Conversión Clientes Potenciales MX/PY, "...[SV] - Pyme El Salvador", 🟡 Conversión - Clientes Potenciales.

`ads_account_get_activity_logs` para el rango 2026-11-21 06:00 – 2026-11-22 06:00 UTC **no devolvió ningún evento** (ni cambios manuales ni el cargo automático de facturación de Meta, que todavía no ocurre porque el día local no ha cerrado). No se ejecutó ningún cambio de presupuesto, targeting ni creativo hoy.

---

## 📊 Análisis e Insights

1. **Fuerte mejora del CPL blendeado, rompiendo tres días consecutivos de deterioro:** 13 leads con $81.06 de gasto (provisional) → CPL blendeado **$6.24**, -48.4% vs. los $12.10 (final) del 20-nov, y el primer día dentro de la meta de $6-7 desde que se documenta esta cuenta.
2. **COL \| Odoo y SLV \| Odoo rompen su racha de dos días en cero** con los mejores CPL individuales registrados hasta ahora en esta cuenta: **SLV \| Odoo $1.84 (4 leads)** y **COL \| Odoo $1.97 (3 leads)** — muy por debajo de la meta $6-7, y revierten la teoría "geográfica" del 20-nov (PY/SLV/COL en cero) planteada como hipótesis.
3. **El grupo en cero ya no es geográfico sino más acotado:** hoy solo **PY (Beco y Odoo) y SLV \| Beco** están en cero leads — 3er día consecutivo en cero para estas 3 campañas específicas — mientras que SLV \| Odoo y COL \| Odoo sí convierten. El patrón parece ser por campaña individual más que por país completo.
4. **Leads totales casi se duplican: 13 hoy vs. 7 el 20-nov** (+85.7%), el mayor número de leads en un día del período registrado, repartidos en **4 campañas distintas** (vs. solo 2, ambas GT, el día anterior) — mejora notable en diversificación de fuentes de leads.
5. **GT \| Odoo sigue subiendo de CPL por tercer día consecutivo:** $5.89 (19-nov) → $7.15 (20-nov) → **$7.96 hoy**, pese a mantener 4 leads los tres días; el gasto también sigue subiendo ($23.55 → $28.61 → $31.82). El mayor gasto no se traduce en más conversiones — señal de eficiencia decreciente que merece revisión prioritaria antes de seguir escalando presupuesto.
6. **GT \| Beco no sostiene su mejor-CPL-histórico de ayer:** cae de 3 leads/$4.85 CPL (20-nov, su mejor resultado histórico) a 2 leads/$7.27 CPL hoy — confirma que el repunte del 20-nov fue puntual, tal como se anticipaba como pendiente de verificación en la nota anterior.
7. **Gasto total baja a $81.06** (provisional), -4.3% vs. los $84.68 finales de ayer, con casi todas las campañas reduciendo gasto salvo GT \| Odoo (+$3.21).
8. **CTR blendeado retrocede levemente a 1.77%** (provisional; vs. 1.90% final de ayer, -6.8%), sigue por debajo de la meta 3-4%. A nivel individual, COL \| Odoo tuvo el mejor CTR del día (3.10%) y también el mejor CPL — primera vez en el período que la campaña con mejor CTR también lidera en CPL.
9. **`ads_insights_anomaly_signal` no detectó anomalías** (solapamiento de subasta, fatiga de creativo o audiencia estrecha) en los ad sets analizados.
10. **Campaña de evento sigue sin datos** ("Evento: El futuro de la gestión de nómina (Odoo)" ACTIVE, sin gasto/impresiones/clicks por ~11º día consecutivo). `ads_get_errors` no devolvió ningún error de entrega bloqueante.
11. No hubo ninguna otra sesión de Claude Code activa en la cuenta hoy aparte de esta rutina, y no se realizó investigación externa de competencia o tendencias de mercado.
12. **Dato pendiente de cierre:** como se explica en la nota de advertencia arriba, los números de esta nota son provisionales (faltan ~8 minutos de cierre del día de la cuenta); se espera que una rutina posterior confirme o ajuste estas cifras con los datos finales, como ha ocurrido en días anteriores.

---

## ✏️ Cambios Realizados

Ninguno en Meta Ads. Solo se hizo lectura/análisis (`ads_get_ad_accounts`, `ads_get_ad_entities`, `ads_account_get_activity_logs`, `ads_insights_anomaly_signal`, `ads_get_errors`); no se modificó presupuesto, targeting, copy ni creativo de ninguna campaña desde esta rutina ni se detectaron cambios manuales en Ads Manager (sin eventos registrados en el log de actividad del día).

**Cambio técnico/de repositorio:** se corrigió el `HEAD` detached descrito en la nota de advertencia (fast-forward de `main` local a `8b20c6d`, ya sincronizado con `origin/main` tras `git fetch`), dejando el repositorio alineado antes de crear esta nota.

---

## 🔬 Investigación Realizada

- Se consultó `ads_get_ad_accounts` para confirmar la cuenta activa de la plantilla (`act_2530001557366648`, "GT | Octopus Innovations") entre las 10 cuentas visibles para este usuario (el resto están CLOSED, DISABLED o no son la cuenta configurada).
- Se consultó `ads_get_ad_entities` (nivel cuenta y campaña) con `date_preset=today` y se verificó la zona horaria real de la cuenta (`timezone_name=America/Guatemala`) para confirmar a qué día calendario corresponde el dato.
- Se consultó `date_preset=yesterday` (2026-11-20) y se comparó contra las cifras finales ya publicadas en [[Reports/2026-11-20 - Reporte Performance]] para detectar drift de atribución tardía (ver nota de advertencia arriba: +$0.30 gasto, +63 impresiones, sin cambio en leads/clicks/CPL).
- Se consultó el campo `lead` por campaña para confirmar que las 3 campañas sin leads (PY Beco, PY Odoo, SLV Beco) reportan **cero leads reales** (campo ausente = 0), no un error o dato faltante de la API.
- Se consultó `ads_account_get_activity_logs` para el rango 2026-11-21 06:00 – 2026-11-22 06:00 UTC: sin resultados (ni cambios manuales ni facturación automática, consistente con que el día local aún no cerró).
- Se ejecutó `ads_insights_anomaly_signal` sobre la cuenta: sin anomalías de solapamiento de subasta, fatiga de creativo o audiencia estrecha.
- Se ejecutó `ads_get_errors` sobre la cuenta: sin errores bloqueantes de publicación o entrega.
- Se comparó campaña por campaña contra los datos finales verificados de [[Reports/2026-11-20 - Reporte Performance]] para identificar el cambio de patrón (geográfico → por campaña individual) descrito en Insights.
- Se auditó `git status`/`git branch -a`/`git fetch`/`git merge-base --is-ancestor`: se detectó y corrigió un `HEAD` detached 8 commits por detrás de `main` local (ya sincronizado con `origin/main` tras el fetch); tras la corrección, repo limpio y alineado.
- No se realizó investigación externa de competencia ni tendencias de mercado.

---

## 📊 Datos Clave del Día

| Métrica (blendeada, 7 campañas lead-gen) | 2026-11-21 (provisional, ~8 min de cierre) | 2026-11-20 (final, verificado) | Meta | Status |
|---|---|---|---|---|
| CPL Promedio | **$6.24** | $12.10 | $6-7 | 🟢 Mejora fuerte (-48.4%), primer día dentro de meta del período registrado |
| Gasto Total (lead-gen) | $81.06 | $84.68 | - | 🟢 -4.3% |
| Leads Totales | **13** | 7 | 4-5/día | 🟢 Casi duplica, muy por encima de meta, máximo del período registrado |
| CTR Promedio | 1.77% | 1.90% | 3-4% | 🔴 Retrocede levemente (-6.8%), sigue bajo meta |
| Impresiones (lead-gen) | 11,018 | 10,976 | - | — |
| Clicks (lead-gen) | 195 | 208 | - | — |
| Campañas activas sin ningún lead | 3 (PY Beco, PY Odoo, SLV Beco) | 5 (SLV Beco, COL Odoo, PY Odoo, SLV Odoo, PY Beco) | - | 🟢 Mejora (de 5 a 3), dos campañas recuperan leads |
| Mejor campaña del día | SLV Odoo ($1.84 CPL, 4 leads — mejor CPL histórico de la cuenta) | GT Beco ($4.85 CPL, 3 leads) | - | — |
| Cambios de campaña ejecutados hoy | 0 | 0 | - | — |

---

## 📋 Proximas Acciones

- [ ] Confirmar al cierre formal del 2026-11-21 si el CPL ($6.24), el CTR (1.77%) y la recuperación de SLV Odoo/COL Odoo se mantienen con los números finales — generar `Reports/2026-11-21 - Reporte Performance.md` una vez cierre el día.
- [ ] **Prioridad alta:** revisar por qué el CPL de **GT \| Odoo** sube por tercer día consecutivo ($5.89 → $7.15 → $7.96) pese a mantener siempre 4 leads — evaluar si conviene pausar el escalado de presupuesto en esta campaña hasta estabilizar el CPL.
- [ ] Confirmar si **PY \| Beco, PY \| Odoo y SLV \| Beco** (3er día consecutivo en cero leads) comparten un factor común (audiencia, puja, horario de entrega, oferta) distinto al de SLV \| Odoo y COL \| Odoo, que sí recuperaron leads hoy.
- [ ] Verificar si la caída de **GT \| Beco** (3 leads/$4.85 → 2 leads/$7.27) es ruido normal o el inicio de una tendencia, dado que ayer se señaló como posible repunte puntual.
- [ ] Verificar en Ads Manager por qué "Evento: El futuro de la gestión de nómina (Odoo)" sigue sin reportar gasto ni métricas (~11 días), aunque sin errores de entrega — confirmar `start_time`, presupuesto o calendario.
- [ ] Seguir trabajando el CTR blendeado (1.77% vs meta 3-4%) con pruebas A/B de creativo, priorizando evaluación por CTR antes de CPL.
- [ ] Pendiente heredado: decidir el futuro de las ~14 campañas históricas pausadas (Toma El control de tu pyme, Pyme Colombia, Pyme El Salvador, etc.) — reactivar, reemplazar formalmente o archivar.

---

## 🔗 Enlaces

- [[Reports/2026-11-20 - Reporte Performance]] — reporte final y verificado del día usado como base de comparación en esta nota.
- [[Daily notes/2026-11-21 - Resumen del Dia]] — nota del día anterior (documenta en realidad el 2026-11-20, final, por el mismo desajuste de zona horaria).
- [[Reports/2026-11-19 - Reporte Performance]] — reporte final y verificado de dos días atrás, para contexto adicional de tendencia.
- Tags: #daily-note #summary #meta-ads #octopus
