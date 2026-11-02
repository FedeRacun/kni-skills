# Paquete y plan

Dimensioná el traspaso al cambio. Un ajuste pequeño no requiere inventar un proyecto, una matriz completa ni una batería de documentos.

## Documento de traspaso

- Identificá producto, pantalla, tarea, dispositivos, versión final y alcance de aprobación. Si no se conoce el commit desplegado, no lo equipares al checkout consultado.
- Por cambio, explicá ubicación, diferencia y motivo. Citá archivos y símbolos comprobados como puntos de entrada, no como un listado obligatorio de archivos a modificar.
- Adjuntá HTML, imágenes, textos y recursos requeridos. Dejá claras su función y procedencia: código de producto, maqueta aproximada, captura renderizada o concepto generado. No conviertas controles simulados, datos ficticios ni navegación decorativa en requisitos nuevos. Evitá arrastrar historiales con conclusiones superadas.
- Separá lo visual acordado de restricciones de datos, permisos y semántica. Detallá qué se mantiene aunque no aparezca en la maqueta: variantes de rol, estados de carga/error, contenido extremo y diferencias de plataforma relevantes. La ausencia en una captura no autoriza su eliminación.
- Identificá conflictos con documentación vigente y decisiones aceptadas que la reemplazan. Pedí actualización acotada como parte del plan; no reescribas la identidad global por una solución de una pantalla.
- Registrá incertidumbres con su consecuencia: qué puede investigar el receptor y qué requiere una decisión del usuario. No conviertas la factibilidad técnica en permiso para degradar silenciosamente la propuesta.

## Prompt para el receptor

Incluí objetivo, ubicación del proyecto y paquete, orden de lectura y alcance de esta primera respuesta. Respetá el proceso del usuario: primero inspección y plan para discutir, después ejecución cuando se apruebe. No invoques automáticamente herramientas, skills o flujos que el receptor quizá no tenga.

Solicitá un plan que explique componentes a reutilizar o extender, capacidades existentes/faltantes, dependencias, posibles adaptaciones, cambios documentales y validación. Si una adaptación modifica composición o comportamiento aceptados, pedí describir el impacto y ofrecer una alternativa antes de ejecutarla. No exijas una nueva aprobación para cada decisión técnica rutinaria.

Para planes extensos, permití proponer hitos ejecutables conforme a las convenciones del proyecto. La aprobación del plan gobierna la ejecución; el traspaso no autoriza por sí solo cambios, commits o despliegues.

## Criterios de aceptación y revisión

Definí comparaciones observables: mismo contenido/estado/rol y anchos relevantes, jerarquía, textos, recursos, acciones, foco y comportamiento. Pedí revisar la aplicación renderizada, no sólo el diff. Compará cada vista con la referencia que representa ese estado; una imagen conceptual no es una especificación exacta de píxeles.

Registrá qué se verificó y qué queda limitado. No impongas píxel perfecto ni aceptes «se parece» como criterio suficiente: buscá fidelidad a decisiones visuales y tareas. Tras implementación, los refinamientos acordados se versionan para evitar comparar contra referencias superadas.

## Autoauditoría del desarrollador

Incluí explícitamente en el prompt y en el plan solicitado una revisión visual del propio agente antes de entregar la implementación. Tras aprobar el plan, el desarrollador debe abrir la aplicación renderizada, comparar con los artefactos acordados en estados, contenido y anchos equivalentes, corregir diferencias dentro del alcance aprobado y revisar lo afectado. No impongas rondas arbitrarias ni hallazgos mínimos; detener cuando las diferencias estén resueltas o haya un límite concreto declarado.

Pedí capturas reales de la versión entregada, resumen de observaciones/correcciones y diferencias o validaciones pendientes. Si no puede inspeccionar el render, debe explicitarlo en lugar de sustituirlo por lectura de código o tests. No autorices rediseños ni adaptaciones materiales por el hecho de autoauditar. La autoauditoría es parte del trabajo del desarrollador; no constituye revisión independiente ni reemplaza la revisión del usuario.
