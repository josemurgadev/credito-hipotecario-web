# Crédito Hipotecario · Web

Frontend de una aplicación de crédito hipotecario: inicio de sesión, menú según el tipo de usuario y gestión del perfil (datos personales y cambio de contraseña).
Consume la API de [credito-hipotecario-api](https://github.com/Jmurga16/credito-hipotecario-api) (.NET 6 con Clean Architecture).

Proyecto de práctica (2023).

## Stack

- **Angular 13** con módulos y rutas con *lazy loading*
- **Angular Material**
- **TypeScript** · **RxJS**

## Qué incluye

- **Autenticación**: login, *guard* de rutas e *interceptor* HTTP para las cabeceras comunes.
- **Layout** con menú de navegación cargado desde la API según el tipo de usuario.
- **Perfil**: datos personales y cambio de contraseña.

## Estructura

```
src/app/
├── core/       # Layout, menú, guard, interceptor, modelos y servicios base
├── modules/
│   ├── auth/   # Login
│   ├── home/   # Inicio
│   └── perfil/ # Datos personales y cambio de contraseña
└── shared/     # Módulo compartido (Angular Material)
```

## Ejecutar en local

Requiere Node.js 16 y la API corriendo.

```bash
git clone https://github.com/Jmurga16/credito-hipotecario-web.git
cd credito-hipotecario-web
npm install
npm start
```

La URL de la API se configura en `src/environments/`.

---

Desarrollado por **José Murga** · [josemurga.dev](https://josemurga.dev)
