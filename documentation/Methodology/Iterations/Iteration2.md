## 🟩 Sprint 2 – Sprint Backlog (detalle)

### 🎯 Objetivo del Sprint

> Permitir que el estudiante gestione sus ramos de manera autónoma.

---

## 📋 Historias incluidas

* HU-04 Crear ramo
* HU-05 Editar ramo
* HU-06 Eliminar ramo
* HU-07 Listar ramos

---

## 🛠 Sprint Backlog (tareas técnicas)

### Backend (.NET)

1. Crear entidad `Course`
2. Relación `User` – `Course`
3. Configurar migración EF
4. Endpoint `POST /courses`
5. Endpoint `GET /courses`
6. Endpoint `PUT /courses/{id}`
7. Endpoint `DELETE /courses/{id}`
8. Validar pertenencia del ramo al usuario
9. Manejo de errores y respuestas HTTP

### Frontend (Next.js)

10. Página `/courses`
11. Formulario crear ramo
12. Formulario editar ramo
13. Listado de ramos
14. Eliminación con confirmación
15. Manejo de estados de carga y error

### General

16. Pruebas manuales CRUD
17. Commit y push del Sprint

---

## ✅ Definition of Done (Sprint 2)

* Usuario puede crear, editar y eliminar ramos
* Solo ve sus propios ramos
* Datos persistidos en MySQL
* UI funcional y usable
* Incremento funcional entregado

---

## 🗓 Organización diaria sugerida

* **Día 1:** Modelo y migraciones
* **Día 2:** Endpoints backend
* **Día 3:** UI de ramos
* **Día 4:** Integración
* **Día 5:** Validaciones y limpieza