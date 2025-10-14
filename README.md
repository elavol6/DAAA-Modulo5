# Notificaciones Android Wear — Acciones múltiples

Notificación con tres acciones: Ver mi Perfil, Dar Follow/Unfollow y Ver Usuario, pensada para Android Wear.

"Ver mi Perfil" abre la app en la pantalla principal; "Ver Usuario" lanza una Activity con fotos recientes (envía userId).

"Dar Follow/Unfollow" dispara una llamada al backend (ej. POST /api/follow o /api/unfollow con followerId, followeeId) y debe actualizar el estado.

Implementación: usar NotificationCompat.Action con PendingIntents distintos; la acción de red puede ejecutarse desde un Service o WorkManager.

Probar en emulador o dispositivo Wear y añadir tests para el endpoint y la integración con la notificación.
