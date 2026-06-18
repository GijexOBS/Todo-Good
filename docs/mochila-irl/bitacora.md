# Mochila IRL - Todo Good

Bitácora técnica del proyecto para diseñar, documentar y actualizar la mochila IRL de **Todo Good**.

Este documento servirá como memoria viva del proyecto: cada decisión final que tomemos debe quedar registrada aquí para poder hacer updates posteriores sin perder contexto.

> Repo base: `GijexOBS/Todo-Good`  
> Documento: `docs/mochila-irl/bitacora.md`  
> Inicio de bitácora: 2026-06-18

---

## Objetivo del proyecto

Armar una mochila IRL funcional para transmisiones en exteriores de Todo Good, tomando como base una **mochila de fotógrafo** por su estructura, cierres, divisiones internas y compartimentos aprovechables para adaptar equipo técnico de transmisión.

La mochila debe ser estable, modular y mantenible, con capacidad de operar durante varias horas de transmisión de forma independiente. La autonomía debe considerar no solo el encoder, red y accesorios, sino también la cámara principal si se decide alimentarla mediante dummy battery.

La prioridad técnica del sistema será conseguir la mayor estabilidad de red posible usando **bonding con módems USB**, complementado por las demás interfaces disponibles en el LiveU elegido: Ethernet directo, Wi-Fi y cualquier otro enlace soportado por el modelo final.

La primera iteración debe priorizar estabilidad y simplicidad operativa con el flujo **Sony FX3 → LiveU Solo PRO HDMI**, dejando multicámara, ATEM y control remoto como una expansión futura una vez validada la base.

La idea principal es construir un sistema donde puedan convivir:

- LiveU como encoder/bonding principal.
- Múltiples dongles o módems USB externos para conectividad celular.
- Ethernet directo al LiveU como enlace adicional cuando exista una red cableada disponible.
- Wi-Fi como enlace adicional o auxiliar, según estabilidad real en campo.
- Adaptadores en L o soluciones de alivio de tensión para evitar que los cables USB se doblen o rompan.
- Router inalámbrico interno para red local y/o dispositivos auxiliares.
- Sistema de energía suficiente para alimentar toda la operación durante varias horas.
- Posible alimentación de cámara mediante dummy battery si el workflow lo requiere.
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
7. **Autonomía real:** el diseño debe considerar varias horas de transmisión independiente, incluyendo cámara si se alimenta desde la mochila.
8. **Aprovechar compartimentos:** la mochila debe facilitar separación física entre energía, red, encoder, cables y accesorios.
9. **Máximo uso de enlaces:** el diseño debe dejar disponibles las interfaces de red del LiveU elegido, sin bloquear USB, Ethernet o Wi-Fi innecesariamente.
10. **Primera iteración simple:** antes de agregar multicámara, switcher o cerebro de control, se validará una versión base estable de una sola cámara.

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

### 2026-06-18 — Base física, autonomía y estrategia de red

**Decisión:** El sistema se diseñará tomando como base una **mochila de fotógrafo**, aprovechando sus cierres, divisiones internas y múltiples compartimentos para adaptar los módulos de transmisión.

**Modelo / marca elegida:** Pendiente. Primero se define el tipo de mochila; el modelo exacto se decidirá después.

**Motivo:** Una mochila de fotógrafo permite organizar equipo delicado en compartimentos separados, reducir movimiento interno, proteger los módulos y facilitar acceso rápido a cables, baterías, módems, router y encoder.

**Objetivo operativo:** La mochila debe poder aguantar varias horas de transmisión de forma independiente. Esto debe incluir el consumo de red, encoder/bonding, router, accesorios y cámara principal si se decide usar dummy battery.

**Prioridad de red:** Se buscará la mayor estabilidad posible usando bonding con módems USB, idealmente combinando distintas operadoras para reducir riesgo de caída por cobertura irregular.

**Interfaces de red consideradas:** Módems USB, Ethernet directo al LiveU y Wi-Fi. El diseño físico debe permitir usar todas las interfaces disponibles del LiveU elegido.

**Nota técnica:** Se tomará como objetivo de diseño contemplar hasta 6 enlaces simultáneos si el modelo final de LiveU lo soporta, por ejemplo una combinación tipo módems USB + Ethernet + Wi-Fi. Esta cifra queda pendiente de validación contra el modelo exacto que se compre o alquile.

**Impacto en el workflow:** El diseño físico debe separar energía, conectividad, encoder y cableado para que el operador pueda diagnosticar problemas rápidamente durante una transmisión en vivo.

