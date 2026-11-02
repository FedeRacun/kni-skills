---
name: propuesta-visual-ui
description: "Trigger: propuesta visual UI/UX, boceto de pantalla, maqueta HTML o refinamiento visual. Materializa y refina una dirección de interfaz."
license: Apache-2.0
metadata:
  author: FedeRacun
  version: "0.1.3"
---

## Activation Contract

Usá para representar o refinar una interfaz en imagen o prototipo. Recuperá el diagnóstico disponible; no exijas ejecutar otra skill si ya alcanza el contexto.

## Hard Rules

- Creá propuestas aisladas; el pedido de una maqueta no autoriza modificar la aplicación ni operar sobre sus datos.
- Conservá decisiones aceptadas salvo nueva instrucción. Distinguí aprobación de composición, identidad y comportamiento; no extiendas una aceptación parcial.
- Mantené semántica, datos necesarios y permisos. Identificá ejemplos y simulaciones; no presentes controles dibujados como funcionalidad existente.
- Partí de la identidad y componentes del proyecto. Justificá los desvíos propuestos; no introduzcas otra estética por defecto del generador o visor.

## Decision Gates

| Pedido o necesidad | Acción |
| --- | --- |
| Imagen conceptual o exploración estética | Leé [imagen conceptual](references/imagen-conceptual.md). |
| HTML, interacción o captura fiel de controles y texto | Leé [prototipo HTML](references/prototipo-html.md). |
| «Imagen» sin técnica especificada | Elegí según la decisión a resolver; explicá si es concepto generado o captura renderizada. |
| Contexto insuficiente | Recuperá referencias y código relevantes; preguntá sólo lo que cambie la dirección. |
| Refinamiento localizado | Modificá lo pedido y sus dependencias visuales; preservá el resto. |

## Execution Steps

1. Resumí tarea, dirección propuesta, decisiones aceptadas, identidad y dudas materiales. Distinguí recomendaciones de requisitos; no reinicies el diagnóstico sin motivo.
2. Elegí el medio y los estados que permitan juzgar la propuesta. Si hay código, confirmá checkout y respetá las instrucciones de exploración del proyecto.
3. Producí una dirección recomendada con contenido representativo. Mostrá alternativas sólo si resuelven una decisión abierta o se solicitan. Adaptá escritorio y móvil a sus tareas; cubrí los formatos pedidos.
4. Inspeccioná el artefacto real: texto, contenido, jerarquía, identidad, estados y anchos relevantes. Corregí fallas observadas; explicitá lo que no pudiste verificar.
5. Al refinar, conservá una versión anterior y regenerá las vistas afectadas. Contrastá la entrega con las decisiones; no prolongues rondas sin un problema concreto.

## Output Contract

Mostrá el artefacto solicitado en la conversación y enlazá los archivos entregables. Explicá cambios y motivos, qué se conserva, simulaciones, desvíos y límites de validación. Actualizá un traspaso breve con decisiones aceptadas, propuestas y dudas para el siguiente refinamiento o implementación. No declares implementado o aprobado lo que sólo representaste.

## References

- [Imagen conceptual](references/imagen-conceptual.md): generación o edición de una dirección estética.
- [Prototipo HTML](references/prototipo-html.md): interacción simulada y capturas de una interfaz renderizada.
