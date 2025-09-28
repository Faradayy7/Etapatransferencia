SnapGallery
SnapGallery es una aplicación móvil desarrollada con Ionic, React y TypeScript, que permite a los usuarios tomar fotos, autenticarse mediante Firebase y gestionar un carrito de compras de imágenes.

Tecnologías utilizadas
Ionic + React: Framework para desarrollo móvil multiplataforma.
TypeScript: Tipado estático para mayor robustez.
Capacitor: Acceso a funcionalidades nativas (cámara, almacenamiento).
Firebase Auth: Autenticación de usuarios.
Context API: Gestión global de estado (autenticación y carrito).
Vite: Herramienta de desarrollo y build.
Cypress: Pruebas end-to-end.
Instalación y configuración
Clona el repositorio

Instala dependencias

Configura Firebase

Crea un proyecto en Firebase Console.
Habilita autenticación por email/contraseña.
Copia la configuración en src/services/firebase.ts.
Inicializa Capacitor

Sincroniza y ejecuta en Android

Estructura del proyecto
src/components/PhotoGallery.tsx: Galería de fotos, botón para tomar foto y agregar al carrito.
src/context/AuthContext.tsx: Contexto de autenticación, login, registro y logout.
src/context/CartContext.tsx: Contexto del carrito, agregar, eliminar y limpiar fotos.
src/pages/Login.tsx y src/pages/Register.tsx: Formularios de autenticación.
src/pages/Cart.tsx: Visualización y gestión del carrito.
src/services/photoService.ts: Lógica para tomar y guardar fotos.
src/services/firebase.ts: Configuración de Firebase.
App.tsx: Rutas y proveedores de contexto.
Funcionalidades principales
Autenticación de usuarios: Registro, login y logout usando Firebase.
Tomar fotos: Utiliza la cámara del dispositivo para capturar imágenes.
Galería de fotos: Visualiza las fotos tomadas en la app.
Carrito de compras: Permite agregar fotos al carrito, eliminar y limpiar el carrito.
Persistencia: Las fotos y el estado del carrito se mantienen durante la sesión.
Exportación a Android: Listo para compilar y ejecutar en dispositivos Android.
Pruebas automáticas: Incluye pruebas end-to-end con Cypress.
Scripts útiles
npm start: Ejecuta la app en modo desarrollo.
npm run build: Compila la app para producción.
npx cap sync: Sincroniza cambios con plataformas nativas.
npx cap open android: Abre el proyecto en Android Studio.
Cómo usar la app
Regístrate o inicia sesión.
Toma una foto usando el botón de la galería.
Agrega fotos al carrito.
Visualiza y gestiona tu carrito desde la página correspondiente.
Exporta y prueba la app en Android.
