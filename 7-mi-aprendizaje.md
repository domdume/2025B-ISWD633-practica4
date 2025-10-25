# MI APRENDIZAJE
1. Optimización del ciclo de vida del Build

  El entendimiento profundo del mecanismo de caché de Docker es un pilar central. He asimilado que un Dockerfile no es un script monolítico, sino una receta para crear capas inmutables e independientes. Esta comprensión es vital en entornos de Integración Continua (CI/CD), donde la reducción de los tiempos de build (minutos vs. segundos) impacta directamente en la velocidad de entrega del software.

2. Gestión de recursos y resiliencia (Runtime)
- Limitación de Recursos (--memory, --cpus): entendí el porqué es crucial (evitar el "noisy neighbor" o "vecino ruidoso", garantizar la estabilidad en entornos compartidos).
- Políticas de Reinicio y Healthchecks: un contenedor no solo debe iniciar, sino mantenerse saludable. La combinación de HEALTHCHECK (para que Docker sepa si la aplicación dentro del contenedor funciona) y las políticas de reinicio (para actuar en consecuencia) es la base de la alta disponibilidad y los sistemas auto-reparables.
3. Higiene del entorno

  Revisé sobre la identificación y eliminación de imágenes huérfanas (dangling images) demuestra una buena práctica de administración, esencial para no saturar los recursos del host y mantener un entorno de desarrollo limpio.

Las prácticas han disminuido la brecha entre "saber qué es Docker" y "saber usar Docker en un entorno productivo".
