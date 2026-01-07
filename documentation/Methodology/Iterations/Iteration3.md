## 🟩 Sprint 3 – Sprint Backlog (detalle)

### 🎯 Objetivo del Sprint

> Permitir la gestión de evaluaciones asociadas a cada ramo.

---

## 📋 Historias incluidas

* HU-08 Crear evaluación
* HU-09 Editar evaluación
* HU-10 Eliminar evaluación
* HU-11 Listar evaluaciones

---

## 🛠 Sprint Backlog (tareas técnicas)

### Backend (.NET)

1. Crear entidad `Evaluation`
2. Relación `Course` – `Evaluation`
3. Configurar migración EF
4. Endpoint `POST /evaluations`
5. Endpoint `GET /courses/{id}/evaluations`
6. Endpoint `PUT /evaluations/{id}`
7. Endpoint `DELETE /evaluations/{id}`
8. Validar suma de porcentajes ≤ 100%
9. Manejo de errores

### Frontend (Next.js)

10. Vista de evaluaciones por ramo
11. Formulario crear evaluación
12. Formulario editar evaluación
13. Tabla/listado de evaluaciones
14. Validaciones de porcentaje
15. Feedback visual al usuario

### General

16. Pruebas de consistencia
17. Commit y push del Sprint

---

## ✅ Definition of Done (Sprint 3)

* Evaluaciones asociadas correctamente a ramos
* Validación de porcentajes correcta
* CRUD completo funcional
* UI clara y usable
* Incremento funcional entregado

---

## 🗓 Organización diaria sugerida

* **Día 1:** Modelo y migraciones
* **Día 2:** Backend evaluaciones
* **Día 3:** UI evaluaciones
* **Día 4:** Integración
* **Día 5:** Ajustes finales
