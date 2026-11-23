---
date: 2026-11-23
aliases: [resumen-2026-11-23]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-11-23

> [!warning] Nota sobre la fecha y los datos (mismo desajuste de zona horaria de rutinas anteriores)
> Esta rutina se ejecutó a las **~05:51 UTC del 23-nov** (≈ 23:51 del 2026-11-22 en `America/Guatemala`, zona horaria de la cuenta `act_2530001557366648`). A esa hora el día local de la cuenta **todavía no cambiaba a 2026-11-23**: `date_preset=today` resolvió a **2026-11-22** (provisional, faltan ~9 minutos de cierre) y `date_preset=yesterday` resolvió a **2026-11-21** (final, ya publicado en [[Reports/2026-11-21 - Reporte Performance]]). Por lo tanto, los datos de "hoy" en esta nota corresponden en realidad al día **2026-11-22** (provisional) y la comparación es contra **2026-11-21** (final). Se mantiene el nombre de archivo `2026-11-23` siguiendo el mismo patrón de rutinas anteriores (fecha del sistema al momento de ejecutarse) — mismo desajuste ya documentado en las notas del 18 al 22-nov.
>
> **Verificación de drift de atribución tardía contra el reporte final del 21-nov:** al re-consultar `date_preset=yesterday` (2026-11-21) hoy, el gasto total subió de $81.56 (final reportado) a **$81.61** (+$0.05) y las impresiones de 11,120 a **11,163** (+43); leads y CPL por campaña no cambiaron. Ajuste marginal (+0.4%), consistente con el mismo patrón ya documentado en notas anteriores (18→19, 19→20, 20→21-nov); no se corrige el reporte ya publicado del 21-nov.
>
> **Higiene de repo corregida en esta rutina:** al iniciar, `HEAD` estaba detached en el commit `d7a5922` ("Add Daily Performance Report - 2026-11-21"), con la rama local `main` 10 commits por detrás (todavía en `23360d1`, el reporte del 16-nov), aunque `origin/main` ya estaba sincronizado en `d7a5922` tras `git fetch`. Se verificó que era un fast-forward limpio (`origin/main` ancestro directo de `HEAD`) y se corrigió: `git checkout main && git merge --ff-only origin/main` (repo quedó "up to date with origin/main"). Este mismo problema se repite y se corrige rutina tras rutina desde el 20-nov; convendría investigar por qué la rama local `main` no avanza automáticamente tras cada push.

---

## 🎯 Campañas Revisadas

Se revisaron las 7 campañas activas de lead-gen + 1 de evento vía `ads_get_ad_entities` (nivel campaña, `date_preset=today` → día real 2026-11-22, provisional):

| Campaña | Status | Gasto | Impresiones | Clicks | CTR | Leads | CPL |
|---|---|---|---|---|---|---|---|
| 🟢 PY \| Odoo \| CP \| Servicios | ACTIVE | $10.36 | 1,528 | 42 | 2.75% | 5 | **$2.07** |
| 🟢 SLV \| Odoo \| CP \| Servicios | ACTIVE | $10.02 | 1,425 | 31 | 2.18% | 4 | $2.51 |
| 🟢 COL \| Odoo \| CP \| Servicios | ACTIVE | $10.37 | 776 | 15 | 1.93% | 2 | $5.19 |
| 🟡 GT \| Beco \| CP \| Conjuntos | ACTIVE | $18.73 | 2,166 | 53 | 2.45% | 3 | $6.24 |
| 🟡 GT \| Odoo \| CP \| Servicios | ACTIVE | $37.87 | 5,498 | 96 | 1.75% | 6 | $6.31 |
| 🟡 PY \| Beco \| CP \| Conjuntos | ACTIVE | $9.57 | 1,626 | 29 | 1.78% | 1 | $9.57 |
| 🔴 SLV \| Beco \| CP \| Conjuntos | ACTIVE | $8.93 | 1,474 | 27 | 1.83% | 0 | — (sin leads) |
| ⚪ Evento: El futuro de la gestión de nómina (Odoo) | ACTIVE (EVENT_RESPONSES, no lead-gen) | $0.00 | 0 | 0 | — | n/a | n/a |

