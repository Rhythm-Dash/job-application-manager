# Job Application Manager

Sistema personal para centralizar la búsqueda, evaluación, seguimiento y automatización asistida de candidaturas laborales.

## Alcance inicial

- Un único usuario.
- LinkedIn, InfoJobs, Randstad, Manpower, Adecco y JobToday.
- Dashboard Angular.
- Firebase Authentication + Firestore.
- Automatización local mediante navegador, con intervención del usuario cuando sea necesaria.
- Sin almacenamiento de contraseñas de portales en Firestore o Git.

## Estructura

- `frontend/`: aplicación Angular.
- `firebase/`: reglas e índices de Firestore.
- `automation/`: automatización local.
- `platforms/`: adaptadores específicos por plataforma.
- `docs/`: arquitectura y fases del proyecto.

## Principio de desarrollo

Cada fase se implementará y verificará antes de continuar con la siguiente. Se priorizan cambios pequeños, trazables y reversibles.