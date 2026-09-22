---
date: 2026-09-22
aliases: [resumen-2026-09-22]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-09-22

> [!warning] Onceava vez consecutiva que la rutina se dispara antes de medianoche Guatemala — sin resolver
> Al momento del pull (2026-09-22 05:51 UTC = **2026-09-21 23:51 hora de Guatemala, GMT-6**), el día calendario 2026-09-22 **todavía no ha comenzado** en la zona horaria de la cuenta Meta Ads. La métrica `date_preset=today` de la API corresponde en realidad a **2026-09-21** (a ~9 min de su cierre real, aún sujeta a la ventana de atribución de leads). Esta nota documenta esa lectura casi-final de 2026-09-21.
>
> Se confirmó vía `list_triggers` que el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") **sigue con el cron `50 5 * * *` (UTC) = 23:50 GT**, sin cambios desde su creación (2026-08-28) y sin cambios desde que se documentó el problema por primera vez (10 ocurrencias previas documentadas en notas anteriores, esta es la onceava). `next_run_at` confirma que disparará mañana a la misma hora. **Acción requerida del usuario:** editar el horario manualmente en https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ, idealmente a las 00:30–01:00 GT.

---

## 🎯 Campañas Revisadas

Lectura casi-final de **2026-09-21** (a ~9 minutos del cierre real, sujeta aún a cambios por ventana de atribución de leads):

| Campaña | Status | Gasto | Leads | CPL | CTR | Emoji |
|---------|--------|-------|-------|-----|-----|-------|
| Toma El control de tu pyme (GT) | ACTIVE | $15.52 | 1 | $15.52 🔴 | 1.52% 🔴 | 🔴 |
| Pyme El Salvador (SV) | ACTIVE | $12.19 | 2 | **$6.10** 🟢 | 1.49% 🔴 | 🟢 |
| Beco (GT) | ACTIVE | $10.46 | 1 | $10.46 🔴 | 1.25% 🔴 | 🔴 |
| Odoo Test (GT) | ACTIVE | $3.97 | 1 | $3.97 🟢 | 2.23% 🟡 | 🟢 |
| **Pyme Colombia (COL) 🆕** | ACTIVE (recién lanzada) | ~$7.19 (de $7.50/día) | N/D — muy reciente | N/D | N/D | 🆕 |
| Toma El control de tu pyme (USA) | PAUSED | $0.00 | - | - | - | ⏸️ |
| Accurate Partners - Loyalti | PAUSED | $0.00 | - | - | - | ⏸️ |
| Conversión Clientes Potenciales - MX | PAUSED | $0.00 | - | - | - | ⏸️ |
| Conversión Clientes Potenciales - PY | PAUSED | $0.00 | - | - | - | ⏸️ |
| 🟡 CONVERSIÓN - CLIENTES POTENCIALES | PAUSED | $0.00 | - | - | - | ⏸️ |

### 🆕 Nueva campaña: Pyme Colombia (primer mercado nuevo desde El Salvador)

El activity log de la cuenta (09-21, hora Guatemala) muestra la creación completa de una campaña nueva **`[2026-08][Lead Generation][Odoo][COL] - Pyme Colombia`**, hecha manualmente por **Gabriel Calderon vía Power Editor** entre las 10:45 PM y 11:02 PM (09-21, hora GT) — no por esta sesión ni por ninguna automatización:

