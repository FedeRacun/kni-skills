---
name: diagnostico-ui-ux
description: "Trigger: auditoría UI/UX, analizar una pantalla o sus fricciones. Diagnostica interfaces existentes y recomienda una dirección antes de prototipar."
license: Apache-2.0
metadata:
  author: FedeRacun
  version: "0.1.4"
---

## Activation Contract

Usá para diagnosticar una pantalla existente desde las tareas de sus usuarios. Tratá las observaciones del usuario como hipótesis. Una petición exclusiva de generar imágenes, implementar o verificar una implementación pertenece a otra etapa.

## Hard Rules

- Diagnosticá sin modificar la aplicación ni datos operativos. El diagnóstico no autoriza prototipos o implementación posteriores.
- Separá hechos, hipótesis y preferencias. Identificá la evidencia y sus límites; no atribuyas pruebas de interacción a una captura.
- Conservá semántica, cálculos y permisos. No inventes datos o certezas operativas para mejorar la presentación.
- Permití concluir que algo funciona o requiere un cambio pequeño; no fabriques defectos ni cuotas de hallazgos.

## Decision Gates

| Situación | Acción |
| --- | --- |
| Falta contexto | Investigá primero; preguntá sólo lo que cambie la recomendación. |
| Sólo hay capturas o relato | Analizá lo disponible y explicitá qué falta comprobar. |
| Una regla visual perjudica la tarea | Proponé el desvío, motivo y alcance; distinguí composición de identidad. |
| Hay métricas o gráficos | Explicitá su significado y agregación temporal; no asumas que todos los valores se suman. |
| Se solicita investigación externa o hace falta contrastar un patrón | Leé [investigación](references/investigacion.md). |

## Execution Steps

1. Identificá usuario, tarea, frecuencia, dispositivo y resultado esperado. Recuperá decisiones previas y qué se quiere conservar.
2. Revisá las instrucciones locales, documentación vigente y componentes relevantes. Respetá el procedimiento de exploración del proyecto. Confirmá checkout y versión; recorré la pantalla real si es accesible. Solicitá iniciar sesión cuando haga falta, sin pedir credenciales.
3. Evaluá jerarquía, distribución, densidad, legibilidad, acciones, feedback y estados relevantes para esa tarea. Detectá decisiones repetidas que el contexto ya resuelve. Considerá móvil, teclado, navegación y accesibilidad según la evidencia disponible.
4. Recomendá una dirección proporcional al problema. Identificá reutilización, excepciones visuales y capacidades funcionales. Si no verificaste su existencia, marcala por comprobar; no afirmes que requiere desarrollo nuevo.
5. Cuestioná tu propuesta: contexto perdido, acciones ambiguas, información oculta, contenido extremo y regresiones. Refiná ante problemas concretos; no prolongues el análisis por pulido indefinido.

## Output Contract

Entregá una explicación dimensionada al pedido con:

- Tarea comprendida, alcance y límites de observación.
- Hallazgos priorizados por impacto y frecuencia en el uso real (o por verificar): evidencia, consecuencia y recomendación. Qué funciona y se conserva.
- Dirección recomendada, motivos, desvíos del diseño y costos funcionales.
- Autocrítica, validaciones pendientes y preguntas materiales.
- Traspaso breve: decisiones confirmadas, propuestas, alternativas descartadas y dudas, para continuar con imágenes o HTML. No presentes recomendaciones como aprobaciones. Guardalo en un archivo cuando se solicite documentación.

## References

- [Investigación de patrones](references/investigacion.md): consultá al investigar fuentes externas.