**Pendientes relacionados:** Elegir modelo exacto de mochila, modelo exacto de LiveU, distribución interna, sistema de energía, cantidad/modelo de módems USB, operadoras celulares, router interno y flujo final de cámara hacia encoder.

**Estado:** Aprobado.

---

### 2026-06-18 — Primera iteración de video: FX3 directo a LiveU Solo PRO HDMI

**Decisión:** La primera iteración funcional de la mochila será una configuración de una sola cámara: **Sony FX3 → LiveU Solo PRO HDMI**.

**Modelo / marca elegida:** Sony FX3 como cámara principal y LiveU Solo PRO en versión HDMI como encoder/bonding objetivo para esta iteración.

**Motivo:** Esta arquitectura reduce puntos de falla, consumo, calor, cableado y complejidad operativa. Antes de agregar ATEM, multicámara, dron, cámara inalámbrica o control remoto, se validará una base simple y estable.

**Alternativas consideradas:** Módulo multicámara con ATEM Mini/Extreme, dron, cámara inalámbrica adicional, monitor externo para multiview y control remoto mediante SBC con Companion. Estas ideas quedan como expansión futura, no como requisito de la primera versión.

**Impacto en el workflow:** El operador podrá enfocarse en cámara, audio, energía y estabilidad de red sin depender de switcheo multicámara en campo. La mochila se probará primero como sistema IRL de una sola cámara.

**Pendientes relacionados:** Definir cable HDMI, alivio de tensión, alimentación de FX3, tipo de batería, ubicación del LiveU, cantidad de módems USB, configuración de bonding y pruebas de autonomía.

**Estado:** Aprobado.

---

## Expansiones futuras en evaluación

Estas ideas no forman parte obligatoria de la primera iteración, pero quedan registradas para una versión multicámara posterior:

- ATEM Mini / ATEM Mini Extreme como switcher previo al LiveU.
- Dron como fuente aérea mediante salida HDMI del control, si el modelo de control lo permite.
- Cámara inalámbrica adicional mediante receptor HDMI.
- Monitor externo pequeño para que un asistente pueda ver program/multiview y switchear.
- Raspberry Pi, Orange Pi o mini PC con Companion como cerebro de control para mandar comandos al ATEM.
- Control desde celular/tablet conectado al router interno de la mochila.

---

## Decisiones técnicas pendientes

Estas decisiones todavía no están cerradas y deben definirse durante el diseño:

- Modelo exacto de mochila de fotógrafo.
- Confirmar compra/alquiler del LiveU Solo PRO HDMI u otra alternativa similar si el presupuesto o disponibilidad cambia.
- Cantidad final y modelo de módems/dongles USB.
- Validar cuántos enlaces simultáneos soporta el LiveU elegido.
- Definir si Ethernet directo será solo backup o parte activa del bonding cuando esté disponible.
- Definir si Wi-Fi será parte activa del bonding o solo enlace auxiliar.
- Router interno recomendado.
- Sistema de energía principal.
- Sistema de energía de respaldo.
- Método de montaje interno de la mochila.
- Distribución física de los equipos dentro de la mochila.
- Cable HDMI entre Sony FX3 y LiveU Solo PRO HDMI.
- Sistema de alivio de tensión para HDMI, USB y alimentación.
- Definir si la Sony FX3 usará batería interna, dummy battery o batería dedicada externa.
- Uso exacto del Accsoon TX/RX dentro del workflow.
- Audio principal y audio de backup.
- Cableado USB, Ethernet, HDMI y alimentación.
- Sistema de ventilación o control térmico.
- Checklist de encendido, operación y apagado.
- Checklist de emergencia para caídas de señal.

---

## Inventario propuesto inicial

> Esta sección es preliminar. Los modelos exactos se irán cerrando como decisiones finales.

### Video

- Sony FX3 como cámara principal.
- Rig SmallRig para montaje, protección y accesorios.
- LiveU Solo PRO HDMI como encoder/bonding objetivo de la primera iteración.
- Cable HDMI corto y seguro desde Sony FX3 hacia LiveU Solo PRO HDMI.
- Accsoon TX/RX como posible monitoreo o transmisión inalámbrica auxiliar en fase posterior.

### Encoder / Bonding

- LiveU Solo PRO HDMI como unidad principal objetivo.
- Módems/dongles USB externos para múltiples operadoras.
- Ethernet directo al LiveU para usar red cableada cuando esté disponible.
- Wi-Fi como enlace adicional o auxiliar, según pruebas de estabilidad.
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
- Posible dummy battery para alimentar la Sony FX3 desde el sistema principal o desde una batería dedicada.

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