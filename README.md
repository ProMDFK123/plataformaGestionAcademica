# 📚 Plataforma de Autogestión Académica
## 🔹 Descripción
Esta aplicación web permite a estudiantes gestionar su propia información académica de forma privada y personalizada.
Cada usuario puede:
- Registrar sus ramos y evaluaciones.
- Calcular automáticamente el promedio ponderado de cada ramo.
- Simular escenarios para conocer la nota mínima necesaria para aprobar.
- Visualizar su progreso académico en dashboards claros y dinámicos.

El proyecto está pensado como herramienta de autogestión, sin depender de sistemas institucionales, lo que lo hace seguro y ético para uso personal.

## 🔹 Tecnologías utilizadas
### Frontend
- Next.js 14 (App Router)
- React 18
- TypeScript
- TailwindCSS
- Axios
### Backend
- ASP.NET Core Web API
- Entity Framework Core
- MySQL Workbench
- JWT para autenticación
### Herramientas
- Docker (Frontend, Backend, DB)
- VS Code
- ESLint / Prettier

## 🔹 Características principales
### 1️⃣ Registro y autenticación
- Registro con información académica mínima:
  - Email
  - Contraseña
  - Universidad
  - Carrera
  - Año de ingreso
  - Escala de notas (min/max)
- Login y Logout seguro con JWT.
- Validaciones estrictas de datos.
### 2️⃣ Gestión de ramos
- Crear, editar y eliminar ramos.
- Campos: nombre, créditos, semestre, estado (cursando/aprobado/reprobado).
- Cada estudiante gestiona únicamente sus propios ramos.
### 3️⃣ Gestión de evaluaciones
- CRUD de evaluaciones dentro de cada ramo.
- Campos: nombre, porcentaje, nota, fecha.
- Validaciones: suma de porcentajes ≤ 100, notas dentro de escala definida.
### 4️⃣ Dashboard y simulaciones
- Promedio por ramo y promedio general.
- Créditos cursados vs aprobados.
- Nota mínima necesaria para aprobar cada ramo.
- Simulaciones de escenarios de notas futuras.
- Visualización clara y moderna con TailwindCSS.

## 🔹 Modelo de datos
### User
```
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
```
Course
- Id
- Name
- Credits
- Semester
- Status
- UserId
```
### Evaluation
```
Evaluation
- Id
- Name
- Weight
- Grade (nullable)
- CourseId
```
### Relaciones
- User 1 ── * Course
- Course 1 ── * Evaluation

## 🔹 Arquitectura
```text
Frontend (Next.js 14)
  │
  ├─ Axios → consume API
  │
Backend (ASP.NET Core Web API)
  │
  └─ Entity Framework Core → PostgreSQL
```
### Docker
- Contenedor frontend
- Contenedor backend
- Contenedor DB (MySQL)

