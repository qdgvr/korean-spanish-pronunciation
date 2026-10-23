# Pronunciación: coreano y español

Atlas de pronunciación en español para aprender coreano.

La identidad visual utiliza los colores del material de BBlingua: cian, magenta, naranja, azul claro y gris sobre blanco. El logotipo de la cabecera está reconstruido con contornos SVG integrados en el HTML, con los cuatro colores de la referencia proporcionada; no carga una imagen externa.

**[Abrir la página](https://qdgvr.github.io/korean-spanish-pronunciation/)**

Pulsa una letra coreana en azul para escuchar. Las 18 consonantes con audio reproducen ejemplos con ㅡ (그, 끄, 느, 드, 뜨, 르, 므, 브, 쁘, 스, 쓰, 즈, 쯔, 츠, 크, 트, 프, 흐). La tabla ofrece las vistas Seúl actual y Tradicional, combinaciones y ejemplos en contexto.

La página principal muestra siete bloques: Pronunciación, Mezcla, Sonidos, Trazos, Sílabas, Escucha y Vocabulario. El bloque Pronunciación aparece encima de Mezcla y abre Consonantes, Vocales, Combinaciones y En contexto; «Inicio» vuelve a los bloques. Hay cuatro tipos de ejercicios de pronunciación: elegir el audio de una consonante, trazar una letra, formar una sílaba a partir del audio y elegir la sílaba escuchada. La ronda mixta contiene 16 retos y mezcla libremente los cuatro tipos; cada tipo también dispone de una ronda de 12. «Tipos de práctica» vuelve a la lista de bloques. Se comprueba la respuesta antes de continuar. Los retos, las sílabas y las opciones cambian de orden al azar, también al repetir los pendientes.

Vocabulario aparece después de Escucha. Elige primero el libro 1A, 1B, 2A o 2B y después la unidad. La tarjeta central muestra la palabra coreana; al pulsarla se gira y muestra el significado en español. «Siguiente» abre la siguiente tarjeta por el lado coreano. Al terminar se puede repasar de nuevo o elegir otra unidad. Las 6.136 entradas de las 47 secciones se leen del Excel proporcionado, sin cambiar sus parejas de palabra y significado; las repeticiones entre unidades se conservan. Cada entrada a una unidad y cada repaso generan un orden aleatorio nuevo. La tarjeta también se puede girar con Intro o Espacio. El Excel de vocabulario no se incluye en el repositorio.

Vocabulario utiliza el inicio de sesión con Google mediante Supabase Auth. No se crea una contraseña para BBlingua ni se pide un código. Al entrar por primera vez, la cuenta del estudiante queda pendiente de aprobación del profesor. Pronunciación y los cinco bloques de práctica de hangul siguen abiertos sin iniciar sesión.

La cuenta docente autorizada tiene acceso a los cuatro libros y a «Gestionar alumnos». Desde esa lista puede aprobar a un estudiante eligiendo el libro y la unidad hasta los que tendrá acceso. Se incluyen todas las unidades anteriores, siguiendo el orden 1A → 1B → 2A → 2B: por ejemplo, 2A Unidad 1 abre 1A y 1B completos y la primera unidad de 2A. «Abrir siguiente unidad» amplía el acceso de ese estudiante en una unidad, sin tener que volver a seleccionar su nivel.

Las unidades ya guardadas en la cuenta se conservan. Al cambiar de dispositivo o borrar los datos del navegador, basta con volver a entrar con la misma cuenta de Google. El acceso aprobado no caduca y el estudiante puede consultar sus unidades abiertas sin solicitar un código semanal.

El servidor comprueba el permiso docente antes de mostrar la lista de alumnos o cambiar su acceso. Las tarjetas se cargan desde Supabase por unidad y las políticas de acceso impiden leer unidades bloqueadas o modificar directamente el progreso. Los datos de los alumnos y la lista de docentes no se incluyen en este HTML. El inicio de sesión usa PKCE y solicita únicamente la identidad, el correo y el perfil básico de Google. Las futuras Actividades todavía no forman parte de esta versión.

Sílabas y Escucha utilizan 197 grafías sin 받침 con 188 grabaciones reales y combinaciones que cubren las 21 vocales. How to Study Korean aporta 167 grafías; KLEAR aporta ocho, Yazu Town cuatro y Darakwon 18. Algunas grafías comparten una misma grabación. La selección mantiene la prioridad KLEAR, grabaciones existentes, Darakwon. Las opciones de escucha excluyen grabaciones compartidas y grafías con vocales fusionadas que harían ambigua la respuesta. No se inventan sílabas sin una correspondencia documentada.

Los ejercicios de escritura incluyen 29 letras y 78 trazos. ㄹ se traza en tres pasos: la esquina superior con forma de ㄱ, la barra central de izquierda a derecha y la esquina inferior con forma de ㄴ. ㄲ, ㄸ, ㅃ, ㅆ y ㅉ usan sus propios contornos completos del SVG original; las otras 24 letras conservan las imágenes del PDF proporcionado. Arrastra el círculo azul siguiendo la flecha sobre la imagen gris clara: la parte recorrida se vuelve negra dentro del mismo contorno. Se puede usar ratón, dedo o lápiz mediante eventos de puntero. Se comprobó en navegador de escritorio la escritura de los cinco glifos sustituidos, la composición y escucha de varias sílabas, las respuestas incorrectas y correctas, y la repetición de pendientes. No se ha realizado una prueba física en móvil o tableta.

La página incluye 230 archivos de audio y las 29 imágenes de escritura dentro de `index.html`. Pronunciación y la práctica de hangul funcionan con esos recursos integrados, sin servicios de voz ni TTS. Vocabulario necesita conexión para iniciar sesión y obtener las tarjetas y unidades de la cuenta. No requiere instalación. El archivo Excel original no se publica.

## Fuentes y atribución

Las atribuciones y enlaces originales están en «Fuentes y créditos» dentro de la página. Las grabaciones proceden de KLEAR Integrated Korean, Darakwon, How to Study Korean, Lee Jong-gyu / Yazu Town, Asahi Press, SIL International, el gráfico de la International Phonetic Association (J. Esling y J. House) y colaboradores de Wikimedia Commons.

24 imágenes de escritura conservan los contornos del documento de Twinkl `ejemplo.pdf`, proporcionado por el usuario. Las cinco consonantes dobles proceden de [Hangul jamo characters in Unicode](https://commons.wikimedia.org/wiki/File:Hangul_jamo_characters_in_Unicode.svg), de KSX1026-1, tipografía HCR Dotum, bajo [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Se extrajo cada contorno completo, se ajustó uniformemente su tamaño y se cambió el color a gris. Estas adaptaciones de los cinco glifos mantienen CC BY-SA 4.0. El PDF original no se incluye en el repositorio.

Se incluyen la [licencia MIT de SIL](source_notices/SIL_LICENSE.txt) y los [avisos MIT del cliente de Supabase](source_notices/Supabase_LICENSE.txt). Cada recurso conserva los derechos de su fuente; este repositorio no cambia sus licencias.

## Publicación

GitHub Pages publica la raíz de la rama `main`. Para actualizar la página, sustituye `index.html` por la versión completa revisada, sin el enlace al Excel, y sube el cambio a `main`.
