\subsection{Mecánicas principales}

\subsubsection*{Movimiento físico}

El movimiento del personaje se controla mediante la manipulación directa de la velocidad del componente \texttt{Rigidbody2D}. Esta decisión técnica busca evitar inercias indeseadas y ofrecer una respuesta inmediata al jugador. La aceleración visual puede ser reforzada mediante animaciones, pero la lectura mecánica debe mantenerse clara y predecible.

\subsubsection*{Sistema de salto}

El salto se implementa mediante una verificación precisa del suelo utilizando \texttt{Physics2D.OverlapCircle} en un punto ubicado a los pies del personaje. Esta detección permite determinar si el jugador está en contacto con una superficie válida antes de autorizar un nuevo salto.

Para mejorar la sensación de peso, el descenso incorpora un multiplicador de caída, conocido como \emph{Fall Multiplier}. Este ajuste incrementa la gravedad efectiva cuando el personaje comienza a caer, evitando saltos excesivamente livianos y proporcionando una respuesta más satisfactoria al aterrizaje.

\subsubsection*{Combate cuerpo a cuerpo para enemigos}

El ataque principal se realiza con espada. El sistema utiliza \emph{triggers} de colisión asociados a ventanas específicas de la animación de ataque. De este modo, el daño no ocurre durante toda la animación, sino en el intervalo donde la espada representa visualmente un impacto válido.

Este enfoque favorece la coherencia entre animación, retroalimentación y resultado mecánico. Además, permite ajustar el balance mediante parámetros como daño base, duración de la ventana activa, tiempo de recuperación y dirección del golpe.

\subsubsection*{Combate a distancia personaje principal}

El ataque secundario consiste en el lanzamiento de flechas mágicas o proyectiles equivalentes. La implementación se basa en la instanciación de prefabs con una velocidad inicial asignada.

\subsubsection*{Economía interna}

Los enemigos derrotados y ciertas áreas secretas otorgan \textbf{Diamantes de Almas}. Estos objetos actúan como moneda interna y pueden intercambiarse en estatuas de guardado o puntos de mejora. Las mejoras principales contempladas son aumento de salud máxima, incremento del daño base y posibles extensiones futuras de energía mágica.

\subsubsection*{Retroalimentación al jugador}

Cada acción relevante debe comunicar su resultado mediante una combinación de animación, sonido, efectos visuales e interfaz. Los golpes deben producir partículas y sacudida leve de cámara; la recolección debe emitir destellos y sonido distintivo; el daño recibido debe reflejarse en la barra de vida, animación de impacto e invulnerabilidad temporal.

