\section{Diseno de Niveles: Estructura}

\subsection{Organizacion general}

El juego se organiza en biomas o zonas tematicas conectadas de forma progresiva. Cada zona introduce nuevos desafios, refuerza mecanicas previamente aprendidas y aporta informacion narrativa sobre la caida del castillo.

\subsection{Jardines Marchitos}

Los Jardines Marchitos funcionan como nivel tutorial. Presentan espacios relativamente abiertos, plataformas simples y enemigos basicos. Su objetivo es ensenar movimiento, salto, ataque y recoleccion sin sobrecargar al jugador.

Los enemigos iniciales pueden incluir esqueletos de baja movilidad y orcos estaticos o de patrulla corta. La arquitectura debe mostrar ruina exterior: arboles secos, estatuas rotas, rejas oxidadas y muros parcialmente destruidos.

\subsection{Mazmorras del Eco}

Las Mazmorras del Eco presentan espacios cerrados, verticalidad, trampas de pinchos y enemigos con patrones mas agresivos. En esta zona se introducen murcielagos, arqueros y segmentos donde el jugador debe combinar salto, combate y lectura de peligros ambientales.

\subsection{Torre del Hechicero}

La Torre del Hechicero representa el tramo final del prototipo o de la primera version completa. Incluye plataformas moviles, zonas de caida libre, enemigos combinados y el combate contra Zarok. Su diseno debe transmitir ascenso, presion y cercania al origen de la maldicion.

\subsection{Construccion tecnica del entorno}

El terreno se construye mediante \texttt{Grid} y \texttt{Tilemap} en Unity. Para optimizar colisiones, se recomienda utilizar \texttt{TilemapCollider2D} junto con \texttt{CompositeCollider2D}, permitiendo unificar superficies y reducir calculos innecesarios.

