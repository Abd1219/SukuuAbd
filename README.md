# SukuuAbd - Perfil Médico de Emergencia PWA

SukuuAbd es una aplicación web progresiva (PWA) diseñada para proporcionar información médica crítica y contactos de emergencia de manera instantánea mediante el escaneo de un código QR. 

## Características principales

- **Acceso instantáneo:** Información vital disponible sin necesidad de que el rescatista inicie sesión.
- **Seguridad de datos:** Reglas de Firebase configuradas para que solo el propietario pueda editar su información.
- **Contactos duales:** Soporte para dos contactos de emergencia con botones de llamada y WhatsApp directos.
- **Alerta de Emergencia:** Sistema de aviso visual inmediato con botón de llamada al 911 integrado.
- **Ultra ligero:** Diseñado para cargar en menos de 2 segundos en condiciones de red limitadas.

## Tecnologías utilizadas

- **Frontend:** HTML5, CSS3 (Vanilla), JavaScript (ES6+).
- **Backend:** Firebase Firestore (Base de datos), Firebase Auth (Google Sign-In), Firebase Hosting.
- **API Externa:** QRServer para generación dinámica de códigos.

## Instalación y Despliegue

1. Clona el repositorio.
2. Instala el Firebase CLI: `npm install -g firebase-tools`.
3. Inicia sesión: `firebase login`.
4. Inicializa el proyecto: `firebase init`.
5. Despliega: `firebase deploy`.

## Seguridad

Este proyecto utiliza Reglas de Seguridad de Firestore para proteger la privacidad del usuario:
- Lectura pública limitada a documentos individuales (vía ID de QR).
- Listado de colección prohibido para evitar scraping.
- Escritura restringida exclusivamente al dueño del perfil mediante autenticación de Firebase.

---
Desarrollado con ❤️ para salvar vidas.
