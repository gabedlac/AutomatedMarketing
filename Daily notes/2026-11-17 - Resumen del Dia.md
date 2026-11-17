---
date: 2026-11-17
aliases: [resumen-2026-11-17]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-11-17

> [!info] Nota sobre los datos
> Datos obtenidos vía `ads_get_ad_entities` (`date_preset=today` / `date_preset=yesterday`) para `act_2530001557366648` (GT | Octopus Innovations) al momento de ejecutar esta rutina. Estas cifras son provisionales (lag normal de atribución de Meta) y pueden variar levemente frente al cierre que se publique en el próximo Reporte Performance. Los valores de "ayer" (2026-11-16) aquí mostrados ya son el cierre final y difieren levemente de los provisionales documentados en el resumen de ese día ($101.11 gasto / $7.22 CPL provisional vs. $102.28 / $7.31 final). `ads_account_get_activity_logs` no registró ningún cambio manual en la cuenta hoy (array vacío). Se encontró de nuevo un `HEAD` desprendido al iniciar la rutina; se corrigió con un fast-forward limpio de `main` a `origin/main` (84 commits), sin conflictos ni pérdida de historial.

---

## 🎯 Campañas Revisadas

Se revisaron las 7 campañas activas de lead-gen + 1 de evento vía `ads_get_ad_entities` (nivel campaña, `date_preset=today`):

| Campaña | Status | Gasto | Impresiones | Clicks | CTR | Leads | CPL |
|---|---|---|---|---|---|---|---|
| 🟢 GT \| Odoo \| CP \| Servicios | ACTIVE | $31.55 | 4,072 | 93 | 2.28% | 9 | **$3.51** |
| 🟡 PY \| Odoo \| CP \| Servicios | ACTIVE | $8.18 | 1,243 | 23 | 1.85% | 1 | $8.18 |
| 🟡 SLV \| Odoo \| CP \| Servicios | ACTIVE | $8.35 | 1,101 | 31 | 2.82% | 1 | $8.35 |
| 🔴 GT \| Beco \| CP \| Conjuntos | ACTIVE | $16.70 | 2,127 | 46 | 2.16% | 1 | $16.70 |
| 🔴 COL \| Odoo \| CP \| Servicios | ACTIVE | $8.24 | 577 | 9 | 1.56% | 0 | — (sin leads) |
| 🔴 PY \| Beco \| CP \| Conjuntos | ACTIVE | $8.79 | 1,384 | 29 | 2.10% | 0 | — (sin leads) |
| 🔴 SLV \| Beco \| CP \| Conjuntos | ACTIVE | $8.40 | 1,262 | 23 | 1.82% | 0 | — (sin leads, 3er día consecutivo) |
| ⚪ Evento: gestión de nómina (Odoo) | ACTIVE (EVENT_RESPONSES, no lead-gen) | $0.00 | 0 | 0 | — | n/a | n/a |

**Resto de la cuenta — todo PAUSED, sin cambios** (confirmado por `ads_account_get_activity_logs` vacío): "COL \| Beco \| CP \| Conjuntos" y "COL \| Odoo \| CP \| Servicios" (versiones de prueba anteriores), ambos boosts de "Evento: Odoo en Acción", "[2026-08][Lead Generation][Odoo][COL] - Pyme Colombia", "...[USA] - Toma El control de tu pyme", "...[GT] - Toma El control de tu pyme", "...[GT] - Beco", "...[GT] - Odoo Test", "...[SV] - Pyme El Salvador", Accurate Partners - Loyalti, Conversión Clientes Potenciales MX/PY, 🟡 Conversión - Clientes Potenciales.

No se ejecutó ningún cambio de presupuesto, targeting ni creativo hoy — ni desde esta rutina ni manualmente en Ads Manager.

---

## 📊 Análisis e Insights

1. **El CPL blendeado sube levemente y vuelve a quedar fuera de meta:** las 7 campañas de lead-gen generaron 12 leads hoy con $90.21 de gasto → CPL blendeado de **$7.52**, +2.9% frente a los $7.31 (cierre final) de ayer, por encima de la meta $6-7.
2. **Leads totales caen -14.3% (14 → 12):** sigue por encima de la meta diaria de 4-5/día, pero es el nivel más bajo desde la mejora reportada ayer.
3. **Las campañas en cero suben de 1 a 3:** hoy cerraron sin leads COL \| Odoo, PY \| Beco y SLV \| Beco, revirtiendo la mejora de ayer (solo SLV Beco en cero).
4. **SLV \| Beco llega a su 3er día consecutivo en cero leads**, con gasto estable (~$8.40) y sin ninguna conversión — la acción prioritaria heredada de ayer sigue sin resolverse y se mantiene como la mancha más persistente de la cuenta.
5. **SLV \| Odoo rompe su racha de 3 días como mejor campaña:** venía con $2.31 → $2.77 → $2.78 de CPL y 3-4 leads/día; hoy cae a solo 1 lead con CPL $8.35 (+200% aprox.), la caída más marcada del día.
6. **GT \| Odoo (mayor volumen de la cuenta) da un salto fuerte y es la mejor campaña del día:** leads suben de 4 a 9 y el CPL baja de $9.22 a **$3.51** (-62%), incluso con menor gasto ($36.87 → $31.55). Compensa gran parte de la caída del resto de la cuenta.
7. **GT \| Beco revierte la recuperación de ayer:** pasó de 3 leads/$5.80 CPL ayer a solo 1 lead/$16.70 CPL hoy — tercera oscilación fuerte en tres días (0 → 3 → 1 leads), patrón de alta volatilidad que amerita seguimiento.
8. **COL \| Odoo y PY \| Beco** generaron 1 lead cada una ayer y hoy caen a cero, sin cambio de presupuesto ni targeting que lo explique.
9. **CTR blendeado mejora a 2.16% hoy** (vs 2.01% ayer), aunque sigue por debajo de la meta 3-4%.
10. **`ads_insights_anomaly_signal` no detectó anomalías** (solapamiento de subasta, fatiga de creativo o audiencia estrecha) en los ad sets analizados.
11. **Campaña de evento sigue sin datos, ya serían 4 días consecutivos** (continuidad desde "tercer día consecutivo" reportado ayer): "Evento: gestión de nómina (Odoo)" sigue ACTIVE pero sin gasto, impresiones ni clicks. `ads_get_errors` no devolvió ningún error de entrega bloqueante; sigue pendiente de verificación directa en Ads Manager.
12. No hubo ninguna otra sesión de Claude Code activa en la cuenta hoy aparte de esta rutina, y no se realizó investigación externa de competencia o tendencias de mercado.