- **22:45–22:46 PM:** 3 imágenes subidas/editadas en la librería de la cuenta (creativos para la nueva campaña).
- **22:59 PM:** Campaña creada con objetivo `OUTCOME_LEADS`, presupuesto inicial **$12.50 USD/día**. Ad set `Toma El control de tu pyme` (COL) creado con optimization goal "Leads", bidding automático, y segmentación: Medellín y Bogotá (+100km), edades 28-50 (mínimo 25), intereses/comportamientos de pequeños empresarios, CEO/Founder, decision makers, Advantage+ audience activado.
- **23:00 PM:** Ad set activado (Pending Process → Active).
- **23:02 PM:** Presupuesto de campaña corregido de $12.50/día a **$7.50/día** (más en línea con el resto de la cuenta) y la duración del ad set acortada (fin: 17 oct → 10 oct).
- **Estado actual:** ACTIVE, `budget_remaining` de solo $0.31 sobre $7.50 — es decir, ya gastó ~$7.19 en su primera hora de vida. Ritmo de gasto agresivo típico de fase de aprendizaje; aún sin leads confirmados ni métricas de CTR/CPL disponibles.

Adicionalmente, el activity log registra un evento de entrega ("Ad delivered", 09-21 11:31 PM) para un anuncio llamado `AD Pyme Urgencia SV_Group_1`, referenciando un `campaign_id` que **no resuelve a ninguna campaña de esta cuenta** al consultarlo directamente — posiblemente ligado a una estructura anterior/duplicada de "Pyme El Salvador". Queda pendiente de investigar, no se especula más sin datos adicionales.

---

## 🔍 Análisis e Insights

- **Expansión a un mercado nuevo:** Colombia es el primer mercado agregado a la cuenta desde que Pyme El Salvador se consolidó. El presupuesto post-corrección ($7.50/día) es razonable frente al resto de la cuenta, pero el gasto casi total de su presupuesto en la primera hora amerita seguimiento cercano mañana para confirmar que no repite el patrón de sobregasto documentado ayer en el ad set "Urgencia" de GT.
- **Los 4 campañas establecidas empeoran fuerte vs. el cierre casi-final de ayer:** CPL promedio ponderado sube de $5.20 a **$8.43** (+62.1%) mientras los leads confirmados caen a la mitad (10 → 5). El gasto de estas 4 campañas también baja (-19.0%), así que la caída de leads no es solo por menos presupuesto — la conversión empeoró.
- **"Toma El control de tu pyme" (GT) marca su peor CPL reciente:** $15.52 con un solo lead, muy por encima de su rango oscilante habitual ($2.43–$9.91 en los últimos 6 cierres). Sigue siendo la campaña más volátil de la cuenta.
- **Beco repite un solo lead a CPL alto ($10.46)**, consistente con su patrón intermitente — no hay evidencia todavía de que el problema de atribución reportado en notas anteriores esté resuelto de forma sostenida.
- **Pyme El Salvador vuelve a ser la campaña más eficiente de la cuenta** ($6.10 CPL, dentro de la meta de $6-7), manteniendo la racha de buen desempeño de días anteriores.
- Ninguna investigación de competencia o tendencias externas se realizó en esta sesión — el foco estuvo en revisar las 5 campañas activas (incluyendo el desglose completo del lanzamiento de Colombia), confirmar el estado del trigger, y revisar el activity log del día.

---

## ✏️ Cambios Realizados

- **Ninguno realizado por esta sesión.** Todos los cambios documentados hoy fueron hechos manualmente por Gabriel Calderon vía Power Editor (Meta Ads Manager), no por esta rutina automatizada:
  - Creación de la campaña **Pyme Colombia** (objetivo Leads, targeting Medellín/Bogotá, Advantage+ audience).
  - Ajuste de presupuesto de campaña: $12.50/día → $7.50/día.
  - Activación del ad set y acortamiento de su fecha de fin (17 oct → 10 oct).
  - Carga de 3 imágenes nuevas a la librería de creativos.
- No se detectaron cambios manuales en las otras 4 campañas activas (GT, Odoo Test, Beco, El Salvador) durante la ventana del día.

---

## 🔬 Investigación Realizada

