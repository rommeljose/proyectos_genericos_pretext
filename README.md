# Proyecto Generico para PreTeXt

Esta es una propuesta y ejemplo base con los requerimientos necesarios para editar un documento (libro, publicación o algún documento genérico) con [**PreTeXt**](https://pretextbook.org/). Usando [**Codespace**](https://docs.github.com/en/codespaces) asociado a este repositorio, lo que permite tener en la nube de GitHub, todo lo necesario para la edición y publicación del documento creado en el formato de preferencia: LaTeX, PDF, web-html, EPUB, cuaderno Jupyter, braille, etc.

[**PreTeXt**](https://pretextbook.org/) es un lenguaje de marcado de las partes lógicas de un documento. El autor, solo debe preocuparse y econcentrarse en capturar sus ideas para compartirlas con otros; pero no en la presentación, ya que de eso se encargan una diversidad de hojas de estilo. [**PreTeXt**](https://pretextbook.org/) es un vocabulario que usa XML; los códigos que se escriben son "marcadores", con etiquetas específicas que describen la estructura semántica de un documento.

El formato de archivo de las fuente de los escritos en [**PreTeXt**](https://pretextbook.org/), son archivos ASCII en texto plano, que se pueden guardar con la extensión .ptx o .xml. Los editores de textos pueden corregir la sintaxis y resaltar los código [**PreTeXt**](https://pretextbook.org/); pero, [**Visual Studio Code**](https://code.visualstudio.com/) -entre otras funciones- tiene un complemento asociado a [**PreTeXt**](https://pretextbook.org/) y sus fuentes en .ptx.

# Uso de este repositorio con Codespaces de GitHub

Luego de crear un Codespace a partir del contenido de la rama *main* de este repositorio, en el terminal de codespace, debe de proceder a instalar  **PreTeXt-CLI** con:

>### $ `pip install pretext`

Para convertir su fuente a uno de los formatos de salida disponibles, digamos HTML, ejecute el comando:

>### $ `pretext build web`

Después de convertir su fuente a, digamos, HTML, puede ver el resultado usando el comando:

>### $ `pretext view web`

**Nota:** Siga los manuales de referencia de [**PreTeXt**](https://pretextbook.org/doc/guide/html/processing-CLI.html#subsection-123) para optimizar y dar luz a sus creaciones.

<img src="https://pretextbook.org/examples/showcase/html/external/ptx-logo.png" alt="drawing" width="200"/>

Cuando esté listo para compartir su proyecto con el mundo, puede copiar el contenido de output/web a cualquier servidor web. Una opción gratuita y cómoda es utilizar GitHub (puede seguir las indicaiones para hacerlo usted siguiendo las indicaciones en el  **gits** de [`rjcg`](https://gist.github.com/rommeljose/b4290459f59de4eb2cc9149ac3b14fae); también puede utilizar `pretext deploy` como se indica en el manual de [**PreTeXt**](https://pretextbook.org/doc/guide/html/processing-CLI.html#subsection-127).

## El flujo de trabajo recomendado para PreTeXt 
Los códigos fuente de los textos y su estructura son procesados por un programa **Python** llamado **PreTeXt-CLI**; que está estrechamente relacionada a [**Visual Studio Code**](https://code.visualstudio.com/). Predesesora a CLI y aún funcional, existe una herramienta llamada [**xsltproc**](https://gnome.pages.gitlab.gnome.org/libxslt/xsltproc.html) que puede procesar las fuentes XML con XSL usadas por [**PreTeXt**](https://pretextbook.org/).

### [Principios de PreTeXt](https://pretextbook.org/doc/guide/html/philosophy.html#paragraphs-7) 
* PreTeXt es un lenguaje de marcado que captura la estructura de libros de texto y trabajos de investigación.
* PreTeXt es legible y escribible por humanos.
* Los documentos PreTeXt sirven como una fuente única que se puede convertir fácilmente a muchos otros formatos, actuales y futuros.
* PreTeXt respeta las buenas prácticas de diseño que se han desarrollado durante los últimos siglos.
* PreTeXt facilita a los autores la implementación de funciones que son comunes y razonables.
* PreTeXt admite documentos en línea que utilizan todas las capacidades de la Web.
* La salida de PreTeXt se diseña seleccionando de una lista de plantillas disponibles, lo que libera al autor de la carga que implica la microgestión del formato de salida.
* PreTeXt es gratuito: el software está disponible sin coste alguno, con una licencia abierta. El uso de PreTeXt no impone ninguna restricción a los documentos preparados con el sistema.
* PreTeXt no es un sistema cerrado: los documentos se pueden convertir a LaTeX y luego desarrollarse utilizando herramientas estándar de LaTeX.
* PreTeXt reconoce que los documentos académicos implican la interacción de autores, editores, académicos, curadores, instructores, estudiantes y lectores, y que cada grupo tiene sus propias necesidades y objetivos.
* PreTeXt reconoce el valor inherente de producir material que sea accesible para todos.