---

## ✏️ Cambios Realizados

Ninguno en Meta Ads. Solo se hizo lectura/análisis (`ads_get_ad_entities`, `ads_account_get_activity_logs`, `ads_insights_anomaly_signal`, `ads_get_errors`); no se modificó presupuesto, targeting, copy ni creativo de ninguna campaña desde esta rutina ni se detectaron cambios manuales en Ads Manager.

Único cambio técnico del día: se corrigió el `HEAD` desprendido del repositorio (`git checkout main` + fast-forward a `origin/main`, 84 commits, sin pérdida de historial) para poder commitear esta nota.

---

## 🔬 Investigación Realizada

- Se consultó `ads_get_ad_entities` (nivel campaña, cuenta `act_2530001557366648`) con `date_preset=today` y `date_preset=yesterday` para comparar día a día.
- Se consultó `ads_account_get_activity_logs` para 2026-11-17 (00:00–24:00 UTC): sin entradas, ningún cambio manual registrado en la cuenta hoy.
- Se ejecutó `ads_insights_anomaly_signal` sobre la cuenta: sin anomalías de solapamiento de subasta, fatiga de creativo o audiencia estrecha.
- Se ejecutó `ads_get_errors` sobre la campaña de evento sin delivery ("Evento: gestión de nómina (Odoo)"): sin errores bloqueantes de publicación.
- Se auditó `git status`/`git log`/`git branch`/`git fetch`: `HEAD` desprendido y rama local `main` desactualizada 84 commits frente a `origin/main`. Se corrigió con un fast-forward limpio (`main` era ancestro directo de `origin/main`, sin conflictos).
- Se revisó la carpeta `Reports/`: solo existe el Reporte Performance de 2026-11-15; falta el de 2026-11-16.
- No se realizó investigación externa de competencia ni tendencias de mercado.

---

## 📊 Datos Clave del Día

| Métrica (blendeada, 7 campañas lead-gen) | 2026-11-17 | 2026-11-16 (cierre final) | Meta | Status |
|---|---|---|---|---|
| CPL Promedio | **$7.52** | $7.31 | $6-7 | 🟡 Sube levemente, fuera de meta |
| Gasto Total (lead-gen) | $90.21 | $102.28 | - | — |
| Leads Totales | 12 | 14 | 4-5/día | 🟢 Por encima de meta, pero -14.3% vs ayer |
| CTR Promedio | 2.16% | 2.01% | 3-4% | 🟡 Mejora, sigue bajo meta |
| Impresiones (lead-gen) | 11,766 | 10,962 | - | — |
| Clicks (lead-gen) | 254 | 220 | - | — |
| Campañas activas sin ningún lead | 3 (COL Odoo, PY Beco, SLV Beco) | 1 (SLV Beco) | - | 🔴 Empeoró |
| Mejor campaña del día | GT Odoo ($3.51 CPL, 9 leads) | SLV Odoo ($2.78 CPL, 4 leads) | - | — |
| Cambios de campaña ejecutados hoy | 0 | 0 | - | — |

---

## 📋 Proximas Acciones

- [ ] Revisar SLV \| Beco con máxima prioridad — 3er día consecutivo en cero leads con gasto estable (~$8.40) sin ninguna conversión; evaluar pausar y reasignar presupuesto si no mejora.
- [ ] Monitorear SLV \| Odoo — rompió su racha de 3 días como mejor campaña, cayendo a 1 lead/$8.35 CPL; confirmar si es ruido de un día o señal de fatiga de audiencia/creativo.
- [ ] Dar seguimiento a GT \| Beco por su alta volatilidad (0 → 3 → 1 leads en 3 días); evaluar estabilidad de audiencia o creativo.
- [ ] Verificar en Ads Manager por qué "Evento: gestión de nómina (Odoo)" lleva ya ~4 días sin reportar gasto ni métricas, aunque sin errores de entrega — confirmar `start_time`, presupuesto o calendario.
- [ ] Revisar COL \| Odoo y PY \| Beco, que cayeron de 1 lead ayer a cero hoy sin cambios de presupuesto ni targeting.
- [ ] Generar el Reporte Performance faltante de 2026-11-16 (carpeta `Reports/` solo tiene el de 2026-11-15).
- [ ] Pendiente heredado: decidir el futuro de las campañas históricas pausadas (Toma El control de tu pyme, Pyme Colombia, Pyme El Salvador, etc.) — reactivar, reemplazar formalmente o archivar.

---

## 🔗 Enlaces

- [[Daily notes/2026-11-16 - Resumen del Dia]] — resumen del día anterior.
- [[Reports/2026-11-15 - Reporte Performance]] — último Reporte Performance disponible en el vault (falta el de 2026-11-16).
- Tags: #daily-note #summary #meta-ads #octopus
