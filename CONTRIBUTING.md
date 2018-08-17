# Contribuir a Niponismo

¡Muchísimas gracias por decidir contribuir al proyecto! Todos aquellos que hemos estado estudiando este idioma por algún tiempo sabemos lo díficil que puede llegar a ser encontrar buen material en español, especialmente para los niveles más avanzados. Este proyecto apunta a solucionar dicho problema, lo cual no es tarea fácil, pero si trabajamos juntos estaremos mucho más cerca de alcanzarlo.

La siguiente es una guía sobre como contribuir de forma que todos estemos coordinados y organizados desde un principio. Seguirla nos ahorrará tiempo y posibles malentendidos, por lo que es necesario que todo aquél que este pensando en colaborar la lea detenidamente.

## Índice
- [¿Cómo contribuir?](#cómo-contribuir)
- [¿Qué contribuir y qué no contribuir?](#qué-contribuir-y-qué-no-contribuir)
- [Reglas básicas](#reglas-básicas)
- [Tu primera contribución](#tu-primera-contribución)
- [Dependencias](#dependencias)
- [Sistema de versionado](#sistema-de-versionado)
- [Nomenclatura de branches](#nomenclatura-de-branches)
- [Guía de inicio](#guía-de-inicio)
- [Cómo reportar un error](#cómo-reportar-un-error)
- [Cómo hacer una sugerencia](#cómo-hacer-una-sugerencia)
- [Cómo se procesa una contribución](#cómo-se-procesa-una-contribución)
- [Comunidad](#comunidad)

## ¿Cómo contribuir?

Existen varias maneras de contribuir al proyecto:
- **¡Corriendo la voz!** - A pesar de ser tan obvio, es muy fácil pasar por alto algo tan sencillo. Esta es la primera opción ya no requiere ningún conocimiento de Git y sobre [cómo contribuir a un proyecto de Código Abierto]. Si pretendemos ayudar a la mayor cantidad de estudiantes posible, primero se deben enterar de que este material existe. Escribe en tu blog, tuitea, haz videos, manda correos electrónicos (¡pero no spam!) a tus amigos, llámalos, haz señales de humo, lo que sea. En fin, **¡corre la voz!**
- **Reportando errores** - Esto también es muy sencillo. Seguramente encuentres errores mientras estés estudiando. Estos pueden variar desde simples errores tipográficos hasta errores conceptuales de gramática, por ejemplo. Cualquiera sea el tipo de error, si has encontrado uno y quieres reportarlo, lee atentamente la sección sobre [cómo reportar un error](#cómo-reportar-un-error).
- **Haciendo una sugerencia** - ¡Todas la ideas son bienvenidas! Lo que no quiere decir que todas vayan a ser aceptadas. Por lo que en general, si tiene algo que te gustaría mejorar o agergar, asegúrate de que siga estas líneas:
  - **Está dentro de los objetivos de este proyecto** - Nos interesa cubrir los tres aspectos principales del idioma: **gramática**, **kanji** y **vocabulario**, especialmente lo exigido en los exámenes hasta el N1 inclusive. Aprender nombres propios y formas gramaticales antiguas y en desuso no son de ninguna prioridad por el momento.
  - **Debe poderse repasar con tarjetas** - No todo se debe estudiar usando tarjetas. Tanto la comprensión lectora como la auditiva, por ejemplo, son ejercicios diaros que requieren que uno se sumerja en ellos lo más que pueda. No hay forma de entrenarnos en esos aspectos simplemente con tarjetas.
  - **En lo posible, no debe requerir gastos** - Adquirir oraciones ya hechas o mandarlas a hacer, o contrar alguien para darles voz implicarían costos que por el momento preferimos evitar. Dicho esto, ambas son opciones a tener en cuenta en un futuro.
  - **Todo material de terceros debe ser libre** - Si quieres sugerir agregar el material hecho por alguien más, asegúrate primero de que éste esté publicado bajo una licencia que permita el libre uso, copia, modificación y redistribución (con o sin modificación) del mismo. Si no entiendes bien sobre estos temas, visita la página de [Creative Commons].
- **Creando tarjetas** - Sin duda que los objetivos de este proyecto son ambiciosos para una sola persona, por lo que si conoces [Git] y [Anki] o estás dispuesto a aprenderlos, tienes todo lo que se necesita para comenzar a colaborar. Sólo asegúrate de leer el resto de guía primero y recuerda que si hay algo que no entiendas, puedes ponerte en contacto a través de [Gitter].

## ¿Qué contruibuir y qué no contrubuir?

En general, no se admite ningún material que vaya en contra de nuestros [Código de Conducta]. Algunos ejemplos son:
- **Material de terceros cuya licencia no sea libre** - En lo posible, debe estar bajo una licencia compatible con [CC BY 4.0] o [CC BY-SA 4.0].
- **No debe ser ofensivo o ilegal** - No se aceptará material que contenga lenguaje obseno, racismo, discriminación, sea ofensivo o insite a la violencia ni mucho menos que sea ilegal.

## Reglas básicas

- Ante todo, **respetar el [Código de Conducta]**, el cual no es más que un conjunto de reglas básicas que nos ayudan un mantener un mínimo de etiqueta en internet, de la misma forma que mantenemos en persona.
- **No utilices el issue tracker para hacer consultas sobre el uso del paquetes de mazos**. Para ello dirígete a [Gitter].
- Fíjate si lo que quieres agregar ya existe o está en nuestros planes.
- Antes de ponerte a trabajar, **crea un "issue" para consultar y discutir sobre cambios o aportes grandes que quieras hacer**. Si has encontrado un error, dirígete a la sección sobre (#cómo-reportar-un-error).
- **Proveé vínculos** a las fuentes que sustenten el material que quieras agregar o apoyen tu posición en caso de que hayas encontrado algún error. Esto no sólo nos ayuda a verificar la veracidad del contenido sino que también es una buena forma de recopilar material útil.
- Asegúrate que tu aporte **respete el formato ya establecido** (fuente, tamaño y color de texto, etc.). Es importante mantener la unidad visual entre todos los mazos del paquete. Si quieres proponer uno nuevo, crea un nuevo issue.
- Respeta la [nomenclatura de branches](#nomenclatura-de-branches).

## Tu primera contribución

¿No estás seguro por dónde empezar? Si no tienes experiencia con Anki y jamás has colaborando en un proyecto de código abierto, aquí tienes una lista de sugerencias:

- Lee el [Manual de Anki].
- Lee sobre [cómo contribuir a un proyecto de Código Abierto](#cómo-contribuir-a-un-proyecto-de-código-abierto).
- [Aprende Git en 15 minutos]

## Dependencias

- [CrowdAnki] - Necesario para registrar los cambios en los mazos con git.

## Sistema de versionado

Niponismo usa una variación del [versionado semántico] con el cual se denota una versión de la forma `x.y.z` donde:

- `x` se incrementa cuando se cumple una [milestone](../../../milestones) o se produce un **cambio mayor** que **provoca una incompatibilidad** causando **que el usuario pierda su progreso**.
- `y` se incrementa cuando se hace un **cambio menor** como agregar o borrar tarjetas **sin que esto provoque incompatibilidades** que le hagan **perder su progreso al usuario**.
- `z` se incrementa cuando se hacen **correcciones** que **no provoquen incompatibilidades** que le hagan **perder su progreso al usuario**.

## Nomenclatura de branches

El proyecto se divide en dos ramas: `master` y `desarrollo`. La primera es desde donde se hacen las publicaciones y la segunda donde debemos trabajar. Cuando quieras contribuir y haces un **pull request** debes hacerlo apuntando a `desarrollo`.

## Guía de inicio

Para colaborar a este proyecto debes hacerlo desde un **fork**. En líneas generales funciona así:

1. Abre un nuevo **issue** y propone tus cambios usando la planilla de **sugerencia**.
2. Si tu propuesta ha sido aceptada y asignada a ti, procede haciendo un **fork** al proyecto.
3. Clonas tu nuevo repositorio creado a partir del **fork** a tu computadora.
4. Realizas tus cambios en la rama `desarrollo`.
5. Subes tus cambios a tu repositorio **remoto**.
6. Cuando te sientas listo, haces un **pull request**.
7. Si tus cambios son aceptados, has completado tu aporte. De lo contrario, has los cambios sugeridos y repite el proceso desde el **paso 3**.

Si es tu primera vez, asegúrate de leer sobre [tu primera contribución](#tu-primera-contribución) y luego sigue estos pasos más detallados:

1. Entra en tu cuenta de [Github] si aún no lo has hecho.
2. Cuando te sientas listo, crea un nuevo **issue** y propone tu idea o cambio. Por ejemplo, si quieres simplemente agregar tarjetas a un mazo ya existente, titula el **issue** como "Agrega tarjetas de oraciones para...". En cualquier caso, trata de que el título sea claro y conciso.
3. Si tu **issue** es **aceptado**, puedes comenzar a trabajar haciendo un **fork** al proyecto. Guarda nota del **número de issue** ya que te lo pediremos más tarde y luego sí has clic en el botón de **Fork** en la parte superior derecha de la página del repositorio.
4. Teniendo una copia del proyecto en tu cuenta de Github, haz un **clon** de éste a tu computadora para trabajar de forma **local**. Para ello, primero haz clic en el botón de **Clon or download** en la página de tu **fork** y copia el URL que aparece debajo de **Cone with HTTPS**. Luego abre una terminal en tu computadora, navega a la carpeta en donde quieras alojar el proyecto (por ejemplo, "proyectos") y escribe lo siguiente: `git clone <pega el URL aquí>`.
5. Git automáticamente añade el proyecto en tu cuenta al que has clonado como tu repositorio **remoto** y le llama **origin**, de forma que cada vez quieras actualizar dicho repositorio, sólo tienes que escribir: `git push origin <nombre del branch>`. Sin embargo, también querrás agregar tus cambios al proyecto original (del que has hecho un **fork**) una vez que estés listo. Para agregarlo entonces, escribe en la terminal: `git remote add upstream <nuestro repositiorio>`. Llamamos **upstream** a nuestro repositorio del que has hecho el **fork** por convención, pero puedes llamarlo como tu quieras ya que este nombre no se reflejará en **nuestro repositorio**.
6. Aunque técnicamente podrías empezar a trabajar, cualquier cambio que hagas aquí se aplicaría a la **rama** o **branch** principal de **tu resposiotiro**, llamada **master**, lo que no es aconsejable. Por lo tanto, crea un nuevo **branch** sobre el cual trabajar escribiendo en tu terminal: `git checkout -b <nombre del branch>`. El nombre que le des a este **branch** sí se reflejará cuando se agregue a **nuestro repositorio**, por lo que asegúrate bien de respetar nuestra nomenclatura.
7. Trabaja sobre tus cambios usando el archivo `Niponinsmo.json`.
8. Agrega dichos cambios junto a tu nuevo **branch** a **tu repositorio** en **Github** escribiendo `git push origin <nombre de tu branch>` en la terminal.
9. Ve a **tu repositorio** en **Github** y verás que éste automáticamente te ofrece hacer un **pull request**, lo cual no es otra cosa que avisarnos que quieres aportar tus cambios a nuestro proyecto. Junto al **pull request** pon el **número de issue** para que podamos asociarlo con el **issue** que habías abierto.
10. Si tus cambios son **aprobados**, ¡felicitaciones! has hecho tu primer aporte al proyecto. De lo contrario, sigue las instrucciones que te demos para hacer las correcciones que correspondan.
11. Una vez que **tus cambios** hayan sido aceptados, estos serán fusionados con un **merge** en nuestra **rama** de **desarrollo** y tal vez incluso en la **master**, por lo que tendrás que actualizar todas tus **branches**, tanto las de tu repositorio **local** como las de tu **origin** (el que tienes en tu cuenta). Para ello, abre nuevamente la terminal y escribe: `git pull upstream master` para actualizar tu **master** con el nuestro y luego `git pull upstream desarrollo` para actualizar tu **branch** de **desarrollo**.
12. En este punto, ya no necesitas más el **branch** que habías creado porque tus cambios quedaron registrados cuando hicimos el **merge**. Así que puedes borrarlo escribiendo: `git branch -d <nombre de tu branch>`.
13. Ahora actualiza también **tu repositorio en Github** con: `git pull origin master` y `git pull origin desarrollo`.
14. Borra **tu viejo branch** de tu **repositorio en Github** también: `git push --delete origin <nombre de tu branch>`.

Listo, con esto has aprendido a hacer tus propias contribuciones al proyecto. Seguramente parezca demasiado para digerir al principio, pero con la práctica, se vuelve algo así como una segunda naturaleza. Ante todo recuerda siempre de mantener tus repositorios actualizados con: `git pull upstream master`, `git pull upstream desarrollo` para actualizar **tu repositorio local** y luego `gi push origin master` y `git push origin desarrollo` para actualizar **tu respositorio en Github**.

## Cómo reportar un error

1. Asegúrate de que no exista ya un **issue** sobre ese mismo error. Busca incluso entre los **asuntos cerrados** también, ya que podría haber sido reportado y solucionado anteriormente.
2. Corrobora de que realmente se un error. Si no estás seguro, ponte en contacto a través de [Gitter][Gitter/errores].
3. Abre un **issue** por cada error usando la plantilla **Reporte de error**.
4. Ten paciencia y revisa el estatus del **issue** a menudo. Recuerda también que puedes ofrecerte para hacer la corrección tu mismo. De ser así, indícalo también en el mensaje y sigue los pasos de la [Guía de inicio](#guía-de-inicio).

## Cómo hacer una sugerencia

Si crees que se te ha ocurrido una buena idea y quieres aportarla al proyecto, abre un **issue** por cada sugerencia usando la plantilla de **Sugerencia**.

## Cómo se procesa una contribución

Por el momento, este es un proyecto manejado por una sola persona con un itinerario de por sí bastante apretado. En tanto el mismo no adquiera grandes dimensiones, trataré de responder de forma diaria, pero por favor, ten paciencia si me demoro un poco en responder.

Una vez que haya revisado tu **issue** le daré una respuesta y etiquetaré el mismo para que sepas rápidamente si ha sido **aceptado**, **rechazado**, está **pendiente** por alguna razón, etc. El tiempo de respuesta variará segun el tipo de aporte:

- **Reportes de errorer**: tendrán la **máxima prioridad** y se tratará de tenerlos resueltos para la próxima actualización de la **versión actualizada**.
- **Contribuciones**: ya sea que quieras arreglar un error o agregar más tarjetas, se intentarán responder en el mismo día.
- **Sugerencias**: tienen la **mínima prioridad** pero si es posible se intentarán responder dentro del mismo día.

## Comunidad

Nuestra forma principal de contacto es través [Gitter]. Puedes hablar, por ejemplo, sobre la dirección del proyecto en la sala de **desarrollo**, consultar sobre un **error**, hacer una **pregunta** sobre gramática, aportar una **sugerencia** o simplemente conversar sobre nuestro lugar favorito en Japón en la sala **miscelanea**.

[cómo contribuir a un proyecto de Código Abierto]: https://opensource.guide/es/how-to-contribute/
[Código de Conducta]: README.md
[Git]: https://git-scm.com/
[Anki]: https://apps.ankiweb.net/
[manual de Anki]: https://apps.ankiweb.net/docs/manual.es.html
[Aprende Git en 15 minutos]: https://try.github.io/levels/1/challenges/1
[CrowdAnki]: https://ankiweb.net/shared/info/1788670778
[versionado semántico]: https://semver.org/lang/es/
[Github]: https://github.com/
[Creative Commons]: https://creativecommons.org/
[Gitter]: https://gitter.im/niponismo
[Gitter/errores]: https://gitter.im/niponismo/errores
[Gitter/sugerencias]: https://gitter.im/niponismo/sugerencias
[CC BY 4.0]: https://creativecommons.org/licenses/by/4.0/deed.es
[CC BY-SA 4.0]: https://creativecommons.org/licenses/by/4.0/deed.es_ES
