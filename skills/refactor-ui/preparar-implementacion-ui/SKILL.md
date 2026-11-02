---
name: preparar-implementacion-ui
description: "Trigger: traspaso visual, prompt para desarrollo o preparar implementación UI. Empaqueta el resultado acordado y solicita un plan antes de implementar."
license: Apache-2.0
metadata:
  author: FedeRacun
  version: "0.1.2"
---

## Activation Contract

Usá al entregar una propuesta visual a un agente desarrollador. Prepará insumos y un prompt de planificación; no ejecutes la implementación ni repitas el diagnóstico.

## Hard Rules

- Distinguí aprobado, propuesto y pendiente. Una aprobación visual no autoriza implementar ni aprueba capacidades simuladas.
- Identificá versión y alcance de cada artefacto. No mezcles capturas anteriores con la versión final sin explicarlo.
- Conservá el resultado acordado como referencia. No impongas copiar HTML/CSS ni aceptes una aproximación genérica; pedí justificar adaptaciones y hacer visibles sus consecuencias antes de ejecutarlas.
- No modifiques la aplicación ni documentos normativos para preparar el paquete. Señalá actualizaciones necesarias para el plan.

## Decision Gates

| Situación | Acción |
| --- | --- |
| Aprobación parcial o faltante | Prepará lo disponible y explicitá pendientes; no inventes una versión aprobada. |
| Hay checkout | Contrastá alcance con código vigente siguiendo su exploración; registrá versión y diferencias. |
| Sólo hay concepto o capturas | Identificá límites; pedí al receptor evaluar viabilidad, sin atribuir medidas o interacción comprobadas. |
| Falta comportamiento o estado | Separá capacidad existente, simulación y desarrollo por confirmar; no amplíes alcance. |
| Plan grande | Permití segmentación según el flujo del proyecto; no exijas otra skill ni crees hitos innecesarios. |

## Execution Steps

1. Recuperá tarea, decisiones y último resultado aceptado. Leé [paquete y plan](references/paquete-y-plan.md).
2. Contrastá dónde, qué y por qué cambia respecto de la aplicación. Identificá componentes y reglas reutilizables, excepciones aceptadas y dudas técnicas.
3. Reuní artefactos y recursos en un paquete persistente. Verificá rutas y dependencias; no uses localhost, portapapeles o archivos temporales como único acceso. Conservá originales y omití borradores descartados del paquete principal.
4. Generá un prompt autónomo para el receptor: leer instrucciones del proyecto y referencias, inspeccionar implementación vigente, proponer plan y detenerse para discutirlo antes de editar. Incluí el contexto que no puede recuperar de este chat.
5. Comprobá integridad y correspondencia de archivos, versiones, decisiones y estados. Para capturas nuevas, renderizá realmente; si faltan, declaralo. Revisá que el plan solicitado cubra diferencias materiales sin autorizar rediseños.

## Output Contract

Entregá documento de traspaso con dónde, qué y motivos, artefactos versionados, alcance funcional y criterios de aceptación; prompt listo para copiar y rutas utilizables. Indicá aprobación y limitaciones de evidencia.

Pedí incluir en el plan adaptaciones, capacidades faltantes y autoauditoría visual antes de entregar: inspeccionar la aplicación renderizada, comparar referencias, corregir dentro del alcance aprobado y volver a revisar lo afectado. Exigí evidencia y límites; una revisión propia no es independiente. Tras aprobar el plan, ejecución y segmentación siguen el flujo del proyecto; la revisión del usuario permanece pendiente.

## References

- [Paquete y plan](references/paquete-y-plan.md): contenido del traspaso y límites entre diseño, planificación y ejecución.