- Se confirmó el estado del trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` vía `list_triggers`: cron sigue en `50 5 * * *` UTC (23:50 GT), sin cambios desde su creación el 2026-08-28. Onceava ocurrencia consecutiva del disparo prematuro documentada.
- Se revisaron las 5 campañas activas de la cuenta (Toma El control GT, Odoo Test, Beco, Pyme El Salvador, y la nueva Pyme Colombia) a nivel cuenta/campaña.
- Se investigó a detalle el lanzamiento de Pyme Colombia: presupuesto, targeting, ad set, y secuencia completa de cambios vía activity log (09-21, 22:45 PM–23:02 PM hora GT).
- Se intentó resolver el `campaign_id` del evento "Ad delivered" de `AD Pyme Urgencia SV_Group_1`; no correspondió a ninguna campaña consultable en la cuenta — queda abierto para revisión.
- No se realizó investigación externa de competencia ni tendencias de mercado en esta sesión.

---

## 📊 Datos Clave del Día

| Métrica (4 campañas establecidas) | 2026-09-21 (casi-cierre) | 2026-09-20 (casi-cierre, ref. nota anterior) | Variación |
|---------|---------------------------|----------------------------------|-----------|
| Gasto Total | $42.14 | $52.00 | 🔻 -19.0% |
| Leads Confirmados | 5 | 10 | 🔻 -50.0% |
| CPL Promedio (ponderado) | **$8.43** | $5.20 | 🔻 +62.1% |
| CTR Promedio (ponderado) | 1.49% | 1.68% | 🔻 -11.3% |
| CPC Promedio | $0.39 | $0.34 | 🔻 +13.5% |
| CPM Promedio | $5.76 | $5.65 | 🔻 +1.9% |
| Impresiones | 7,312 | 9,203 | 🔻 -20.5% |
| Clicks | 109 | 155 | 🔻 -29.7% |
| Alcance (Reach) | 5,769 | 7,204 | 🔻 -19.9% |
| Mejor CPL del día | Pyme El Salvador: **$6.10** | Pyme El Salvador: $3.91 | Mismo líder, CPL sube |
| Peor CPL del día | Toma El control GT: $15.52 | Beco: $9.91 | Cambio de peor performer |

**Pyme Colombia (nueva, sin comparación previa):** ~$7.19 gastados de $7.50/día de presupuesto, sin leads ni CTR/CPL confirmados aún.

> [!caution] No confirmar como cierre real
> Estas cifras corresponden a una lectura tomada ~9 minutos antes del cierre real de 2026-09-21 y pueden moverse al resolverse la ventana de atribución de leads. Confirmar con el Reporte Performance formal cuando esté disponible (~7 AM GT).

---

## ✅ Próximas Acciones

- [ ] **Editar manualmente el horario del trigger** `trig_01DMJfrsQXaTY5KJntXisDPQ` en https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ — mover de 23:50 GT a ~00:30-01:00 GT (onceava ocurrencia del problema, sigue sin resolverse)
- [ ] Dar seguimiento cercano al lanzamiento de **Pyme Colombia**: confirmar si el gasto casi-total del presupuesto en su primera hora se repite mañana (posible necesidad de ajustar el presupuesto o el pacing) y si empieza a generar leads
- [ ] Confirmar el cierre oficial de 2026-09-21 con el Reporte Performance formal, en particular el salto de CPL de "Toma El control" (GT) a $15.52
- [ ] Investigar el evento de entrega de `AD Pyme Urgencia SV_Group_1` cuyo `campaign_id` no resolvió en la cuenta actual
- [ ] Dar seguimiento al patrón intermitente de Beco (nuevamente 1 solo lead a CPL alto)

---

## 🔗 Enlaces

- [[Daily notes/2026-09-21 - Resumen del Dia]] - Resumen del día anterior (misma alerta de timing, décima ocurrencia)
- [[Reports/2026-09-20 - Reporte Performance]] - Último reporte formal disponible (reporte de 09-21 aún pendiente, se genera ~7 AM GT)
- [[CLAUDE.md]] - Tarea de A/B testing de copys; nueva expansión a Colombia y volatilidad de CPL de "Toma El control" a seguir confirmando

#daily-note #summary #meta-ads #octopus
