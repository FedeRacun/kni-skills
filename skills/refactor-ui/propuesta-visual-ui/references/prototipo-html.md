# Prototipo HTML y capturas

Usá un prototipo para evaluar distribución, controles, navegación local y estados. Reutilizá el código, tokens y recursos existentes cuando sean pertinentes y accesibles. Si reproducís su apariencia en HTML autónomo, declaralo como aproximación: no afirmes reutilizar componentes reales si sólo copiaste su aspecto. Elegí un soporte que permita representar la identidad del producto; un visor con estilos propios no debe sustituirla silenciosamente.

## Alcance de la simulación

Construí el mínimo recorrido que haga evaluable la propuesta, con contenido realista y datos ficticios identificados. Implementá las interacciones comprometidas para la revisión: por ejemplo, abrir y cerrar un panel, filtrar resultados o decidir entre continuar y descartar una edición. Conservá estados coherentes entre esos pasos.

No conectes el prototipo a operaciones de producción, importaciones reales ni escrituras de negocio. La simulación de guardar, cobrar o borrar afecta sólo datos ficticios del prototipo. Identificá las acciones fuera de alcance; evitá controles que aparenten funcionar cuando no hacen nada. No agregues backend, dependencias o capacidades nuevas para completar la apariencia.

Usá controles semánticos, etiquetas visibles y foco de teclado. Conservá unidades, estados y definiciones de métricas. Si faltan datos o reglas, mostrarlos como una hipótesis no los convierte en requisitos. Hacé explícitas las decisiones pendientes sin introducir instrucciones de implementación dentro del flujo del producto.

## Verificación visual e interactiva

Renderizá el HTML en un navegador o visor compatible. Revisá anchos y tareas relevantes, con contenido representativo y estados abiertos, vacíos o de error sólo cuando afecten la decisión. Comprobá texto, recortes, superposiciones, acciones duplicadas y continuidad de contexto. Si hay lógica no trivial, verificá al menos un resultado observable del recorrido, además de mirar la pantalla.

Si una prueba automatizada muestra un salto o cambio de foco inesperado, repetí la interacción de forma directa antes de atribuirlo a la interfaz: el controlador puede desplazar el elemento antes del clic. Registrá el viewport observado y las dimensiones de la captura exportada si difieren; una transformación del visor no demuestra un cambio de diseño.

Si la propuesta instruye a operar una interfaz externa, contrastá el recorrido y los nombres de controles con esa plataforma y estado, mediante observación o documentación oficial vigente. No generalices el menú de un navegador a otro ni presentes instrucciones heredadas como comprobadas por haber renderizado el HTML. Explicitá lo no verificado.

Las capturas deben proceder de esa versión renderizada. Si se piden capturas y HTML, entregá ambos; un enlace al prototipo no sustituye las imágenes. Mantené contenido y estado comparables entre versiones. El viewport de navegador no prueba el comportamiento del teclado nativo o de un teléfono físico.

En un refinamiento, identificá el último artefacto relevante y trabajá sobre él. Guardá una versión nueva, conservá la anterior y actualizá sus capturas afectadas. Si no podés acceder al artefacto previo, declaralo antes de reconstruirlo como si fuera una edición fiel.

## Entrega y límites

Mostrá el prototipo mediante el visor disponible y las capturas inline cuando se soliciten. Entregá el archivo HTML o el artefacto ejecutable correspondiente. Identificá versión, estados demostrados, capacidades simuladas y diferencias respecto de la aplicación.

Si no fue posible renderizar, podés entregar el archivo con esa limitación explícita. No afirmes haber verificado apariencia, interacción o responsive sin observarlos. La aprobación de una maqueta tampoco demuestra que la aplicación implementada haya conservado esas propiedades.
