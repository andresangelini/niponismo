# ![Niponismo]
[![Apoya en Patreon](https://img.shields.io/badge/apoya%20en-patreon-orange.svg)][Patreon]
[![Lee en Medium](https://img.shields.io/badge/lee%20en-medium-red.svg)][Medium]
[![Join the chat at https://gitter.im/niponismo/Lobby](https://badges.gitter.im/niponismo/Lobby.svg)](https://gitter.im/niponismo/?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Colección de mazos [Anki] para el estudio del idioma nipón.

## Índice
- [Sobre el proyecto](#sobre-el-proyecto)
- [Descarga](#descarga)
- [Actualizar](#actualizar)
- [Cómo usar](#cómo-usar)
- [¿Quiéres ayudar?](#quieres-ayudar)
- [Cómo funciona](#cómo-funciona)
  - [Dependencias](#dependencias)
  - [Tipos de nota](#tipos-de-nota)
  - [Campos](#campos)
  - [Etiquetas](#etiquetas)
- [Bibliografía](#bibliografía)
- [Otras fuentes](#otras-fuentes)
- [Legal](#legal)

## Sobre el proyecto

**Niponismo** es una colección de mazos [Anki] para asistir en el estudio de las diferentes áreas del japonés empleando el [Sistema de Repetición Espaciada][SRE].

Visita la publicación en [Medium] para a acceder a todas las notas gramaticales, saber más sobre el proyecto y mantenerte informado de las últimas novedades. ¡Y por favor no olvides de dejar un comentario con tus opiniones y sugerencias!

## Descarga

1. Dirígete a la página de [publicaciones](https://github.com/andresangelini/niponismo/releases).
2. Busca y descarga la última versión de `Niponismo.apkg`.
3. Abre el archivo con [Anki].

También puedes descargarlo directamente desde los [mazos compartidos] de [Anki].

**IMPORTANTE:** si tienes pensado contribuir debes usar el complemento [CrowdAnki] y usar el archivo `Niponismo.json` en su lugar. Lee la [guía sobre cómo contribuir](../../blob/master/CONTRIBUTING.md) para saber más.

## Actualizar

Simplemente descarga la última versión del archivo y luego importalo desde [Anki]. **_Se recomienda siempre respaldar primero_** con la función de [exportar] antes de realizar cualquier actualización.

## Cómo usar

Si jamás has usado [Anki] antes y no sabes lo que son la **examinación de recuerdo activo (active recall testing)** y la **repetición espaciada (spaced repetition)**, es recomendable que primero leas el [manual de Anki]. Cabe aclarar además, que **este método no es un reemplazo de otros recursos** tales como libros de texto y clases presenciales, sino por el contrario, un complemento.  

La colección está conformada por varios mazos anidados los cuales se distribuyen de la siguiente forma:

- Niponismo
  - Gramática
    - Definiciones
    - Oraciones

Dependiendo de cuál eligamos podremos estudiar todas las áreas juntas o sólo una en particuar.

**Niponismo** es el mazo principal que contiene al resto y es el recomendado parar estudiar ya que el programa se encarga de mezclar las tarjetas de los diferentes mazos de acuerdo a nuestra configuración.

**Gramática** cubre el área gramatical haciendonos repasar tanto las **Definiciones** como las **Oraciones**.

**Definiciones** es un mazo con tarjetas que se estudian en ambas direcciones con la forma gramatical de un lado y la interpretación más aproximada al español del otro.

**Oraciones** está compuesto por tarjetas en donde se presentan oraciones con espacios en blanco en los cuales se debe escribir la gramática apropiada siguiendo las siguientes reglas:

- `A + / + B` se interpreta como **tiene que ir A o B**
- `(X) + A` se interpreta como **tiene que ir A (con o sin X antes)**
- `(X) + A + / + (X) + B` se interpreta como **tiene que ir A (con o sin X antes) o B (con o sin X antes)**
- `(X/Y/Z) + A + / + (X/Y/Z) + B` se interpreta como **tiene que ir A (con o sin X, Y o Z antes) o B (con o sin X, Y o Z antes)**

Algunas oraciones contienen más de un espacio en blanco. En esos casos, lo que va entre dichos espacios se representa en la respuesta con el símbolo `～`. Un ejemplo sencillo es la forma gramatical `だの～だの` o `であれ～であれ～であれ/であろうと～であろうt～であろうと`.

## ¿Quieres ayudar?

Los objetivos de este proyecto son ciertamente ambiciosos pero para nada imposibles si cada uno de nosotros aporta al menos un poco. Si tu también deseas ayudar, por favor empieza por leer la [guía sobre cómo contribuir](../../blob/master/CONTRIBUTING.md).

También puedes apoyarme en **[Patreon]**. ¡Muchas gracias!

## Cómo funciona
Si eres un usuario avanzado de Anki y estás pensando en colaborar o hacer tus propias modificaciones, estas son las cosas que probablemente querrás saber acerca de los mazos.

### Dependencias
- [Japanese Support] - Genera furigana automaticamente usando el tipo de nota "Japanese (recognition)".

### Tipos de nota
 - **Gramática japonesa** - Para tarjetas del mazo "Definiciones".
 - **Japanese (recognition)** - Para tarjetas del mazo "Oraciones".

### Campos
  Los campos y su cantidad dependen del tipo de nota de la tarjeta:

  - **Gramática japonesa**

   - **Japonés** - Aquí va la forma gramatical en kanji.
   - **Furigana** - Escribe la misma forma gramatical en kanji pero con la lectura entre corchetes detrás de cada palabra y dejando un espacio delante de la misma, a menos que se encuentra al principio de la oración. Ejemplo:
   > 今日[きょう]はいい 天気[いい]ですね。

   - **Español** - La interpretación de lo que significa en español.
   - **Ejemplo N°** - Una frase de ejemplo con `＿＿＿` (tres subguiones en entrada japonesa) en lugar de la forma gramatical. Por ejemplo:
   > 僕[ぼく]はそのゲームにはまっちゃった。いつも 始[はじ]めた＿＿＿ 次[つぎ]の 朝[あさ]まで 止[と]められない。

   - **Traducción N°** - La traducción al español. Recuerda que las traducciones siempre deben ser interpretativas, jamás literales.
   - **Audio japonés** - Ruta donde se aloja el archivo de audio en japonés.
   - **Audio español** - Ruta donde se aloja el archivo de audio en español.


  - **Japanese (recognition)**

   - **Expression** - Escribe la frase en japonés con `＿＿＿` en lugar de la forma gramatical así como cualquier conjugación de verbo o partículas que deba usar.
   - **Meaning** - El significado de la oración en español.
   - **Reading** - Campo reservado para el complemento [Japanes Support] el cual agregará la lectura automáticamente.
   - **Grammar** - Escribe aquí la respuesta correcta con kanji. También se debe incluir cualquier estructura gramatical tales como la conjugación de los verbos, partículas, etc.

### Etiquetas
Las tarjetas están organizadas por grupos con el uso de [etiquetas][etiquetas en Anki]. A continuación está una lista del tipo de etiquetadas existentes:

- Mazo al que pertenece (puede ser más de uno si está en un mazo anidado).
- Nivel de estudio.
- Autor de las oraciones de ejemplo y de ejercicio (puede ser más de uno).

## Bibliografía

- [Dictionary of Advanced Japanese Grammar] de Seichi Makino y Michio Tutsui. ISBN-13: 978-4789012959 y ISBN-10: 4789012956.
- [「日本語能力試験」対策日本語総まとめN1文法] de Hitoko Sasaki, Noriko Matsumoto 2010. ISBN 978-4-87217-726-8.
- [Diccionario Japonés-Español Romanizado / ローマ字和西（日本語スペイン語）辞典] de Eduardo López Herrero (Kashibashobo). ISBN 4-7601-1148-4 C3587.

**Descargo**: *los vínculos proporcionados en esta bibliografía son a mero título informativo. Ni este proyecto ni sus contribuidores tienen afiliación alguna con sus autores, editoriales o sitios de venta.*

## Otras fuentes

- [Tae Kim's Guide to Learning Japanese].
- [JGram: The Japanese Grammar Database].

## Legal

[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/deed.es)

Este paquete de mazos se encuentra publicado bajo los términos de la licencia [Creative Commons Attribution 4.0 (CC BY-SA 4.0)][CC BY-SA 4.0] a excepción del siguiente contenido:
- Las oraciones y traducciones identificadas con la etiqueta "tatoeba" pertenecen al proyecto [Tatoeba] y están publicadas bajo la licencia [Creative Commons Attribution 2.0 license (CC-BY 2.0)][CC-BY 2.0].
- Las oraciones identificadas con la etiqueta "jgram" pertenecen al sitio [Jgram] y están publicadas bajo la licencia [Attribution-ShareAlike 2.0 Generic (CC BY-SA 2.0)][CC BY-SA 2.0].

Si crees que me he olvidado de alguien, por favor, no dudes en [hacermelo saber][Gitter].

[Niponismo]: niponismo.svg "Logo de Niponismo"
[Dictionary of Advanced Japanese Grammar]: https://www.amazon.com/Dictionary-Advanced-Japanese-Grammar-English/dp/4789012956
[「日本語能力試験」対策日本語総まとめN1文法]: https://www.amazon.co.jp/%E6%97%A5%E6%9C%AC%E8%AA%9E%E7%B7%8F%E3%81%BE%E3%81%A8%E3%82%81-N1-%E6%96%87%E6%B3%95-%E3%80%8C%E6%97%A5%E6%9C%AC%E8%AA%9E%E8%83%BD%E5%8A%9B%E8%A9%A6%E9%A8%93%E3%80%8D%E5%AF%BE%E7%AD%96-%E4%BD%90%E3%80%85%E6%9C%A8/dp/4872177266/ref=sr_1_6?s=books&ie=UTF8&qid=1523885802&sr=1-6&keywords=%E3%80%8C%E6%97%A5%E6%9C%AC%E8%AA%9E%E8%83%BD%E5%8A%9B%E8%A9%A6%E9%A8%93%E3%80%8D%E5%AF%BE%E7%AD%96+%E6%97%A5%E6%9C%AC%E8%AA%9E%E7%B7%8F%E3%81%BE%E3%81%A8%E3%82%81 "Amazón Japón"
[Tae Kim's Guide to Learning Japanese]: http://www.guidetojapanese.org/spanish/index.html
[JGram: The Japanese Grammar Database]: http://jgram.org/
[Diccionario Japonés-Español Romanizado / ローマ字和西（日本語スペイン語）辞典]: https://www.amazon.es/Diccionario-Japon%C3%A9s-Espa%C3%B1ol-Romanizado-Eduardo-Herrera/dp/4760111484/ref=sr_1_1?ie=UTF8&qid=1523887983&sr=8-1&keywords=Diccionario+Japon%C3%A9s-Espa%C3%B1ol+Romanizado "Amazon España"
[Tatoeba]: https://tatoeba.org/spa/
[Jgram]: http://jgram.org/
[Anki]: https://apps.ankiweb.net/
[manual de Anki]: https://apps.ankiweb.net/docs/manual.es.html
[SRE]: https://apps.ankiweb.net/docs/manual.es.html#repetici%C3%B3n-espaciada
[mazos compartidos]: https://ankiweb.net/shared/info/1221922925
[exportar]: https://apps.ankiweb.net/docs/manual.es.html#exportar
[CrowdAnki]: https://ankiweb.net/shared/info/1788670778
[Kanji Koohii]: https://kanji.koohii.com/
[mazo propio]: https://apps.ankiweb.net/docs/manual.es.html#descargando-mazos-compartidos
[Gitter]: https://gitter.im/niponismo
[Git]: https://git-scm.com/
[cómo contribuir]: https://opensource.guide/es/how-to-contribute/
[Japanese Support]: https://ankiweb.net/shared/info/3918629684
[etiquetas en Anki]: https://apps.ankiweb.net/docs/manual.es.html#a%C3%B1adiendo-etiquetas
[Patreon]: https://www.patreon.com/niponismo
[Medium]: https://medium.com/niponismo
[KanjiHantaa]: https://kanji.koohii.com/profile/KanjiHantaa
[CC-BY 2.0]: https://creativecommons.org/licenses/by/2.0/deed.es
[CC BY-SA 2.0]: https://creativecommons.org/licenses/by-sa/2.0/deed.es
[CC BY-SA 4.0]: https://creativecommons.org/licenses/by-sa/4.0/deed.es
