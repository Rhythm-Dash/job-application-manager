# Arquitectura

## Objetivo

Aplicación personal para centralizar ofertas y candidaturas de un único usuario.

## Componentes

```text
Cloud
├── Angular dashboard
├── Firebase Authentication
├── Firestore
└── Backend/Cloud Functions (fase posterior)

PC local
├── Navegador
├── Playwright (fase posterior)
└── Sesiones locales del navegador (nunca en Git)

Plataformas
├── LinkedIn
├── InfoJobs
├── Randstad
├── Manpower
├── Adecco
└── JobToday
```

## Flujo

1. Ejecutar búsquedas.
2. Normalizar ofertas.
3. Eliminar duplicados.
4. Calcular compatibilidad.
5. Mostrar ofertas para revisión.
6. Preparar candidatura.
7. Enviar solo cuando el flujo sea compatible y esté autorizado.
8. Registrar el resultado en Firestore.

## Seguridad

- Firebase Authentication protege el acceso.
- Firestore aplica aislamiento por `userId`.
- No se almacenan contraseñas de portales.
- No se suben sesiones ni perfiles de navegador.
- CAPTCHA y 2FA requieren intervención del usuario.
