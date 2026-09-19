# Incubadora Digital Guanajuato - Prototipo de Validación de Proyectos

Prototipo interactivo desarrollado para la recepción, análisis algorítmico y dictaminación de proyectos de emprendimiento en el Estado de Guanajuato, alineado a las directrices de IDEA GTO y la SDES.

## Requisitos del Sistema
* Cualquier navegador web moderno (Google Chrome, Microsoft Edge, Mozilla Firefox o Safari).
* No requiere instalación de Node.js, servidores locales, bases de datos ni conexión a internet.

## Instrucciones de Despliegue
1. Copie el código fuente proporcionado y guárdelo en un archivo con el nombre `index.html`.
2. Haga doble clic sobre `index.html` para ejecutarlo en su navegador.

## Casos de Prueba para la Demostración

### Caso A: Proyecto de Alto Impacto (Aprobación Directa >= 80%)
1. En Pantalla 1, ingrese datos del solicitante y presione "Iniciar Postulación de Proyecto".
2. En Pantalla 2, seleccione el municipio (ej. León), giro (ej. Tecnologías de la Información) y adjunte un archivo de prueba.
3. En el cuestionario, seleccione **Sí** en al menos 8 de las 10 preguntas.
4. Haga clic en "Enviar Postulación al Comité Directivo".
5. Verifique en Pantalla 3:
   * Vista Emprendedor: Indicador verde de "Aprobado (>=80%)" y folio de trámite generado.
   * Vista Comité: Pestaña con la ficha técnica completa y porcentaje de cumplimiento.

### Caso B: Proyecto en Maduración (En Espera 60% - 70%)
1. Repita el proceso y marque **Sí** en exactamente 6 o 7 de las 10 preguntas.
2. Verifique en Pantalla 3:
   * El sistema clasificará el proyecto con la etiqueta ámbar "En Espera".
   * El mensaje notificará que la solicitud pasa a "Análisis Humano por el Comité".
   * En la Vista Comité, use el botón "Poner en Espera" para simular la resolución técnica.

### Caso C: Proyecto No Elegible (Rechazo < 60%)
1. Responda **Sí** en 5 o menos preguntas.
2. Verifique en Pantalla 3 la etiqueta roja de "Rechazado" y el texto de canalización a talleres formativos.

## Funcionalidad de Decisión del Evaluador
En la Pantalla 3, haga clic en la pestaña superior "Vista Comité Directivo (Evaluador)". El evaluador
gubernamental cuenta con tres botones interactivos de decisión final (Aprobado, En Espera, Rechazado), 
los cuales registran la deliberación en el prototipo y emiten una confirmación en pantalla.