**Resto de la cuenta — todo PAUSED** (14 campañas, sin cambios desde días anteriores): COL \| Beco \| CP \| Conjuntos, COL \| Odoo \| CP \| Servicios (versión de prueba anterior), 2x boosts de "Evento: Odoo en Acción", "[2026-08][Lead Generation][Odoo][COL] - Pyme Colombia", "...[USA] - Toma El control de tu pyme", "...[GT] - Toma El control de tu pyme", Accurate Partners - Loyalti, "...[GT] - Odoo Test", "...[GT] - Beco", Conversión Clientes Potenciales MX/PY, "...[SV] - Pyme El Salvador", 🟡 Conversión - Clientes Potenciales.

`ads_account_get_activity_logs` para el rango 2026-11-22 06:00 – 2026-11-23 06:00 UTC **no devolvió ningún evento** (ni cambios manuales ni el cargo automático de facturación de Meta, que todavía no ocurre porque el día local no ha cerrado). No se ejecutó ningún cambio de presupuesto, targeting ni creativo hoy.

---

## 📊 Análisis e Insights

1. **Mejor día del período registrado tanto en CPL como en leads:** 21 leads con $105.85 de gasto (provisional) → CPL blendeado **$5.04**, -19.6% vs. los $6.27 (final) del 21-nov, y el primer día claramente por debajo de toda la banda meta $6-7 (no solo tocándola). Leads totales suben a **21** (+61.5% vs. 13), nuevo máximo del período.
2. **PY \| Odoo rompe su racha de 3 días consecutivos en cero de la forma más fuerte vista hasta ahora:** pasa de 0 a **5 leads a $2.07 CPL**, el mayor número de leads de una sola campaña en un día del período y uno de los CPL más bajos registrados — contradice la hipótesis de un problema estructural en esta campaña.
3. **PY \| Beco también sale de su racha de 3 días en cero, pero a un costo alto:** 1 lead a **$9.57 CPL**, bien por encima de la meta $6-7 — la recuperación es parcial y cara comparada con la de PY \| Odoo.
4. **SLV \| Beco es ahora la única campaña en cero leads**, por 4º-5º día consecutivo (viene de la racha de 3 días reportada el 21-nov) — el grupo "en cero" se reduce de 3 campañas a 1, pero se concentra justo en esta campaña, que merece revisión prioritaria de audiencia/creativo/puja.
5. **GT \| Odoo rompe su racha de 3 días consecutivos de CPL en aumento:** $5.89 (19-nov) → $7.15 (20-nov) → $7.99 (21-nov) → **$6.31 hoy**, con su mejor número de leads del período (**6**, vs. 4 los tres días previos) pese a seguir siendo la campaña de mayor gasto absoluto ($37.87). Señal positiva que contradice la preocupación de eficiencia decreciente marcada como prioridad el 21-nov.
6. **GT \| Beco continúa su recuperación parcial:** 2 leads/$7.31 (21-nov) → 3 leads/**$6.24** hoy, ya dentro de la meta $6-7, aunque todavía lejos de su mejor histórico (3 leads/$4.85 del 20-nov).
7. **COL \| Odoo y SLV \| Odoo retroceden en CPL pero mantienen leads:** COL \| Odoo sube de $2.02 (21-nov) a **$5.19** (2 leads, -1 vs. ayer) y SLV \| Odoo sube de $1.86 a **$2.51** (4 leads, igual que ayer) — ambas siguen por debajo de la meta, pero ya no son las de mejor CPL del día (ese lugar lo toman PY \| Odoo y SLV \| Odoo).
8. **Gasto total sube a $105.85** (provisional), +29.8% vs. los $81.56 finales de ayer — el mayor gasto absoluto del período, pero acompañado de un salto aún mayor en leads (+61.5%), lo que explica la mejora de CPL pese a gastar más.
9. **CTR blendeado mejora a 2.02%** (provisional; vs. 1.75% final de ayer, +15.4%), el mejor del período registrado, aunque sigue por debajo de la meta 3-4%. A nivel individual, **PY \| Odoo tuvo el mejor CTR del día (2.75%)** y también uno de los mejores CPL.
10. **`ads_insights_anomaly_signal` no detectó anomalías** (solapamiento de subasta, fatiga de creativo o audiencia estrecha) en los ad sets analizados.
11. **Campaña de evento sigue sin datos** ("Evento: El futuro de la gestión de nómina (Odoo)" ACTIVE, sin gasto/impresiones/clicks por ~13º día consecutivo). `ads_get_errors` no devolvió ningún error de entrega bloqueante.
12. No hubo ninguna otra sesión de Claude Code activa en la cuenta hoy aparte de esta rutina, y no se realizó investigación externa de competencia o tendencias de mercado.
13. **Dato pendiente de cierre:** como se explica en la nota de advertencia arriba, los números de esta nota son provisionales (faltan ~9 minutos de cierre del día de la cuenta); se espera que una rutina posterior confirme o ajuste estas cifras con los datos finales, como ha ocurrido en días anteriores.

---

## ✏️ Cambios Realizados

Ninguno en Meta Ads. Solo se hizo lectura/análisis (`ads_get_ad_accounts`, `ads_get_ad_entities` con `date_preset=today` y `date_preset=yesterday`, `ads_account_get_activity_logs`, `ads_insights_anomaly_signal`, `ads_get_errors`); no se modificó presupuesto, targeting, copy ni creativo de ninguna campaña desde esta rutina ni se detectaron cambios manuales en Ads Manager (sin eventos registrados en el log de actividad del día).

**Cambio técnico/de repositorio:** se corrigió el `HEAD` detached descrito en la nota de advertencia (fast-forward de `main` local a `origin/main`, ya en `d7a5922`), dejando el repositorio alineado antes de crear esta nota.

---

## 🔬 Investigación Realizada

- Se consultó `ads_get_ad_accounts` para confirmar la cuenta activa de la plantilla (`act_2530001557366648`, "GT | Octopus Innovations") entre las 10 cuentas visibles para este usuario (el resto están CLOSED, DISABLED o no son la cuenta configurada).
- Se consultó `ads_get_ad_entities` (nivel cuenta) y se verificó la zona horaria real de la cuenta (`timezone_name=America/Guatemala`) junto con `date -u` / `TZ='America/Guatemala' date` del sistema para confirmar a qué día calendario corresponde el dato ("hoy" de la cuenta = 2026-11-22, provisional, ~9 min de cierre).
- Se consultó `ads_get_ad_entities` (nivel campaña) con `date_preset=today` (→ 22-nov, provisional) y `date_preset=yesterday` (→ 21-nov) para las 7 campañas lead-gen activas más la de evento.
- Se comparó `date_preset=yesterday` (21-nov) contra las cifras finales ya publicadas en [[Reports/2026-11-21 - Reporte Performance]] para detectar drift de atribución tardía (ver nota de advertencia arriba: +$0.05 gasto, +43 impresiones, sin cambio en leads/clicks/CPL por campaña).
- Se consultó `ads_account_get_activity_logs` para el rango 2026-11-22 06:00 – 2026-11-23 06:00 UTC: sin resultados (ni cambios manuales ni facturación automática, consistente con que el día local aún no cerró).
- Se ejecutó `ads_insights_anomaly_signal` sobre la cuenta: sin anomalías de solapamiento de subasta, fatiga de creativo o audiencia estrecha.
- Se ejecutó `ads_get_errors` sobre la cuenta: sin errores bloqueantes de publicación o entrega.
- Se auditó `git status`/`git branch -a`/`git fetch`/`git merge-base --is-ancestor`: se detectó y corrigió un `HEAD` detached 10 commits por detrás de `main` local (ya sincronizado con `origin/main` tras el fetch); tras la corrección, repo limpio y alineado.
- No se realizó investigación externa de competencia ni tendencias de mercado.

---

## 📊 Datos Clave del Día

| Métrica (blendeada, 7 campañas lead-gen) | 2026-11-22 (provisional, ~9 min de cierre) | 2026-11-21 (final, verificado) | Meta | Status |
|---|---|---|---|---|
| CPL Promedio | **$5.04** | $6.27 | $6-7 | 🟢 Mejora fuerte (-19.6%), primer día claramente bajo meta del período registrado |
| Gasto Total (lead-gen) | $105.85 | $81.56 | - | 🟡 +29.8%, mayor gasto absoluto del período |
| Leads Totales | **21** | 13 | 4-5/día | 🟢 +61.5%, muy por encima de meta, máximo del período registrado |
| CTR Promedio | 2.02% | 1.75% | 3-4% | 🟡 Mejora (+15.4%), mejor del período, pero sigue bajo meta |
| Impresiones (lead-gen) | 14,493 | 11,163 | - | — |
| Clicks (lead-gen) | 293 | 195 | - | — |
| Campañas activas sin ningún lead | 1 (SLV Beco) | 3 (PY Beco, PY Odoo, SLV Beco) | - | 🟢 Mejora (de 3 a 1) |
| Mejor campaña del día | PY Odoo ($2.07 CPL, 5 leads — máximo de leads de una campaña en el período) | SLV Odoo ($1.86 CPL, 4 leads) | - | — |
| Cambios de campaña ejecutados hoy | 0 | 0 | - | — |

---

## 📋 Proximas Acciones

- [ ] Confirmar al cierre formal del 2026-11-22 si el CPL ($5.04), el CTR (2.02%) y la recuperación de PY Odoo/PY Beco se mantienen con los números finales — generar `Reports/2026-11-22 - Reporte Performance.md` una vez cierre el día.
- [ ] **Prioridad alta:** revisar por qué **SLV \| Beco** sigue en cero leads por 4º-5º día consecutivo (único grupo en cero hoy) — evaluar audiencia, puja, horario de entrega u oferta frente a SLV \| Odoo (mismo país, sí convierte).
- [ ] Confirmar si la recuperación de **PY \| Odoo** (0 → 5 leads, $2.07 CPL) es sostenible o puntual, y si **PY \| Beco** (1 lead a $9.57, sobre meta) puede bajar de CPL sin perder el lead recién obtenido.
- [ ] Verificar si la mejora de **GT \| Odoo** (CPL $7.99 → $6.31, 6 leads nuevo máximo) marca un cambio de tendencia o es ruido, antes de decidir sobre el escalado de presupuesto que se señaló pausar el 21-nov.
- [ ] Verificar en Ads Manager por qué "Evento: El futuro de la gestión de nómina (Odoo)" sigue sin reportar gasto ni métricas (~13 días), aunque sin errores de entrega — confirmar `start_time`, presupuesto o calendario; el tiempo acumulado ya justifica revisión manual directa.
- [ ] Seguir trabajando el CTR blendeado (2.02% vs meta 3-4%) con pruebas A/B de creativo, priorizando evaluación por CTR antes de CPL.
- [ ] Investigar por qué la rama local `main` queda detached/desactualizada rutina tras rutina (recurrente desde el 20-nov) para evitar depender de la corrección manual en cada ejecución.
- [ ] Pendiente heredado: decidir el futuro de las ~14 campañas históricas pausadas (Toma El control de tu pyme, Pyme Colombia, Pyme El Salvador, etc.) — reactivar, reemplazar formalmente o archivar.

---

## 🔗 Enlaces

- [[Reports/2026-11-21 - Reporte Performance]] — reporte final y verificado del día usado como base de comparación en esta nota.
- [[Daily notes/2026-11-22 - Resumen del Dia]] — nota del día anterior (documenta en realidad el 2026-11-21, final, por el mismo desajuste de zona horaria).
- [[Reports/2026-11-20 - Reporte Performance]] — reporte final de dos días atrás, para contexto adicional de tendencia.
- Tags: #daily-note #summary #meta-ads #octopus
