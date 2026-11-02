# kni-skills

Skills personales organizadas por función. Cada skill contiene instrucciones en `SKILL.md` y, cuando hace falta, referencias locales. Se pueden usar con un agente compatible con ese formato y con las herramientas necesarias para la tarea.

## Skills disponibles

### Refactor de UI — `refactor-ui`

Auditar una interfaz, explorar mejoras, refinar un resultado visual y preparar su implementación. El método es común; la identidad visual, los componentes y las reglas los aporta cada proyecto.

| Skill | Para qué usarla | Qué entrega |
| --- | --- | --- |
| [diagnostico-ui-ux](skills/refactor-ui/diagnostico-ui-ux/SKILL.md) | Analizar una pantalla existente según sus usuarios, tareas, dispositivos y fricciones. | Hallazgos sustentados, lo que conviene conservar y una dirección recomendada. |
| [propuesta-visual-ui](skills/refactor-ui/propuesta-visual-ui/SKILL.md) | Convertir una dirección en una imagen conceptual o un prototipo HTML y refinarla. | Artefactos inspeccionados, decisiones identificadas y alternativas cuando ayudan a resolver una duda. |
| [preparar-implementacion-ui](skills/refactor-ui/preparar-implementacion-ui/SKILL.md) | Entregar el resultado acordado a un agente desarrollador. | Paquete con dónde, qué y por qué cambia; referencias visuales; criterios de aceptación; prompt para proponer un plan antes de implementar. |
| [revision-ui-ux](skills/refactor-ui/revision-ui-ux/SKILL.md) | Revisar una propuesta, un refinamiento o una implementación contra las tareas y decisiones acordadas. | Problemas comprobables, diferencias, aspectos que funcionan y verificaciones pendientes. |

## Orden de uso

1. **Diagnosticar** con `diagnostico-ui-ux`. Compartí la pantalla, quién la usa, qué necesita hacer, los dispositivos relevantes y las fricciones percibidas. La skill puede concluir que la pantalla ya funciona y no requiere un rediseño.
2. **Proponer y refinar** con `propuesta-visual-ui`. Elegí imagen conceptual o HTML según lo que quieras evaluar. Refiná sobre versiones identificadas hasta acordar el resultado. Una imagen no demuestra interacción ni responsive.
3. **Preparar la implementación** con `preparar-implementacion-ui`. Reuní el resultado aprobado y sus recursos. El agente desarrollador primero inspecciona el proyecto y propone un plan para discutir. Tras aprobarlo, lo ejecuta directamente o por hitos según el flujo del proyecto. El plan incluye una autoauditoría visual de la implementación renderizada antes de entregarla, con correcciones, capturas y limitaciones explícitas.
4. **Revisar** con `revision-ui-ux`. Contrastá la implementación con el resultado aprobado y refiná las diferencias concretas. La autoauditoría del desarrollador no reemplaza esta revisión ni la aprobación del usuario.

`revision-ui-ux` también sirve entre rondas de propuesta o para un cambio localizado. No es obligatorio ejecutar todas las skills para una tarea pequeña, repetir un diagnóstico disponible ni producir variantes por el solo hecho de usar una skill.

La aprobación visual y la aprobación del plan son decisiones distintas. El traspaso solicita planificación; no autoriza por sí mismo modificar la aplicación, publicar o desplegar.

## Cómo usarlas

Copiá o instalá la **carpeta completa de la skill** en el directorio de skills que utilice tu entorno, manteniendo `SKILL.md` y sus referencias. La forma de descubrir o invocar skills depende del entorno; también podés indicar explícitamente el nombre y la ubicación de su `SKILL.md`.

Ejemplos de pedidos:

- «Usá `diagnostico-ui-ux` para auditar esta pantalla. Se usa principalmente en móvil y queremos conservar sus funciones actuales».
- «Usá `propuesta-visual-ui` para crear un prototipo HTML de la dirección acordada y comparar dos soluciones para esta decisión pendiente».
- «Usá `preparar-implementacion-ui` para entregar esta versión aprobada a desarrollo. Detallá dónde, qué y por qué cambia, adjuntá los artefactos y pedí un plan antes de implementar».
- «Usá `revision-ui-ux` para comparar esta implementación con el prototipo aprobado y señalar diferencias verificables».

Aportá documentación de producto/diseño, componentes existentes y referencias aceptadas cuando estén disponibles. Las herramientas de navegador o generación de imágenes dependen del medio solicitado; cada skill debe declarar las limitaciones de lo que pudo inspeccionar.

## Organización del repositorio

Las skills se guardan en `skills/<función>/<nombre>/`. Hoy la categoría disponible es `refactor-ui`. Las futuras skills de planes, ajustes o performance tendrán su propia categoría cuando se incorporen.

Cada carpeta debe ser autónoma: sus referencias se resuelven dentro de ella y no dependen de conversaciones, rutas personales ni otra skill instalada. El README es el índice de propósito y orden; `SKILL.md` contiene las instrucciones de ejecución.
