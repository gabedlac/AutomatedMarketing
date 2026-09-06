---
date: 2026-09-05
aliases: [resumen-2026-09-05]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-09-05

> [!info] Nota sobre esta entrada (actualizada con datos de cierre)
> Esta nota se generó originalmente al cierre parcial del día (pull en vivo) y se actualizó posteriormente con los datos finales de Meta Ads API una vez cerradas las ventanas de atribución de leads (hasta 72h). No hubo sesiones de trabajo manual sobre las campañas durante el día — el activity log de la cuenta solo registra eventos automáticos de Meta (refresh de audiencias personalizadas `asa_auto_custom_audience`) y los ajustes de presupuesto/pausa aplicados **el día anterior** (2026-09-04) por Gabriel Calderon en los ad sets de prueba A/B de "Toma El control de tu pyme". Ver el desglose completo por campaña en [[Reports/2026-09-05 - Reporte Performance]].

---

## 🎯 Campañas Revisadas (datos finales de cierre)

| Campaña | Status | Gasto | Leads | CPL | CTR |
|---------|--------|-------|-------|-----|-----|
| 🟢 Beco GT | ACTIVE | $9.66 USD | 2 | $4.83 USD | 1.42% |
| 🟢 Toma El control de tu pyme (GT) | ACTIVE | $14.92 USD | 3 | $4.97 USD | 1.87% |
| 🟢 Pyme El Salvador | ACTIVE | $10.55 USD | 2 | $5.28 USD | 1.22% |
| 🔴 Odoo Test | ACTIVE | $3.52 USD | 0 | - | 1.77% |
| ⏸️ Toma El control de tu pyme (USA) | PAUSED | - | - | - | - |
| ⏸️ Accurate Partners - Loyalti | PAUSED | - | - | - | - |
| ⏸️ Conversión Clientes Potenciales - MX | PAUSED | - | - | - | - |
| ⏸️ Conversión Clientes Potenciales - PY | PAUSED | - | - | - | - |
| ⏸️ 🟡 CONVERSIÓN - CLIENTES POTENCIALES | PAUSED | - | - | - | - |

No se realizaron cambios manuales (presupuesto, targeting, copys, pausas) en ninguna campaña durante el día. Los únicos eventos del activity log de la cuenta desde el día anterior son:
- 10 eventos "Custom audience created" (`asa_auto_custom_audience`), generados automáticamente por Meta el 2026-09-04.
- Los 3 ajustes a nivel de ad set aplicados **el día anterior** (2026-09-04, 9:05-9:06 AM) por Gabriel Calderón vía Power Editor — ver sección de Cambios Realizados.

---

## 🔍 Análisis e Insights

- **⚠️ Corrección vs. la lectura en vivo del mismo día:** el pull parcial tomado durante el 2026-09-05 había registrado a Pyme El Salvador con **0 leads**, sumándose a lo que parecía una racha de varios días consecutivos sin conversión, y a Odoo Test con 1 lead. Con el cierre de datos y las ventanas de atribución (que siguen cerrando hasta 72h después), los números finales son: **Pyme El Salvador con 2 leads ($5.28 CPL)** y **Odoo Test con 0 leads**. Es decir, la racha sin leads de Pyme El Salvador en realidad **terminó este día (2026-09-05)**, no el 2026-09-06 como se documentó en el resumen del día siguiente — esa narrativa queda corregida aquí.
- **Reversión de roles inédita:** Odoo Test, la campaña más eficiente de la cuenta en los últimos ~10 días (CPL ~$4.28-4.37), es la única sin ningún lead hoy pese a gasto y CTR normales (1.77%) — probable varianza de un día de bajo volumen o fricción puntual en el formulario/landing, no una caída de creativo o alcance.
- **"Toma El control de tu pyme (GT)" registra su mejor resultado desde el rebalanceo de presupuesto del 2026-09-04:** sube de 2 a 3 leads y el CPL baja de $6.74 (día anterior, cerrado) a $4.97 (hoy, cierre final) — la primera señal clara de que el ajuste (pausar AD Pyme Productividad, subir AD Pyme Excel y AD Pyme Urgencia a $7.50/día) está funcionando.
- **Beco GT duplica sus leads** (1 → 2) y toma el primer lugar del ranking de CPL de la cuenta ($4.83), su mejor día en semanas.
- **CPL promedio de cuenta cae con fuerza a $5.52 USD** (cierre final) — dentro de la meta de $6-7 por primera vez en semanas, una mejora de ~44% vs. los $9.86 USD del día anterior.
- **CTR promedio de la cuenta sube a 1.56%**, el más alto de la semana, aunque sigue muy por debajo de la meta de 3-4%.
- 5 campañas siguen en PAUSED sin actividad ni gasto — sin cambios respecto a días anteriores.

