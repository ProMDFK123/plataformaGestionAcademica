# 🟦 Planificación de Iteraciones Scrum

**Plataforma de Autogestión Académica**

---

## ⏱ Duración y ritmo

* **Sprint length:** 1 semana
* **Total sprints:** 6
* **Incremento entregable** al final de cada sprint

---

## 🧱 Visión del Producto (Product Goal)

> Permitir que un estudiante gestione y analice su progreso académico de forma autónoma, segura y personalizada.

---

## 📦 Product Backlog (agrupado por valor)

1. Autenticación y registro académico
2. Gestión de ramos
3. Gestión de evaluaciones
4. Cálculo académico inteligente
5. Dashboard y UX
6. Infraestructura y cierre

---

# 🟩 Sprint 1 – Autenticación y Setup

### 🎯 Objetivo del Sprint

Permitir que un estudiante se registre e inicie sesión con información académica mínima.

---

### 🧩 Historias de Usuario

* **HU-01:** Registro de usuario con datos académicos
* **HU-02:** Login con JWT
* **HU-03:** Persistencia de sesión

---

### 🛠 Tareas técnicas

**Backend**

* Crear proyecto ASP.NET Core Web API
* Configurar EF Core con MySQL
* Entidad `User`
* Hash de contraseñas
* Endpoint `/auth/register`
* Endpoint `/auth/login`
* Generación de JWT

**Frontend**

* Setup Next.js 14
* Formulario de registro (2 pasos)
* Formulario de login
* Manejo de token (localStorage / cookies)

---

### ✅ Entregable

✔ Usuario puede registrarse y loguearse
✔ JWT funcional
✔ Base de datos creada

---

# 🟩 Sprint 2 – Gestión de Ramos

### 🎯 Objetivo del Sprint

Permitir que el estudiante gestione sus ramos.

---

### 🧩 Historias de Usuario

* **HU-04:** Crear ramos
* **HU-05:** Editar ramos
* **HU-06:** Eliminar ramos
* **HU-07:** Listar ramos del usuario

---

### 🛠 Tareas técnicas

**Backend**

* Entidad `Course`
* Endpoints CRUD `/courses`
* Autorización por `UserId`
* Validaciones de datos

**Frontend**

* Página `/courses`
* Formulario crear/editar ramo
* Lista de ramos

---

### ✅ Entregable

✔ CRUD completo de ramos
✔ Datos aislados por usuario

---

# 🟩 Sprint 3 – Gestión de Evaluaciones

### 🎯 Objetivo del Sprint

Registrar evaluaciones y pesos por ramo.

---

### 🧩 Historias de Usuario

* **HU-08:** Crear evaluaciones
* **HU-09:** Editar evaluaciones
* **HU-10:** Eliminar evaluaciones
* **HU-11:** Listar evaluaciones por ramo

---

### 🛠 Tareas técnicas

**Backend**

* Entidad `Evaluation`
* Endpoints `/courses/{id}/evaluations`
* Validación suma de porcentajes ≤ 100

**Frontend**

* Página `/courses/[id]`
* Formulario de evaluaciones
* Tabla de evaluaciones

---

### ✅ Entregable

✔ Evaluaciones asociadas a ramos
✔ Validaciones académicas funcionando

---

# 🟩 Sprint 4 – Cálculo Académico Inteligente

### 🎯 Objetivo del Sprint

Agregar valor mediante cálculos automáticos.

---

### 🧩 Historias de Usuario

* **HU-12:** Promedio ponderado por ramo
* **HU-13:** Nota mínima necesaria para aprobar
* **HU-14:** Simulación de escenarios

---

### 🛠 Tareas técnicas

**Backend**

* Servicio de cálculo académico
* Endpoints de cálculo
* Tests de lógica (opcional pero recomendado)

**Frontend**

* Mostrar promedio por ramo
* Inputs para simulación
* Resultados en tiempo real

---

### ✅ Entregable

✔ Cálculos confiables
✔ Simulación usable

---

# 🟩 Sprint 5 – Dashboard y UX

### 🎯 Objetivo del Sprint

Visualizar claramente el progreso académico.

---

### 🧩 Historias de Usuario

* **HU-15:** Dashboard general
* **HU-16:** Resumen de créditos y estados

---

### 🛠 Tareas técnicas

**Frontend**

* Página `/dashboard`
* Gráficos básicos
* Mejoras visuales con Tailwind

**Backend**

* Endpoint de resumen académico

---

### ✅ Entregable

✔ Dashboard funcional
✔ UX clara y consistente

---

# 🟩 Sprint 6 – Infraestructura y Cierre

### 🎯 Objetivo del Sprint

Dejar el proyecto listo para entrega y portafolio.

---

### 🧩 Historias de Usuario

* **HU-17:** Dockerización completa
* **HU-18:** Documentación final

---

### 🛠 Tareas técnicas

* `docker-compose.yml` con MySQL
* Variables de entorno
* README final
* Screenshots
* Limpieza de código

---

### ✅ Entregable final

✔ Proyecto ejecutable con Docker
✔ Documentación profesional
✔ Listo para portafolio

---

## 🧠 Definition of Done (global)

* Funcionalidad implementada
* Validaciones completas
* Seguridad aplicada
* Código formateado
* Commit realizado
* Incremento ejecutable
