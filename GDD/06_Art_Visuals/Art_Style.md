\subsection{Estilo gráfico}

\subsubsection*{Dirección artística}

\emph{Chronicles of the Cursed Knight} emplea un estilo visual basado en pixel art inspirado en producciones de 16 y 32 bits, combinado con técnicas modernas de iluminación, partículas y composición multicapa.

La dirección artística busca equilibrar atmósfera gótica, claridad mecánica y coherencia narrativa. Aunque el entorno utiliza una paleta predominantemente oscura y melancólica, los personajes, enemigos y elementos interactivos deben conservar suficiente contraste visual para garantizar lectura inmediata durante la jugabilidad.

La estética general prioriza escenarios decadentes, arquitectura medieval deteriorada y elementos sobrenaturales asociados con corrupción espiritual y ruinas abandonadas.

\subsubsection*{Lenguaje visual}

El diseño del entorno utiliza formas angulares, estructuras fragmentadas y siluetas desgastadas para transmitir decadencia y pérdida. Las zonas afectadas por la corrupción presentan grietas luminosas, vegetación marchita, niebla tenue y deformaciones progresivas de la arquitectura.

En contraste, los elementos vinculados al Eco de Elara utilizan iluminación suave, partículas flotantes y colores fríos o dorados para representar calma, memoria y protección espiritual.

Este contraste visual permite diferenciar claramente las áreas seguras de las zonas dominadas por la corrupción.

\subsubsection*{Formato visual}

La relación de aspecto principal corresponde a 16:9. Se recomienda utilizar una cámara ortográfica con parámetros consistentes y herramientas de \emph{Pixel Perfect} para conservar nitidez en sprites, tiles y animaciones.

El escalado debe evitar deformaciones y preservar la lectura de siluetas, especialmente durante secuencias de combate o desplazamiento rápido.

La interfaz y los efectos visuales deben adaptarse al estilo pixel art sin romper coherencia estética.

\subsubsection*{Parallax 2.5D}

La sensación de profundidad se construye mediante un sistema de parallax multicapa. El escenario se divide en capas de fondo, entorno medio y primer plano, cada una con velocidades de desplazamiento distintas respecto al movimiento del jugador.

Las capas lejanas incluyen cielo, montañas y estructuras del castillo, mientras que los planos cercanos contienen muros, columnas, vegetación y elementos decorativos.

Este enfoque permite generar profundidad visual sin abandonar la jugabilidad bidimensional.

La implementación visual busca reforzar la sensación de aislamiento, escala y decadencia del reino mediante fondos con predominancia de tonos fríos y desaturados.

\subsubsection*{Iluminación y atmósfera}

La iluminación cumple una función tanto estética como narrativa. Las zonas seguras presentan fuentes de luz cálidas y relativamente estables, mientras que las áreas corrompidas utilizan iluminación tenue, contrastes agresivos y efectos de sombra parcial.

Se contempla el uso de niebla ligera, partículas ambientales y variaciones de color para reforzar la sensación de aislamiento y deterioro.

Los efectos luminosos asociados con magia, almas y reliquias deben destacar dentro del escenario para atraer la atención del jugador y reforzar la identidad sobrenatural del mundo.

\subsubsection*{Efectos visuales}

Los efectos visuales contemplados incluyen partículas al impactar enemigos, polvo al aterrizar después de un salto elevado, destellos al recolectar Diamantes de Almas y emisiones de luz en objetos mágicos o rituales.

Para reforzar impactos importantes se propone el uso de \emph{Screen Shake} mediante Cinemachine Impulse, combinado con efectos breves de congelamiento visual (\emph{hit stop}) durante ataques significativos.

Estos recursos buscan mejorar la percepción de impacto, respuesta y peso mecánico.

Asimismo, se considera el uso de pequeños destellos de daño, variaciones temporales de iluminación y efectos de desenfoque leve durante habilidades o encuentros importantes.

\subsubsection*{Criterios de legibilidad}

La legibilidad visual constituye una prioridad de diseño. Los elementos peligrosos deben presentar contraste suficiente y formas reconocibles incluso en escenas oscuras o con múltiples efectos visuales.

Las plataformas deben diferenciarse claramente del decorado, los enemigos deben conservar siluetas identificables y los objetos recolectables deben atraer la mirada sin saturar visualmente la escena.

La composición general busca evitar ruido visual excesivo que pueda afectar la precisión del jugador durante exploración o combate.

El personaje principal debe conservar prioridad visual respecto al entorno mediante contraste cromático, separación de planos y posibles efectos de iluminación sutil alrededor de la silueta.