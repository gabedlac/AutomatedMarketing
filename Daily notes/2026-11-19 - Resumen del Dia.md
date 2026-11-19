---
date: 2026-11-19
aliases: [resumen-2026-11-19]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-11-19

> [!warning] Nota sobre la fecha y los datos
> Esta rutina se ejecutó a las 05:50 UTC del 19-nov (≈ 23:50 del 2026-11-18 en `America/Guatemala`, zona horaria de la cuenta `act_2530001557366648`). A esa hora el día local de la cuenta **todavía no cambiaba a 2026-11-19** (faltaban ~10 minutos): `date_preset=today` resolvió a 2026-11-18, y `date_preset=yesterday` resolvió a 2026-11-17 (datos finales, consistentes con [[Reports/2026-11-17 - Reporte Performance]], con variaciones mínimas por ventana de atribución tardía). Por lo tanto, los datos de "hoy" en esta nota corresponden en realidad al día **2026-11-18** (prácticamente cerrado, faltaban ~10 minutos) y los de "ayer" a **2026-11-17** (cierre final). Se mantiene el nombre de archivo `2026-11-19` siguiendo el mismo patrón de rutinas anteriores (fecha del sistema al momento de ejecutarse) — mismo patrón de desajuste ya documentado en [[Daily notes/2026-11-18 - Resumen del Dia]].
>
> **Hallazgo de higiene de repo corregido en esta rutina:** al iniciar, `HEAD` estaba detached en el commit `e81fdda` ("Add Daily Performance Report - 2026-11-17"), 2 commits por delante de `main`/`origin/main` (que seguían en `23360d1`, el reporte del 16-nov). Esto significaba que las notas de `Daily notes/2026-11-18` y `Reports/2026-11-17` existían en el working tree pero **nunca se habían fusionado a `main` ni publicado a `origin`** por una rutina anterior. Se verificó que era un fast-forward limpio (`main` ancestro directo de `HEAD`) y se corrigió: `git checkout main && git merge --ff-only e81fdda && git push`. `main` y `origin/main` quedaron sincronizados en `e81fdda` antes de continuar con esta nota.

---

## 🎯 Campañas Revisadas

Se revisaron las 7 campañas activas de lead-gen + 1 de evento vía `ads_get_ad_entities` (nivel campaña, `date_preset=today`, equivalente a 2026-11-18 casi cerrado en zona horaria de la cuenta):

| Campaña | Status | Gasto | Impresiones | Clicks | CTR | Leads | CPL |
|---|---|---|---|---|---|---|---|
| 🟢 PY \| Beco \| CP \| Conjuntos | ACTIVE | $8.56 | 1,425 | 19 | 1.33% | 2 | **$4.28** |
| 🟢 PY \| Odoo \| CP \| Servicios | ACTIVE | $6.85 | 1,133 | 27 | 2.38% | 1 | $6.85 |
| 🟢 SLV \| Odoo \| CP \| Servicios | ACTIVE | $5.92 | 972 | 16 | 1.65% | 1 | $5.92 |
| 🟡 GT \| Odoo \| CP \| Servicios | ACTIVE | $24.52 | 3,702 | 78 | 2.11% | 2 | $12.26 |
| 🟡 GT \| Beco \| CP \| Conjuntos | ACTIVE | $15.33 | 2,213 | 29 | 1.31% | 1 | $15.33 |
| 🔴 COL \| Odoo \| CP \| Servicios | ACTIVE | $8.41 | 844 | 15 | 1.78% | 0 | — (sin leads) |
| 🔴 SLV \| Beco \| CP \| Conjuntos | ACTIVE | $8.19 | 1,234 | 25 | 2.03% | 0 | — (sin leads) |
| ⚪ Evento: gestión de nómina (Odoo) | ACTIVE (EVENT_RESPONSES, no lead-gen) | sin datos | sin datos | sin datos | — | n/a | n/a |

**Resto de la cuenta — todo PAUSED** (13 campañas, confirmado por `ads_get_ad_entities` con filtro `effective_status=PAUSED`): COL \| Beco \| CP \| Conjuntos, COL \| Odoo \| CP \| Servicios (versión de prueba anterior), 2x boosts de "Evento: Odoo en Acción", "[2026-08][Lead Generation][Odoo][COL] - Pyme Colombia", "...[USA] - Toma El control de tu pyme", "...[GT] - Toma El control de tu pyme", Accurate Partners - Loyalti, "...[GT] - Odoo Test", "...[GT] - Beco", Conversión Clientes Potenciales MX/PY, "...[SV] - Pyme El Salvador", 🟡 Conversión - Clientes Potenciales.

