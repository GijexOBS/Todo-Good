# Mochila IRL - Todo Good

Bitácora técnica del proyecto para diseñar, documentar y actualizar la mochila IRL de **Todo Good**.

Este documento servirá como memoria viva del proyecto: cada decisión final que tomemos debe quedar registrada aquí para poder hacer updates posteriores sin perder contexto.

> Repo base: `GijexOBS/Todo-Good`  
> Documento: `docs/mochila-irl/bitacora.md`  
> Inicio de bitácora: 2026-06-18

---

## Objetivo del proyecto

Diseñar una mochila IRL estable, modular y mantenible para transmisiones en exteriores de Todo Good, considerando video, audio, energía, conectividad, redundancia, ergonomía y operación real en campo.

La idea principal es construir un sistema donde puedan convivir:

- LiveU como encoder/bonding principal.
- Múltiples dongles USB externos para conectividad celular.
- Adaptadores en L o soluciones de alivio de tensión para evitar que los cables USB se doblen o rompan.
- Router inalámbrico interno para red local y/o dispositivos auxiliares.
- Sistema de energía suficiente para alimentar toda la operación.
- Sony FX3 con rig SmallRig como cámara principal.
- Sistema Accsoon TX/RX para monitoreo o envío inalámbrico según el workflow final.
- Cableado ordenado, reemplazable y fácil de diagnosticar en vivo.

---

## Principios de diseño

1. **Estabilidad primero:** si algo puede fallar por movimiento, calor o tirones, debe asegurarse o tener alternativa.
2. **Modularidad:** cada bloque debe poder cambiarse sin rehacer toda la mochila.
3. **Redundancia razonable:** backups en energía, conectividad y cableado crítico.
4. **Operación simple:** en vivo no debe requerir abrir menús raros o hacer troubleshooting complejo.
5. **Mantenimiento fácil:** cables, adaptadores, baterías y dongles deben poder reemplazarse rápido.
6. **Documentación constante:** cada decisión final se registra aquí.

---

## Decisiones finales

### 2026-06-18 — Creación de la bitácora del proyecto

**Decisión:** Se creó una bitácora específica para el proyecto **Mochila IRL - Todo Good** dentro del repo `GijexOBS/Todo-Good`.

**Archivo:** `docs/mochila-irl/bitacora.md`

**Motivo:** Centralizar las decisiones técnicas del proyecto y evitar perder contexto entre conversaciones, pruebas, compras y rediseños.

**Estado:** Aprobado.

---

### 2026-06-18 — Nombre del proyecto

**Decisión:** Esta línea de trabajo queda nombrada como **Mochila IRL - Todo Good**.

**Motivo:** Identificar claramente el sistema IRL backpack de Todo Good y separarlo de otros proyectos técnicos del canal.

**Estado:** Aprobado.

---

## Decisiones técnicas pendientes

Estas decisiones todavía no están cerradas y deben definirse durante el diseño:

- Modelo exacto de LiveU a utilizar.
- Cantidad final y modelo de dongles USB.
- Router interno recomendado.
- Sistema de energía principal.
- Sistema de energía de respaldo.
- Método de montaje interno de la mochila.
- Distribución física de los equipos dentro de la mochila.
- Flujo de video desde Sony FX3 hacia LiveU.
- Uso exacto del Accsoon TX/RX dentro del workflow.
- Audio principal y audio de backup.
- Cableado USB, Ethernet, HDMI/SDI y alimentación.
- Sistema de ventilación o control térmico.
- Checklist de encendido, operación y apagado.
- Checklist de emergencia para caídas de señal.

---

## Inventario propuesto inicial

> Esta sección es preliminar. Los modelos exactos se irán cerrando como decisiones finales.

### Video

- Sony FX3 como cámara principal.
- Rig SmallRig para montaje, protección y accesorios.
- Accsoon TX/RX para monitoreo o transmisión inalámbrica auxiliar.
- Cable HDMI o SDI según el flujo final hacia LiveU.

### Encoder / Bonding

- LiveU como unidad principal.
- Dongles USB externos para múltiples operadoras.
- Adaptadores USB en L o extensiones cortas con alivio de tensión.

### Red

- Router inalámbrico interno para red local de la mochila.
- Cable Ethernet corto de repuesto.
- Posible switch pequeño si el diseño lo requiere.

### Energía

- Batería principal de alta capacidad.
- Reguladores/conversores según voltajes requeridos.
- Cables DC adecuados para cada equipo.
- Power bank o batería auxiliar para backup.

### Cableado y accesorios

- Cables USB cortos de buena calidad.
- Adaptadores USB en L.
- Cables Ethernet cortos.
- Velcro, bridas reutilizables y organizadores.
- Bolsas internas o panel MOLLE según mochila elegida.
- Etiquetas para identificar cables y puertos.

---

## Template para futuras decisiones

Copiar y completar este bloque cada vez que se cierre una decisión:

```md
### YYYY-MM-DD — Título de la decisión

**Decisión:** 

**Modelo / marca elegida:** 

**Motivo:** 

**Alternativas consideradas:** 

**Impacto en el workflow:** 

**Pendientes relacionados:** 

**Estado:** Aprobado.
```

---

## Notas de trabajo

- Este documento debe actualizarse cada vez que se cierre una decisión final.
- Las ideas preliminares pueden anotarse, pero no deben mezclarse con decisiones aprobadas.
- Las decisiones aprobadas deben ser claras, fechadas y fáciles de rastrear.
- Evitar incluir claves de stream, IPs públicas sensibles, credenciales, números de teléfono privados o datos operativos que no deberían estar en un repo público.
