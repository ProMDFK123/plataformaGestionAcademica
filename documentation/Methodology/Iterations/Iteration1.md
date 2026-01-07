## 🟩 Sprint 1 – Sprint Backlog (detalle)

### 🎯 Objetivo del Sprint

> Permitir que un estudiante se registre e inicie sesión con su información académica mínima.

---

## 📋 Historias incluidas

* HU-01 Registro de usuario
* HU-02 Login con JWT
* HU-03 Persistencia de sesión

---

## 🛠 Sprint Backlog (tareas técnicas)

### Backend (.NET)

1. Crear proyecto ASP.NET Core Web API
2. Configurar conexión a **MySQL** con EF Core
3. Crear entidad `User`
4. Configurar migraciones EF
5. Implementar hash de contraseñas
6. Endpoint `POST /auth/register`
7. Endpoint `POST /auth/login`
8. Generación de JWT
9. Middleware de autenticación

### Frontend (Next.js)

10. Crear proyecto Next.js 14 con TypeScript
11. Configurar TailwindCSS
12. Página `/register`
13. Página `/login`
14. Servicio Axios base
15. Manejo de token (login/logout)

### General

16. Variables de entorno
17. Commit y push del Sprint

---

## ✅ Definition of Done (Sprint 1)

* Usuario puede registrarse
* Usuario puede iniciar sesión
* JWT válido
* Datos guardados en MySQL
* Front y Back conectados
* Sprint demo funcional

---

## 🗓 Organización diaria sugerida

* **Día 1:** Setup backend + DB
* **Día 2:** Auth backend
* **Día 3:** Frontend auth
* **Día 4:** Integración front-back
* **Día 5:** Validaciones y limpieza
