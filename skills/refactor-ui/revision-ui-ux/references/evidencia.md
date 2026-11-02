# Evidencia y validación de una interfaz

Identificá qué versión representa cada insumo. Un checkout, una maqueta y una aplicación publicada pueden corresponder a estados distintos. No atribuyas una observación del navegador al código local sin comprobar esa relación. Conservá las referencias aprobadas como contexto de decisión, no como prueba de que la implementación ya las respeta.

## Según el medio

- **Imagen:** verificá contenido visible, jerarquía, claridad e identidad. No infieras foco, áreas táctiles exactas, comportamiento responsive, lectores de pantalla ni operaciones funcionales desde el bitmap.
- **Prototipo:** renderizá y recorré los estados relacionados con la decisión. Distinguí simulaciones de capacidades verificadas de la aplicación. No exijas completar un backend para evaluar una composición.
- **Implementación:** comprobá tareas y restricciones pertinentes, con datos representativos y sin escrituras operativas no autorizadas. No ejecutes cobros, borrados, importaciones ni otras operaciones reales sólo para completar una auditoría. Si hace falta, identificá una prueba segura pendiente.
- **Refinamiento:** compará fuente y vistas relevantes. Un cambio de texto puede exigir ajustar el contenedor; esa dependencia no equivale a rediseñar. Un diff pequeño tampoco demuestra por sí solo un resultado correcto.

## Reproducción y herramientas

Registrá estado, pasos y viewport relevantes para cada problema. La automatización puede desplazar un elemento antes del clic o alterar el foco; verificá una interacción directa antes de atribuir esos efectos al producto. Distinguí el viewport CSS, las dimensiones exportadas y posibles transformaciones del visor. Una captura JPEG no es una referencia sin pérdida para comparación de píxeles.

Evaluá cada dispositivo en sus tareas reales. Pasar de escritorio a móvil puede servir para explorar estados, pero no demuestra que esa transición sea un recorrido habitual. Si un hallazgo depende de enlaces compartidos, cambios de dispositivo o datos extremos, explicitá esa condición y su frecuencia conocida o por comprobar. No descartes un riesgo material sólo por ser infrecuente; justificá su consecuencia.

Comprobá si un control deshabilitado o una capacidad ausente responde a carga, permisos o una decisión de alcance antes de llamarlo defecto. No exijas paridad entre dispositivos ni sustituyas reglas de negocio para que una pantalla resulte más uniforme.

## Cierre

Dimensioná las correcciones al efecto sobre la tarea. Reabrí una decisión aceptada sólo ante evidencia o un nuevo pedido; una alternativa estética por sí sola no invalida lo aprobado. Si falta evidencia, señalá la comprobación que podría cambiar el juicio. Una pantalla puede estar bien resuelta y conservar ajustes menores pendientes.
