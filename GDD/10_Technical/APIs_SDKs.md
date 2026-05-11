\subsection{APIs / SDKs}

\subsubsection*{Unity 6 LTS}

Unity 6 LTS constituye el motor principal del proyecto. Se utiliza por su soporte para desarrollo 2D, herramientas de física, sistema de animación, manejo de escenas, exportación multiplataforma y flujo de trabajo ampliamente documentado.

\subsubsection*{Cinemachine}

Cinemachine se emplea para seguimiento suave de cámara, configuración de \emph{Dead Zones}, transiciones y efectos de sacudida mediante Cinemachine Impulse. Su uso permite mejorar la presentación sin construir desde cero un sistema de cámara complejo.

\subsubsection*{TextMeshPro}

TextMeshPro se utiliza para renderizar textos nítidos en interfaz, diálogos, contadores y textos flotantes. Su calidad visual es superior al sistema de texto clásico de Unity y resulta especialmente útil en resoluciones variables.

\subsubsection*{Git y GitHub}

El repositorio se aloja en GitHub. Git se utiliza para control de versiones, trazabilidad de cambios, trabajo por ramas e integración del equipo. La estructura de ramas propuesta incluye \texttt{main}, \texttt{dev} y ramas de características como \texttt{feature/combate} o \texttt{feature/ui}.

\subsubsection*{Git LFS}

Git LFS es obligatorio para archivos pesados como \texttt{.png}, \texttt{.wav}, \texttt{.mp3} y \texttt{.psd}. Su uso evita saturar el historial del repositorio y mejora la gestión de recursos binarios.

\subsection{Middleware}

Actualmente, el proyecto no contempla la integración de middleware de terceros complejo (como FMOD para audio o Havok para físicas), todas las funcionalidades centrales se resuelven de forma nativa a través de los sistemas y paquetes de Unity mencionados anteriormente.

