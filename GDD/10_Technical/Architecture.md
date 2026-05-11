\subsection{Arquitectura}

\subsubsection*{Patrones de diseño}

El proyecto contempla el uso del patrón \emph{Singleton} en controladores globales como \texttt{GameManager}, \texttt{UIManager} y \texttt{CameraShake}. Este patrón permite garantizar una única instancia de sistemas centrales y facilita accesos como \texttt{GameManager.Instance.UpdateScore()}.

No obstante, el uso de singletons debe mantenerse controlado para evitar acoplamiento excesivo. Los sistemas específicos, como enemigos, proyectiles o recolectables, deben comunicarse mediante referencias claras, eventos o interfaces cuando sea conveniente.

\subsubsection*{Componentes principales}

\textbf{PlayerController.} Gestiona movimiento, salto, lectura de entrada y estados básicos del jugador.

\textbf{CombatController.} Administra ataques cuerpo a cuerpo, proyectiles, tiempos de recuperación y consumo de energía.

\textbf{HealthSystem.} Controla salud, daño, muerte e invulnerabilidad temporal.

\textbf{EnemyAI.} Implementa estados de patrulla, persecución, ataque y muerte.

\textbf{UIManager.} Actualiza HUD, menús, contadores y estados de pantalla.

\textbf{GameManager.} Administra progreso global, pausa, reinicio, guardado temporal y transiciones.

\subsubsection*{Flujo de datos}

El flujo recomendado prioriza una comunicación clara entre sistemas. El jugador recolecta Diamantes de Almas, el sistema de inventario o GameManager actualiza la cantidad disponible, y el UIManager refleja el cambio en pantalla. Del mismo modo, cuando un enemigo recibe daño, su HealthSystem procesa el impacto, instancia retroalimentación visual y notifica la entrega de recompensa al morir.

\subsubsection*{Consideraciones de rendimiento}

La arquitectura debe evitar instanciaciones excesivas durante momentos de combate intenso. Si las pruebas evidencian caídas de FPS, los proyectiles, textos flotantes y efectos recurrentes deben migrarse a un sistema de \emph{Object Pooling}.

