---
name: revision-ui-ux
description: "Trigger: revisar propuesta UI/UX, auditar un prototipo o verificar una implementación visual. Contrasta el resultado con tareas y decisiones acordadas."
license: Apache-2.0
metadata:
  author: FedeRacun
  version: "0.1.1"
---

## Activation Contract

Usá para revisar una propuesta, refinamiento o implementación identificable. Contrastá el resultado con la tarea, las decisiones aceptadas y la evidencia disponible. Un diagnóstico inicial o la creación de otra propuesta pertenece a otra etapa.

## Hard Rules

- Revisá sin modificar artefactos ni datos operativos, salvo que el pedido incluya corregirlos dentro de un alcance definido.
- Separá defectos comprobados, hipótesis y preferencias. No fabriques hallazgos ni exijas cambios para demostrar que revisaste.
- Conservá lo aceptado y evaluá desvíos por sus consecuencias. Si una decisión aceptada causa un problema material, explicalo sin reabrir todo el diseño.
- Una captura no prueba interacción; una maqueta no prueba implementación. No declares aprobaciones del usuario ni garantías que no obtuviste.

## Decision Gates

| Evidencia | Qué revisar |
| --- | --- |
| Imagen conceptual | Contenido, jerarquía e identidad; explicitá límites funcionales. |
| HTML interactivo | Render e interacciones relevantes, además de su código. |
| Aplicación implementada | Recorridos y estados autorizados; correspondencia con lo acordado y regresiones. |
| Refinamiento localizado | Diff, vistas afectadas y conservación de decisiones anteriores. |
| Falta una versión o criterio | Recuperalo si es accesible; delimitá lo no comprobable y preguntá sólo si cambia el juicio. |

## Execution Steps

1. Identificá artefacto, versión, tarea, dispositivo y alcance. Recuperá qué se aceptó, qué sigue propuesto y qué no corresponde reconsiderar.
2. Leé [evidencia y validación](references/evidencia.md). Revisá instrucciones y convenciones del proyecto, respetando su procedimiento de exploración cuando haya código.
3. Inspeccioná el resultado real. Elegí estados representativos según la tarea y el cambio; comprobá contenido, legibilidad, acciones, foco y contexto donde la evidencia permita hacerlo.
4. Contrastá las diferencias con lo acordado y examiná regresiones. Conservá y explicá lo que funciona. No conviertas una preferencia o un caso remoto en bloqueo sin justificar su impacto.
5. Recomendá correcciones proporcionales y validaciones pendientes. Tras una corrección, revisá lo afectado; ampliá sólo ante riesgos o fallas concretos. Cerrá cuando el alcance esté cubierto o haya un límite explícito de evidencia.

## Output Contract

Entregá un juicio acotado al alcance: qué funciona, problemas que impiden la tarea y ajustes menores. Por hallazgo, indicá evidencia reproducible, consecuencia, impacto y frecuencia conocida o por verificar, confianza y recomendación. Separá hipótesis y preferencias; si no encontrás problemas sustentados, decilo.

Registrá versiones y estados revisados, decisiones que se conservan y verificaciones pendientes. Usá capturas o referencias precisas cuando ayuden a comprobar un hallazgo. No uses una puntuación arbitraria como sustituto de razones ni presentes una revisión propia como evaluación independiente.

## References

- [Evidencia y validación](references/evidencia.md): consultá para delimitar observaciones y evitar falsos positivos.
