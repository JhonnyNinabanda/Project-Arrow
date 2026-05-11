\subsection{Estructura}

\subsubsection*{Organización general}

El juego se organiza en biomas o zonas temáticas conectadas de forma progresiva. Cada zona introduce nuevos desafíos, refuerza mecánicas previamente aprendidas y aporta información narrativa sobre la caída del castillo.

\subsubsection*{Jardines Marchitos}

Los Jardines Marchitos funcionan como nivel tutorial. Presentan espacios relativamente abiertos, plataformas simples y enemigos básicos. Su objetivo es enseñar movimiento, salto, ataque y recolección sin sobrecargar al jugador.

Los enemigos iniciales pueden incluir esqueletos de baja movilidad y orcos estáticos o de patrulla corta. La arquitectura debe mostrar ruina exterior: árboles secos, estatuas rotas, rejas oxidadas y muros parcialmente destruidos.

\subsubsection*{Mazmorras del Eco}

Las Mazmorras del Eco presentan espacios cerrados, verticalidad, trampas de pinchos y enemigos con patrones más agresivos. En esta zona se introducen murciélagos, arqueros y segmentos donde el jugador debe combinar salto, combate y lectura de peligros ambientales.

\subsubsection*{Torre del Hechicero}

La Torre del Hechicero representa el tramo final del prototipo o de la primera versión completa. Incluye plataformas móviles, zonas de caída libre, enemigos combinados y el combate contra Zarok. Su diseño debe transmitir ascenso, presión y cercanía al origen de la maldición.

\subsubsection*{Construcción técnica del entorno}

El terreno se construye mediante \texttt{Grid} y \texttt{Tilemap} en Unity. Para optimizar colisiones, se recomienda utilizar \texttt{TilemapCollider2D} junto con \texttt{CompositeCollider2D}, permitiendo unificar superficies y reducir cálculos innecesarios.

