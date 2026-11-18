---
date: 2026-11-18
aliases: [resumen-2026-11-18]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-11-18

> [!info] Nota sobre los datos y la fecha
> Esta rutina se ejecutó a las 05:51 UTC (≈ 23:51 del 2026-11-17 en `America/Guatemala`, zona horaria de la cuenta). A esa hora el día local de la cuenta **todavía no cambiaba a 2026-11-18** (confirmado: `date_preset=today` en `ads_get_ad_entities` resolvió a 2026-11-17, idéntico a una consulta explícita con `time_range={"since":"2026-11-18","until":"2026-11-18"}`, que devolvió las campañas sin ninguna métrica porque ese día aún no había comenzado en la zona horaria de la cuenta). Por lo tanto, los datos de "hoy" en esta nota corresponden en realidad al día **2026-11-17** (prácticamente cerrado, faltaban ~9 minutos) de la cuenta `act_2530001557366648` (GT | Octopus Innovations), y los de "ayer" a **2026-11-16** (cierre maduro, consistente con el Reporte Performance ya publicado). Se mantiene el nombre de archivo `2026-11-18` siguiendo el mismo patrón de todas las rutinas anteriores (fecha del sistema al momento de ejecutarse). `ads_account_get_activity_logs` para el rango 2026-11-17 00:00–24:00 (America/Guatemala) solo registró un evento automático de Meta ("Account billed", $720.00 USD), sin cambios manuales de presupuesto, targeting ni creativo. No se encontró `HEAD` desprendido ni rama desactualizada al iniciar la rutina (`git status` limpio, `main` al día con `origin/main`).

---

## 🎯 Campañas Revisadas

Se revisaron las 7 campañas activas de lead-gen + 1 de evento vía `ads_get_ad_entities` (nivel campaña, `date_preset=today`, equivalente a 2026-11-17 en zona horaria de la cuenta):

| Campaña | Status | Gasto | Impresiones | Clicks | CTR | Leads | CPL |
|---|---|---|---|---|---|---|---|
| 🟢 SLV \| Odoo \| CP \| Servicios | ACTIVE | $8.80 | 1,305 | 28 | 2.15% | 4 | **$2.20** |
| 🟢 COL \| Odoo \| CP \| Servicios | ACTIVE | $7.99 | 690 | 9 | 1.30% | 2 | $4.00 |
| 🟢 PY \| Odoo \| CP \| Servicios | ACTIVE | $8.95 | 1,368 | 33 | 2.41% | 2 | $4.48 |
| 🟢 GT \| Beco \| CP \| Conjuntos | ACTIVE | $13.76 | 1,815 | 27 | 1.49% | 2 | $6.88 |
| 🟡 SLV \| Beco \| CP \| Conjuntos | ACTIVE | $7.43 | 1,055 | 16 | 1.52% | 1 | $7.43 |
| 🟡 GT \| Odoo \| CP \| Servicios | ACTIVE | $30.95 | 4,348 | 69 | 1.59% | 4 | $7.74 |
| 🔴 PY \| Beco \| CP \| Conjuntos | ACTIVE | $7.24 | 1,175 | 15 | 1.28% | 0 | — (sin leads) |
| ⚪ Evento: gestión de nómina (Odoo) | ACTIVE (EVENT_RESPONSES, no lead-gen) | $0.00 | 0 | 0 | — | n/a | n/a |

**Resto de la cuenta — todo PAUSED, sin cambios** (confirmado por `ads_account_get_activity_logs`, solo un evento de facturación automática de Meta): "COL \| Beco \| CP \| Conjuntos" y "COL \| Odoo \| CP \| Servicios" (versiones de prueba anteriores), ambos boosts de "Evento: Odoo en Acción", "[2026-08][Lead Generation][Odoo][COL] - Pyme Colombia", "...[USA] - Toma El control de tu pyme", "...[GT] - Toma El control de tu pyme", "...[GT] - Beco", "...[GT] - Odoo Test", "...[SV] - Pyme El Salvador", Accurate Partners - Loyalti, Conversión Clientes Potenciales MX/PY, 🟡 Conversión - Clientes Potenciales.

