# Notificaciones Android Wear — Acciones múltiples

Notificación con tres acciones: Ver mi Perfil, Dar Follow/Unfollow y Ver Usuario, pensada para Android Wear.

"Ver mi Perfil" abre la app en la pantalla principal; "Ver Usuario" lanza una Activity con fotos recientes (envía userId).

"Dar Follow/Unfollow" dispara una llamada al backend (ej. POST /api/follow o /api/unfollow con followerId, followeeId) y debe actualizar el estado.

Implementación: usar NotificationCompat.Action con PendingIntents distintos; la acción de red puede ejecutarse desde un Service o WorkManager.

Probar en emulador o dispositivo Wear y añadir tests para el endpoint y la integración con la notificación.
--
README corto generado según las instrucciones para implementar notificaciones con acciones múltiples en Android Wear.
# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript and enable type-aware lint rules. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.