`ads_account_get_activity_logs` para el rango 2026-11-18 00:00–24:00 (America/Guatemala) **no devolvió ningún evento** (ni cambios manuales ni el cargo automático de facturación de Meta que suele registrarse alrededor de las 7:39am — todavía no ocurrió porque el día local no ha cerrado). No se ejecutó ningún cambio de presupuesto, targeting ni creativo hoy.

---

## 📊 Análisis e Insights

1. **El CPL blendeado empeora con fuerza y rompe la racha positiva de ayer:** las 7 campañas de lead-gen acumulan 7 leads con $77.78 de gasto (casi cerrado, faltan ~10 min) → CPL blendeado de **$11.11**, +93.6% frente a los $5.74 (final) del 2026-11-17, muy por encima del rango meta $6-7.
2. **Leads totales caen a la mitad (15 → 7):** por debajo de lo reportado en varios días recientes, aunque todavía dentro/por encima de la meta diaria de 4-5/día.
3. **Las campañas en cero suben de 1 a 2:** hoy son COL \| Odoo y SLV \| Beco; ninguna de las dos estaba en cero ayer (2 y 1 lead respectivamente). PY \| Beco, que llevaba 2+ días consecutivos sin leads, **rompe su racha** con 2 leads hoy a $4.28 CPL — la mejor campaña del día.
4. **GT \| Odoo (mayor volumen de la cuenta) se deteriora de nuevo:** leads caen de 4 a 2 y el CPL sube de $7.84 a $12.26 (+56%), encadenando un segundo día fuera de meta tras el retroceso ya reportado el 17-nov (9→4 leads).
5. **GT \| Beco retrocede con fuerza:** de 2 leads/$6.93 CPL (dentro de meta) a 1 lead/$15.33 CPL (+121%), la peor cifra de CPL de toda la cuenta hoy.
6. **SLV \| Odoo retrocede tras su mejor día registrado:** de 4 leads/$2.20 CPL ayer a 1 lead/$5.92 CPL hoy — sigue dentro de meta pero con una caída notable de volumen.
7. **CTR blendeado mejora levemente a 1.81%** (vs 1.66% ayer), pero sigue muy por debajo de la meta de 3-4%.
8. **`ads_insights_anomaly_signal` no detectó anomalías** (solapamiento de subasta, fatiga de creativo o audiencia estrecha) en los ad sets analizados — el deterioro de CPL/leads no tiene una causa técnica identificada por la herramienta.
9. **Campaña de evento sigue sin datos** ("Evento: gestión de nómina (Odoo)" ACTIVE, sin gasto/impresiones/clicks reportados). `ads_get_errors` no devolvió ningún error de entrega bloqueante. Problema persistente ya reportado en días anteriores, pendiente de verificación manual en Ads Manager.
10. **Importante — dato provisional:** como se explica en la nota de advertencia arriba, al día de hoy (2026-11-18 en la cuenta) le faltaban ~10 minutos para cerrar al momento de esta rutina; los números pueden variar mínimamente (atribución tardía) antes del cierre definitivo, aunque un cambio material en los próximos minutos es poco probable.
11. No hubo ninguna otra sesión de Claude Code activa en la cuenta hoy aparte de esta rutina, y no se realizó investigación externa de competencia o tendencias de mercado.

---

## ✏️ Cambios Realizados

Ninguno en Meta Ads. Solo se hizo lectura/análisis (`ads_get_ad_entities`, `ads_account_get_activity_logs`, `ads_insights_anomaly_signal`, `ads_get_errors`); no se modificó presupuesto, targeting, copy ni creativo de ninguna campaña desde esta rutina ni se detectaron cambios manuales en Ads Manager (sin eventos registrados en el log de actividad del día).

**Cambio técnico/de repositorio:** se corrigió el `HEAD` detached descrito en la nota de advertencia (fast-forward de `main` a `e81fdda` + push a `origin/main`), dejando el repositorio sincronizado antes de crear esta nota.

---

## 🔬 Investigación Realizada