No se ejecutó ningún cambio de presupuesto, targeting ni creativo hoy — ni desde esta rutina ni manualmente en Ads Manager.

---

## 📊 Análisis e Insights

1. **El CPL blendeado mejora con fuerza y vuelve a quedar dentro de meta:** las 7 campañas de lead-gen generaron 15 leads hoy con $85.12 de gasto → CPL blendeado de **$5.67**, -25.6% frente a los $7.62 (cierre casi final) de ayer, por debajo del rango meta $6-7 por primera vez en varios días.
2. **Leads totales suben +25% (12 → 15):** muy por encima de la meta diaria de 4-5/día, y el nivel más alto reportado en la bóveda hasta ahora.
3. **Las campañas en cero bajan de 3 a 1:** solo PY \| Beco cerró sin leads hoy; COL \| Odoo, SLV \| Beco y GT \| Beco rompieron su racha en cero.
4. **SLV \| Odoo recupera su mejor forma:** de 1 lead/$8.41 CPL ayer a 4 leads/**$2.20** CPL hoy (-74%), la mejora relativa más marcada del día y la campaña más eficiente de la cuenta.
5. **GT \| Beco revierte su mala racha:** de 1 lead/$16.94 CPL ayer a 2 leads/$6.88 CPL hoy (-59%), ahora dentro de meta.
6. **COL \| Odoo rompe su racha en cero** con 2 leads a $4.00 CPL, su mejor resultado reciente registrado en la bóveda.
7. **PY \| Beco acumula al menos 2 días consecutivos sin ningún lead** (0 ayer, 0 hoy), con gasto estable (~$7-9) y ninguna conversión — se convierte en la mancha más persistente de la cuenta hoy.
8. **GT \| Odoo (mayor volumen de la cuenta) retrocede:** leads caen de 9 a 4 y el CPL sube de $3.56 a $7.74 (+117%), aunque sigue aportando el mayor empuje de impresiones/clicks de la cuenta; no hay anomalía detectada que lo explique.
9. **CTR blendeado cae a 1.68% hoy** (vs 2.16% ayer, -22%), empeorando frente a una meta ya exigente de 3-4% — contraste notable con la mejora fuerte en CPL/leads.
10. **`ads_insights_anomaly_signal` no detectó anomalías** (solapamiento de subasta, fatiga de creativo o audiencia estrecha) en los ad sets analizados.
11. **Campaña de evento sigue sin datos** ("Evento: gestión de nómina (Odoo)" ACTIVE pero $0 gasto/impresiones/clicks), continuidad del problema reportado en días anteriores. `ads_get_errors` no devolvió ningún error de entrega bloqueante sobre esta campaña; sigue pendiente de verificación directa en Ads Manager.
12. No hubo ninguna otra sesión de Claude Code activa en la cuenta hoy aparte de esta rutina, y no se realizó investigación externa de competencia o tendencias de mercado.

---

## ✏️ Cambios Realizados

Ninguno en Meta Ads. Solo se hizo lectura/análisis (`ads_get_ad_entities`, `ads_account_get_activity_logs`, `ads_insights_anomaly_signal`, `ads_get_errors`); no se modificó presupuesto, targeting, copy ni creativo de ninguna campaña desde esta rutina ni se detectaron cambios manuales en Ads Manager (solo un cargo automático de facturación de Meta).

No hubo ningún cambio técnico/de repositorio necesario hoy (repo limpio, sin `HEAD` desprendido).

---

## 🔬 Investigación Realizada

- Se consultó `ads_get_ad_entities` (nivel campaña, cuenta `act_2530001557366648`) con `date_preset=today` y `date_preset=yesterday`, y se verificó la resolución real de fechas con `time_range` explícito y con el campo `timezone_name` (`America/Guatemala`) a nivel cuenta.
- Se consultó `ads_account_get_activity_logs` para 2026-11-17 00:00–24:00 (America/Guatemala): un solo evento automático de Meta ("Account billed", $720.00 USD), ningún cambio manual registrado en la cuenta.
- Se ejecutó `ads_insights_anomaly_signal` sobre la cuenta: sin anomalías de solapamiento de subasta, fatiga de creativo o audiencia estrecha.
- Se ejecutó `ads_get_errors` sobre la campaña de evento sin delivery ("Evento: gestión de nómina (Odoo)"): sin errores bloqueantes de publicación.
- Se auditó `git status`/`git log`: rama `main` al día con `origin/main`, sin cambios pendientes.
- Se revisó la carpeta `Reports/`: solo existen los Reportes Performance de 2026-11-15 y 2026-11-16; falta el de 2026-11-17.
- No se realizó investigación externa de competencia ni tendencias de mercado.

---

## 📊 Datos Clave del Día

| Métrica (blendeada, 7 campañas lead-gen) | Hoy (2026-11-17 real) | Ayer (2026-11-16) | Meta | Status |
|---|---|---|---|---|
| CPL Promedio | **$5.67** | $7.62 | $6-7 | 🟢 Mejora fuerte, dentro de meta |
| Gasto Total (lead-gen) | $85.12 | $91.39 | - | — |
| Leads Totales | 15 | 12 | 4-5/día | 🟢 +25% vs ayer, muy por encima de meta |
| CTR Promedio | 1.68% | 2.16% | 3-4% | 🔴 Empeora, bajo meta |
| Impresiones (lead-gen) | 11,756 | 11,918 | - | — |
| Clicks (lead-gen) | 197 | 258 | - | — |
| Campañas activas sin ningún lead | 1 (PY Beco) | 3 (COL Odoo, PY Beco, SLV Beco) | - | 🟢 Mejoró |
| Mejor campaña del día | SLV Odoo ($2.20 CPL, 4 leads) | GT Odoo ($3.56 CPL, 9 leads) | - | — |
| Cambios de campaña ejecutados hoy | 0 | 0 | - | — |

---

## 📋 Proximas Acciones

- [ ] Seguir de cerca PY \| Beco — al menos 2 días consecutivos sin leads con gasto estable (~$7-9); evaluar pausar y reasignar presupuesto si no mejora pronto.
- [ ] Confirmar si la mejora de SLV \| Beco y GT \| Beco (ambas rompiendo rachas negativas) es sostenida o ruido de un día.
- [ ] Monitorear GT \| Odoo tras su retroceso (9→4 leads, CPL $3.56→$7.74) — mayor volumen de la cuenta, vigilar fatiga de audiencia/creativo aunque no se detectó anomalía.
- [ ] Investigar la caída de CTR blendeado (2.16%→1.68%) a pesar de la mejora en CPL/leads — revisar creativo y frecuencia.
- [ ] Verificar en Ads Manager por qué "Evento: gestión de nómina (Odoo)" sigue sin reportar gasto ni métricas, aunque sin errores de entrega — confirmar `start_time`, presupuesto o calendario.
- [ ] Generar el Reporte Performance faltante de 2026-11-17 (carpeta `Reports/` solo tiene hasta 2026-11-16).
- [ ] Pendiente heredado: decidir el futuro de las campañas históricas pausadas (Toma El control de tu pyme, Pyme Colombia, Pyme El Salvador, etc.) — reactivar, reemplazar formalmente o archivar.

---

## 🔗 Enlaces

- [[Daily notes/2026-11-17 - Resumen del Dia]] — resumen del día anterior.
- [[Reports/2026-11-16 - Reporte Performance]] — último Reporte Performance disponible en el vault (falta el de 2026-11-17).
- Tags: #daily-note #summary #meta-ads #octopus
