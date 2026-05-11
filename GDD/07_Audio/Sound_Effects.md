\subsection{Efectos de sonido}

\subsubsection*{Principios generales}

Los efectos de sonido deben proporcionar retroalimentación inmediata y contribuir a la atmósfera. Cada acción importante del jugador debe tener una respuesta sonora reconocible: pasos, salto, aterrizaje, golpe de espada, impacto contra enemigo, recolección y daño recibido.

\subsubsection*{Efectos principales}

\textbf{Pasos.} Deben variar ligeramente en tono mediante código para evitar repetición perceptible. La superficie del nivel puede modificar el timbre en fases posteriores.

\textbf{Espada.} Los ataques deben incluir sonidos metálicos, desplazamiento de aire y un impacto diferenciado cuando el golpe conecta con un enemigo.

\textbf{Recolección.} Los Diamantes de Almas deben emitir un sonido agudo y breve, similar a una campana cristalina, para reforzar la satisfacción de obtención.

\textbf{Daño.} El daño recibido por el jugador debe tener un sonido claro pero no excesivamente intrusivo. Los enemigos pueden utilizar variaciones según tipo o tamaño.

\subsubsection*{Implementación técnica}

Los objetos clave deben utilizar componentes \texttt{AudioSource}. La gestión de volumen, mezcla y reproducción puede centralizarse mediante un administrador de audio, permitiendo separar música, efectos y posibles voces.