### Comparación vs. el día anterior (2026-09-04, cerrado)

| Métrica | 2026-09-04 | 2026-09-05 (cierre final) | Cambio |
|---------|------|----------------|--------|
| Gasto Total | $39.43 USD | $38.65 USD | 🔻 -2% |
| Leads Total | 4 | 7 | 🟢 +75% |
| CPL Promedio | $9.86 USD | $5.52 USD | 🟢 -44% |
| CTR Promedio | 1.30% | 1.56% | 🟢 +20% |
| Impresiones | 9,969 | 8,543 | 🔻 -14% |
| Clicks | 130 | 133 | 🔺 +2% |
| Reach | 7,778 | 7,161 | 🔻 -8% |

*Nota: estos números reemplazan la comparación "vs. ayer" publicada en la versión parcial de esta nota, que usaba datos de 2026-09-05 aún incompletos (CPL $9.59, 4 leads). Los totales de hoy ya están cerrados: se obtuvieron mediante pull directo a Meta Ads API una vez cerradas las ventanas de atribución de leads.*

---

## ✏️ Cambios Realizados

- **Ninguno el 2026-09-05.** No hubo ajustes de presupuesto, pausas, nuevos copys ni cambios de targeting ese día.
- **Contexto (día anterior, 2026-09-04):** se aplicaron 3 ajustes a nivel de ad set dentro de "Toma El control de tu pyme (GT)", documentados en [[campaigns/Adjustments/2026-09-04 - Updates]]:
  - Pausa de AD Pyme Productividad (0 conversiones con gasto activo).
  - Aumento de presupuesto de AD Pyme Excel: $5/día → $7.50/día (CPL $2.21, ganador del 30-ago).
  - Aumento de presupuesto de AD Pyme Urgencia: $5/día → $7.50/día (CPL $2.19, mejor rendimiento).
  - Objetivo esperado: pasar de 6 a 9 leads/día con el mismo presupuesto total ($15/día) — el cierre del 2026-09-05 es la primera confirmación de que va en la dirección correcta.
- Fuera de Meta Ads: ninguno.

---

## 🔬 Investigación Realizada

- Ninguna investigación de competencia, tendencias o recursos externos registrada este día.

---

## 📊 Datos Clave del Día (cierre final)

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| CPL Promedio | $5.52 USD | $6-7 | 🟢 Dentro y mejor que meta |
| Gasto Total | $38.65 USD | - | - |
| Leads Total | 7 | 4-5 | 🟢 Muy por encima de meta |
| CTR Promedio | 1.56% | 3-4% | 🔴 Bajo |
| CPC Promedio | $0.29 USD | - | - |
| Impresiones Total | 8,543 | - | - |
| Clicks Total | 133 | - | - |
| Reach Total | 7,161 | - | - |

**Mejor campaña del día:** Beco GT — CPL $4.83 USD (más bajo de la cuenta), aunque "Toma El control de tu pyme (GT)" lidera en volumen con 3 leads.
**Campaña a vigilar:** Odoo Test — 0 leads pese a ser normalmente la más eficiente de la cuenta; confirmar si es varianza puntual o el inicio de un problema real.

---

## ✅ Próximas Acciones

- [x] ~~Generar el Reporte Performance formal de 2026-09-05~~ — hecho, ver [[Reports/2026-09-05 - Reporte Performance]].
- [ ] **Corregir la narrativa de "racha sin leads" de Pyme El Salvador en el resumen del 2026-09-06** — el dato final muestra que la racha terminó el 2026-09-05, no el 09-06.
- [ ] Investigar por qué Odoo Test se quedó en 0 leads el 2026-09-05 pese a CTR y gasto normales.
- [ ] Continuar monitoreo diario de CPL en "Toma El control de tu pyme" según el plan de A/B testing — el ajuste del 2026-09-04 muestra aquí su mejor resultado hasta ahora.
- [ ] Investigar por qué el CTR promedio de la cuenta (1.56%) sigue muy por debajo de la meta de 3-4% pese a la mejora de esta semana.
- [ ] Generar reporte de performance con desglose a nivel de anuncio (ad-level) cuando se retome sesión de trabajo activa.

---

## 🔗 Enlaces

- [[Reports/2026-09-05 - Reporte Performance]] - Reporte formal con desglose completo por campaña
- [[Daily notes/2026-09-04 - Resumen del Dia]] - Resumen del día anterior
- [[Daily notes/2026-09-06 - Resumen del Dia]] - Resumen del día siguiente (contiene la narrativa de Pyme El Salvador a corregir)
- [[campaigns/Adjustments/2026-09-04 - Updates]] - Ajustes de presupuesto cuyo primer resultado positivo se confirma hoy

#daily-note #summary #meta-ads #octopus
