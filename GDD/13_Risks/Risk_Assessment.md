\subsection{Riesgos técnicos}

\subsubsection*{Conflictos de fusión en Unity}

Las escenas \texttt{.unity} y los prefabs pueden ser difíciles de fusionar en Git, especialmente cuando varios integrantes modifican los mismos archivos. Esto puede provocar pérdida de trabajo, conflictos extensos o errores difíciles de rastrear.

\textbf{Mitigación.} Cada integrante trabajará en escenas de prueba separadas, por ejemplo \texttt{Level\_Denis} o \texttt{Level\_Dev2}. Solo una persona responsable integrará prefabs probados en la escena principal. Además, se recomienda hacer commits pequeños y frecuentes.

\subsubsection*{Rendimiento}

La instanciación constante de proyectiles, partículas o textos flotantes puede generar caídas de FPS, especialmente durante combates intensos.

\textbf{Mitigación.} Si las pruebas evidencian problemas de rendimiento, se reemplazará el uso recurrente de \texttt{Instantiate} y \texttt{Destroy} por un sistema de \emph{Object Pooling}. También se revisará el uso de colliders, partículas y actualizaciones por frame.

\subsubsection*{Integración}

Los sistemas de movimiento, combate, enemigos, UI y audio pueden funcionar individualmente pero fallar al integrarse. Este riesgo es común en prototipos con varias áreas de trabajo paralelas.

\textbf{Mitigación.} Se realizarán integraciones semanales en la rama \texttt{dev}. Cada integración debe probar una escena común con los sistemas principales activos.

\subsection{Riesgos de diseño}

\subsubsection*{Scope creep}

El alcance excesivo puede surgir si el equipo intenta crear demasiados niveles, enemigos, mecánicas o sistemas narrativos para el tiempo disponible. Esto puede llevar a una experiencia incompleta y poco pulida.

\textbf{Mitigación.} Se adopta una filosofía de corte vertical. Es preferible completar un nivel con el cien por ciento de las mecánicas principales funcionando que producir varios niveles vacíos o incompletos.

\subsubsection*{Balance}

Una dificultad mal calibrada puede hacer que el juego resulte frustrante o demasiado simple. Esto afectaría la percepción de calidad del prototipo.

\textbf{Mitigación.} Se implementarán variables ajustables para daño, vida, velocidad, recursos y ubicación de checkpoints. El balance final se realizará durante la fase de QA.

