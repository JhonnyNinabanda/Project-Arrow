\subsection{Comportamiento de enemigos}

\subsubsection*{Modelo general}

La inteligencia artificial se basa en una máquina de estados finitos simplificada. Este enfoque facilita la implementación, depuración y expansión de comportamientos. Los estados principales son patrulla, persecución, ataque y muerte.

\subsubsection*{Patrulla}

En estado de patrulla, el enemigo se desplaza horizontalmente usando \texttt{transform.Translate} o movimiento controlado por físicas. Para detectar bordes, emite un \texttt{Raycast2D} hacia abajo frente a su posición. Si el rayo no detecta suelo, el enemigo gira cambiando su orientación.

\subsubsection*{Persecución}

La persecución se activa cuando el jugador entra en una zona definida por un \texttt{CircleCollider2D} configurado como \emph{Trigger}. Al detectar al jugador, la IA establece como objetivo el \texttt{Transform} del personaje y se aproxima mediante \texttt{Vector2.MoveTowards} o una alternativa compatible con físicas.

\subsubsection*{Ataque}

Cuando la distancia al jugador cae por debajo de un umbral determinado, el enemigo se detiene y activa un \emph{Trigger} en el \texttt{Animator}. La ventana de daño debe sincronizarse con la animación, evitando que el jugador reciba impacto antes de una lectura visual adecuada.

\subsubsection*{Muerte}

Al llegar sus puntos de vida a cero, el enemigo desactiva su \texttt{BoxCollider2D}, cambia su \texttt{Rigidbody2D} a modo cinemático si es necesario y reproduce la animación de muerte. Al finalizar, el objeto se destruye mediante \texttt{Destroy} o se devuelve a un sistema de \emph{Object Pooling} si este ha sido implementado.