- Se consultó `ads_get_ad_entities` (nivel campaña y cuenta, `act_2530001557366648`) con `date_preset=today` y `date_preset=yesterday`, y se verificó la zona horaria real de la cuenta (`timezone_name=America/Guatemala`) para confirmar a qué día calendario corresponde cada dato.
- Se consultó `ads_account_get_activity_logs` para 2026-11-18 00:00–24:00 (America/Guatemala): sin resultados (ni cambios manuales ni facturación automática, consistente con que el día aún no cerró).
- Se ejecutó `ads_insights_anomaly_signal` sobre la cuenta: sin anomalías de solapamiento de subasta, fatiga de creativo o audiencia estrecha.
- Se ejecutó `ads_get_errors` sobre la campaña de evento sin delivery: sin errores bloqueantes de publicación.
- Se listaron las 13 campañas PAUSED de la cuenta para confirmar que no hubo reactivaciones.
- Se auditó `git status`/`git log`/`git branch -a`: se detectó y corrigió un `HEAD` detached 2 commits por delante de `main`/`origin/main` (ver advertencia arriba); tras la corrección, repo limpio y sincronizado.
- Se revisó la carpeta `Reports/`: tras la corrección del repo, ya incluye hasta 2026-11-17; sigue faltando el Reporte Performance de 2026-11-18 (pendiente de que ese día cierre formalmente).
- No se realizó investigación externa de competencia ni tendencias de mercado.

---

## 📊 Datos Clave del Día

| Métrica (blendeada, 7 campañas lead-gen) | Hoy (2026-11-18, ~10 min de cerrar) | Ayer (2026-11-17, final) | Meta | Status |
|---|---|---|---|---|
| CPL Promedio | **$11.11** | $5.74 | $6-7 | 🔴 Empeora con fuerza, muy fuera de meta |
| Gasto Total (lead-gen) | $77.78 | $86.04 | - | — |
| Leads Totales | 7 | 15 | 4-5/día | 🟡 Cae a la mitad, aunque sigue ≥ meta |
| CTR Promedio | 1.81% | 1.66% | 3-4% | 🔴 Mejora leve, sigue bajo meta |
| Impresiones (lead-gen) | 11,523 | 11,918 | - | — |
| Clicks (lead-gen) | 209 | 198 | - | — |
| Campañas activas sin ningún lead | 2 (COL Odoo, SLV Beco) | 1 (PY Beco) | - | 🔴 Empeoró |
| Mejor campaña del día | PY Beco ($4.28 CPL, 2 leads) | SLV Odoo ($2.20 CPL, 4 leads) | - | — |
| Cambios de campaña ejecutados hoy | 0 | 0 | - | — |

---

## 📋 Proximas Acciones

- [ ] Confirmar al cierre formal del 2026-11-18 (vía rutina de Reporte Performance) si el salto de CPL ($5.74→$11.11) y la caída de leads (15→7) se mantienen con los números finales, y generar `Reports/2026-11-18 - Reporte Performance.md` (actualmente falta en la carpeta `Reports/`).
- [ ] Investigar el deterioro de **GT \| Odoo** (segundo día consecutivo fuera de meta: 9→4→2 leads, CPL $3.56→$7.84→$12.26) — mayor volumen de la cuenta, revisar fatiga de audiencia/creativo aunque `ads_insights_anomaly_signal` no detectó anomalías.
- [ ] Revisar **GT \| Beco** tras su peor CPL del día ($15.33, 1 lead) — confirmar si es ruido de un día o inicio de una racha negativa.
- [ ] Monitorear **COL \| Odoo** y **SLV \| Beco**, ambas en cero leads hoy tras tener leads ayer — evaluar creativo/audiencia si se repite mañana.
- [ ] Seguir vigilando si **PY \| Beco** sostiene la recuperación (2 leads/$4.28 CPL) tras 2+ días en cero.
- [ ] Verificar en Ads Manager por qué "Evento: gestión de nómina (Odoo)" sigue sin reportar gasto ni métricas, aunque sin errores de entrega — confirmar `start_time`, presupuesto o calendario.
- [ ] Investigar por qué el CTR blendeado sigue muy por debajo de meta (1.81% vs 3-4%) a pesar de la leve mejora — revisar creativo y frecuencia.
- [ ] Pendiente heredado: decidir el futuro de las ~13 campañas históricas pausadas (Toma El control de tu pyme, Pyme Colombia, Pyme El Salvador, etc.) — reactivar, reemplazar formalmente o archivar.

---

## 🔗 Enlaces

- [[Daily notes/2026-11-18 - Resumen del Dia]] — nota del día anterior (documenta en realidad el 2026-11-17, por el mismo desajuste de zona horaria).
- [[Reports/2026-11-17 - Reporte Performance]] — último Reporte Performance disponible en el vault (falta el de 2026-11-18, día que esta nota documenta de forma provisional).
- Tags: #daily-note #summary #meta-ads #octopus
