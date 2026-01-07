# 📘 Historias de Usuario

**Plataforma de Autogestión Académica**

---

## 🔐 Autenticación y Usuario

### HU-01 Registro de usuario

**Como** estudiante
**Quiero** registrarme ingresando mi información académica básica
**Para** poder usar la plataforma de autogestión.

**Criterios de aceptación**

* Se solicita nombre, email, contraseña y datos académicos mínimos
* El email debe ser único
* La contraseña se almacena en forma segura
* El usuario queda registrado en la base de datos

---

### HU-02 Inicio de sesión

**Como** estudiante
**Quiero** iniciar sesión con mis credenciales
**Para** acceder a mi información académica.

**Criterios de aceptación**

* Validación de credenciales
* Retorno de JWT válido
* Manejo de credenciales incorrectas

---

### HU-03 Persistencia de sesión

**Como** estudiante
**Quiero** mantener mi sesión activa
**Para** no tener que iniciar sesión cada vez que ingreso.

**Criterios de aceptación**

* Token almacenado localmente
* Sesión válida entre recargas
* Cierre de sesión manual

---

## 📚 Gestión de Ramos

### HU-04 Crear ramo

**Como** estudiante
**Quiero** registrar un ramo
**Para** llevar control de mis asignaturas.

**Criterios de aceptación**

* El ramo queda asociado al usuario
* Se valida información obligatoria
* Se guarda en la base de datos

---

### HU-05 Editar ramo

**Como** estudiante
**Quiero** modificar un ramo existente
**Para** mantener actualizada mi información.

**Criterios de aceptación**

* Solo puedo editar mis propios ramos
* Los cambios se reflejan correctamente
* Validación de datos

---

### HU-06 Eliminar ramo

**Como** estudiante
**Quiero** eliminar un ramo
**Para** quitar asignaturas que ya no curso.

**Criterios de aceptación**

* Confirmación previa
* Eliminación lógica o física
* No afecta otros ramos

---

### HU-07 Listar ramos

**Como** estudiante
**Quiero** ver todos mis ramos
**Para** tener una visión general de mis asignaturas.

**Criterios de aceptación**

* Solo se muestran ramos del usuario
* Lista clara y ordenada

---

## 📝 Gestión de Evaluaciones

### HU-08 Crear evaluación

**Como** estudiante
**Quiero** agregar evaluaciones a un ramo
**Para** registrar mis notas y porcentajes.

**Criterios de aceptación**

* Evaluación asociada a un ramo
* Porcentaje válido
* Datos guardados correctamente

---

### HU-09 Editar evaluación

**Como** estudiante
**Quiero** editar una evaluación
**Para** corregir información ingresada.

**Criterios de aceptación**

* Solo evaluaciones propias
* Validaciones activas
* Cambios persistidos

---

### HU-10 Eliminar evaluación

**Como** estudiante
**Quiero** eliminar una evaluación
**Para** mantener información actualizada.

**Criterios de aceptación**

* Confirmación previa
* Eliminación correcta

---

### HU-11 Listar evaluaciones

**Como** estudiante
**Quiero** ver las evaluaciones de un ramo
**Para** conocer el estado de mis notas.

**Criterios de aceptación**

* Asociadas al ramo correcto
* Ordenadas claramente

---

## 📊 Cálculos Académicos

### HU-12 Promedio ponderado

**Como** estudiante
**Quiero** ver mi promedio ponderado por ramo
**Para** conocer mi rendimiento académico.

**Criterios de aceptación**

* Cálculo correcto
* Considera porcentajes
* Resultado claro

---

### HU-13 Nota mínima necesaria

**Como** estudiante
**Quiero** saber qué nota necesito
**Para** aprobar un ramo.

**Criterios de aceptación**

* Considera evaluaciones pendientes
* Resultado comprensible

---

### HU-14 Simulación de escenarios

**Como** estudiante
**Quiero** simular distintas notas
**Para** tomar mejores decisiones académicas.

**Criterios de aceptación**

* Entrada flexible
* Resultados en tiempo real

---

## 📈 Dashboard

### HU-15 Dashboard académico

**Como** estudiante
**Quiero** ver un dashboard general
**Para** entender mi situación académica rápidamente.

**Criterios de aceptación**

* Información resumida
* Visualmente clara

---

### HU-16 Estado de ramos

**Como** estudiante
**Quiero** ver el estado de mis ramos
**Para** saber cuáles están aprobados o en riesgo.

**Criterios de aceptación**

* Estados claros
* Actualización automática

---

### HU-17 Resumen académico

**Como** estudiante
**Quiero** ver un resumen global
**Para** evaluar mi progreso general.

**Criterios de aceptación**

* Datos consolidados
* Fácil interpretación

---

## ⚙️ Infraestructura y Calidad

### HU-18 Dockerización

**Como** desarrollador
**Quiero** dockerizar la aplicación
**Para** facilitar el despliegue.

---

### HU-19 Documentación

**Como** desarrollador
**Quiero** documentar el proyecto
**Para** que sea entendible y mantenible.

---

### HU-20 Preparación para despliegue

**Como** desarrollador
**Quiero** dejar el proyecto listo para producción
**Para** presentarlo como proyecto profesional.
