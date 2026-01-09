# 🧪 Plan de Testing

**Plataforma de Autogestión Académica**

---

## 1️⃣ Objetivo del Testing

El objetivo del proceso de testing es verificar que la plataforma funcione correctamente, cumpla con los requisitos definidos en las historias de usuario y entregue un incremento estable al final de cada sprint.

---

## 2️⃣ Alcance del Testing

El testing cubrirá:

* Funcionalidades principales del sistema
* Validaciones de datos
* Integración Frontend – Backend
* Persistencia de información en la base de datos
* Manejo de errores y casos inválidos

No se contempla testing de carga ni estrés debido al alcance académico del proyecto.

---

## 3️⃣ Tipos de Testing

### 🔹 Testing Funcional

Verifica que cada funcionalidad cumpla con lo esperado según las historias de usuario.

### 🔹 Testing de Integración

Valida la correcta comunicación entre:

* Frontend (Next.js)
* Backend (.NET)
* Base de datos (MySQL)

### 🔹 Testing de Validación

Comprueba:

* Campos obligatorios
* Formatos correctos
* Restricciones de negocio (porcentajes, permisos, etc.)

### 🔹 Testing Manual

Las pruebas se realizarán de forma manual mediante interacción directa con la aplicación y herramientas como Postman.

---

## 4️⃣ Ambiente de Pruebas

| Elemento      | Descripción            |
| ------------- | ---------------------- |
| Frontend      | Next.js 14             |
| Backend       | ASP.NET Core Web API   |
| Base de datos | MySQL                  |
| Herramientas  | Postman, Navegador Web |
| Entorno       | Desarrollo local       |

---

## 5️⃣ Estrategia de Testing por Sprint

Al finalizar cada sprint se ejecutan pruebas sobre:

* Las historias desarrolladas en el sprint actual
* Las funcionalidades críticas de sprints anteriores (regresión básica)

Cada sprint debe entregar un incremento **probado y funcional**.

---

## 6️⃣ Plantilla de Casos de Prueba

### 📋 Caso de Prueba – CP-XX

| Campo              | Descripción                                 |
| ------------------ | ------------------------------------------- |
| ID                 | CP-01                                       |
| Historia asociada  | HU-01 Registro de usuario                   |
| Módulo             | Autenticación                               |
| Precondición       | Usuario no registrado                       |
| Datos de entrada   | Nombre, email, contraseña                   |
| Pasos              | 1. Ingresar datos <br> 2. Enviar formulario |
| Resultado esperado | Usuario registrado correctamente            |
| Resultado obtenido | —                                           |
| Estado             | Pendiente / Aprobado / Fallido              |
| Observaciones      | —                                           |

---

## 7️⃣ Criterios de Aceptación de Pruebas

Una historia de usuario se considera **aprobada** cuando:

* Todos sus casos de prueba están en estado **Aprobado**
* No existen errores críticos
* La funcionalidad es usable desde el frontend

---

## 8️⃣ Gestión de Errores

Los errores detectados se documentan indicando:

* Historia afectada
* Descripción del error
* Pasos para reproducirlo
* Prioridad (Alta / Media / Baja)

Los errores críticos deben resolverse dentro del sprint.

---

## 9️⃣ Evidencia de Testing

Como evidencia del proceso de testing se pueden incluir:

* Capturas de pantalla
* Registros de pruebas manuales
* Resultados de pruebas en Postman

---

## 🔟 Cierre de Testing

El proceso de testing finaliza cuando:

* Todos los sprints han sido probados
* No existen errores críticos pendientes
* El sistema cumple con los objetivos del proyecto
