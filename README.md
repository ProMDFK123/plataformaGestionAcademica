# 🎓 Plataforma de Autogestión Académica

![Next.js](https://img.shields.io/badge/Next.js-14-black)
![React](https://img.shields.io/badge/React-18-61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6)
![ASP.NET](https://img.shields.io/badge/ASP.NET_Core-Web_API-512BD4)
![MySQL](https://img.shields.io/badge/MySQL-4479A1)
![Docker](https://img.shields.io/badge/Docker-2496ED)
![License](https://img.shields.io/badge/license-MIT-green)

---

## 📌 Descripción general

La **Plataforma de Autogestión Académica** es una aplicación web donde cada estudiante gestiona de forma **privada y personalizada** su progreso académico.

El sistema permite registrar ramos, evaluaciones y notas, calcular promedios automáticamente y **simular escenarios académicos**, como la **nota mínima necesaria para aprobar** un ramo.

El proyecto sigue un enfoque de **autogestión**, sin depender de sistemas institucionales ni compartir datos entre usuarios.

---

## 🎯 Objetivos del proyecto

* Aplicar un stack moderno de desarrollo web full stack.
* Implementar autenticación segura con JWT.
* Diseñar una arquitectura limpia y escalable.
* Resolver un problema real mediante lógica académica automatizada.
* Utilizar Scrum como marco de trabajo.

---

## 🧩 Funcionalidades principales

### 🔐 Autenticación

* Registro y login con JWT.
* Registro con información académica mínima:

  * Email
  * Contraseña
  * Universidad
  * Carrera
  * Año de ingreso
  * Escala de notas (mínima y máxima)

---

### 📚 Gestión de ramos

* Crear, editar y eliminar ramos.
* Información por ramo:

  * Nombre
  * Créditos
  * Semestre
  * Estado (cursando / aprobado / reprobado)
* Cada usuario gestiona únicamente sus propios ramos.

---

### 📝 Gestión de evaluaciones

* CRUD de evaluaciones por ramo.
* Campos:

  * Nombre
  * Porcentaje
  * Nota (opcional)
* Validaciones:

  * La suma de porcentajes no puede superar el 100%.
  * Las notas deben respetar la escala definida por el usuario.

---

### 📊 Cálculo inteligente y simulaciones

* Promedio ponderado por ramo.
* Promedio general.
* Cálculo automático de la **nota mínima necesaria para aprobar**.
* Simulación de escenarios académicos futuros.

---

### 📈 Dashboard personal

* Créditos cursados vs aprobados.
* Estado de los ramos.
* Visualización clara del progreso académico.
* Interfaz moderna y responsive.

---

## 🏗 Arquitectura del sistema

```text
Frontend
└─ Next.js 14 (React 18 + TypeScript + TailwindCSS)
   └─ Axios (consumo de API REST)

Backend
└─ ASP.NET Core Web API
   └─ Entity Framework Core

Base de Datos
└─ MySQL (MySQL Workbench)

Infraestructura
└─ Docker (Frontend + Backend + DB)
```

---

## 🗃 Modelo de datos

### User

```csharp
User
- Id
- Email
- PasswordHash
- University
- Career
- EntryYear
- MinGrade
- MaxGrade
```

### Course

```csharp
Course
- Id
- Name
- Credits
- Semester
- Status
- UserId
```

### Evaluation

```csharp
Evaluation
- Id
- Name
- Weight
- Grade (nullable)
- CourseId
```

**Relaciones**

* User 1 ── * Course
* Course 1 ── * Evaluation

---

## 🛠 Tecnologías utilizadas

### Frontend

* Next.js 14 (App Router)
* React 18
* TypeScript
* TailwindCSS
* Axios

### Backend

* ASP.NET Core Web API
* Entity Framework Core
* JWT Authentication

### Base de datos

* MySQL (MySQL Workbench)

### DevOps y herramientas

* Docker & Docker Compose
* ESLint / Prettier
* VS Code

---

## 🚀 Instalación y ejecución

### 1️⃣ Clonar el repositorio

```bash
git clone https://github.com/ProMDFK123/plataformaGestionAcademica
```

---

### 2️⃣ Configurar variables de entorno

Archivo `.env` para el backend:

```env
DB_HOST=localhost
DB_PORT=3306
DB_USER=root
DB_PASS=password
DB_NAME=autogestion
JWT_SECRET=clave_secreta_segura
```

---

### 3️⃣ Ejecutar con Docker

```bash
docker-compose up --build
```

---

### 4️⃣ Accesos

* Frontend: `http://localhost:3000`
* Backend API: `http://localhost:5000/api`

---

## 🔐 Seguridad

* Autenticación basada en JWT.
* Todas las operaciones están filtradas por el `UserId` obtenido desde el token.
* No se acepta el `UserId` desde el frontend.
* Contraseñas hasheadas.
* Validaciones estrictas en backend.

---

## 🧭 Roadmap Scrum (resumen)

| Sprint | Objetivo                       |
| ------ | ------------------------------ |
| 1      | Setup, Auth y Registro         |
| 2      | CRUD de Ramos                  |
| 3      | CRUD de Evaluaciones           |
| 4      | Cálculos académicos            |
| 5      | Dashboard y UX                 |
| 6      | Docker, documentación y cierre |

---

## 👤 Autor

**Gabriel López**
Estudiante de Ingeniería Civil en Computación e Informática


¿Seguimos con eso? 🚀
