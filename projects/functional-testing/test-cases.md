# 🧪 Test Cases — E-commerce Web Application

## 📌 Información general

| Campo | Información |
|---|---|
| Proyecto | E-commerce Web Application |
| Tipo de pruebas | Functional Testing |
| Plataforma | Web |
| QA | Irving Quezada |
| Estado | En ejecución |

---

## 📋 Casos de prueba

### TC-001 — Login exitoso

| Campo | Detalle |
|---|---|
| Prioridad | Alta |
| Tipo | Funcional / Positivo |
| Precondición | Usuario registrado y activo |
| Datos | Usuario y contraseña válidos |

**Pasos:**

1. Acceder a la pantalla de Login.
2. Ingresar usuario válido.
3. Ingresar contraseña válida.
4. Seleccionar "Iniciar sesión".

**Resultado esperado:**

El sistema debe autenticar al usuario y mostrar la página
principal de la aplicación.

Actual Result: El usuario pudo iniciar sesión correctamente y se mostró la sesión activa.
Status: ✅ PASS

### Evidencia

![TC-001 - Login exitoso](./evidence/TC-001.png)

---

### TC-002 — Login con contraseña incorrecta

| Campo | Detalle |
|---|---|
| Prioridad | Alta |
| Tipo | Funcional / Negativo |
| Precondición | Usuario registrado |
| Datos | Usuario válido + contraseña incorrecta |

**Pasos:**

1. Acceder a Login.
2. Ingresar usuario válido.
3. Ingresar una contraseña incorrecta.
4. Seleccionar "Iniciar sesión".

**Resultado esperado:**

El sistema debe rechazar el acceso y mostrar un mensaje
indicando que las credenciales no son válidas.

**Resultado obtenido:** Pendiente

**Estado:** ⏳ Not Run

---

### TC-003 — Login con campos vacíos

| Campo | Detalle |
|---|---|
| Prioridad | Alta |
| Tipo | Validación / Negativo |
| Precondición | Ninguna |
| Datos | Campos vacíos |

**Pasos:**

1. Acceder a Login.
2. Dejar usuario vacío.
3. Dejar contraseña vacía.
4. Seleccionar "Iniciar sesión".

**Resultado esperado:**

El sistema debe solicitar el ingreso de los campos obligatorios
y no permitir el inicio de sesión.

**Resultado obtenido:** Pendiente

**Estado:** ⏳ Not Run

---

### TC-004 — Búsqueda de producto existente

| Campo | Detalle |
|---|---|
| Prioridad | Alta |
| Tipo | Funcional / Positivo |
| Precondición | Aplicación disponible |
| Datos | Nombre de producto existente |

**Pasos:**

1. Acceder al catálogo.
2. Introducir el nombre de un producto existente.
3. Ejecutar la búsqueda.

**Resultado esperado:**

El sistema debe mostrar los productos que coincidan con el
criterio de búsqueda.

**Resultado obtenido:** Pendiente

**Estado:** ⏳ Not Run

---

### TC-005 — Búsqueda de producto inexistente

| Campo | Detalle |
|---|---|
| Prioridad | Media |
| Tipo | Funcional / Negativo |
| Precondición | Aplicación disponible |
| Datos | Producto inexistente |

**Pasos:**

1. Acceder al catálogo.
2. Introducir un producto que no exista.
3. Ejecutar la búsqueda.

**Resultado esperado:**

El sistema debe informar que no existen resultados para el
criterio utilizado.

**Resultado obtenido:** Pendiente

**Estado:** ⏳ Not Run

---

### TC-006 — Agregar producto al carrito

| Campo | Detalle |
|---|---|
| Prioridad | Alta |
| Tipo | Funcional / Positivo |
| Precondición | Producto disponible |
| Datos | Producto existente |

**Pasos:**

1. Seleccionar un producto.
2. Acceder al detalle del producto.
3. Seleccionar "Agregar al carrito".
4. Acceder al carrito.

**Resultado esperado:**

El producto debe aparecer en el carrito con la cantidad y
precio correspondientes.

**Resultado obtenido:** Pendiente

**Estado:** ⏳ Not Run

---

### TC-007 — Eliminar producto del carrito

| Campo | Detalle |
|---|---|
| Prioridad | Alta |
| Tipo | Funcional |
| Precondición | Debe existir un producto en el carrito |

**Pasos:**

1. Acceder al carrito.
2. Seleccionar la opción para eliminar el producto.
3. Confirmar la eliminación si aplica.

**Resultado esperado:**

El producto debe eliminarse correctamente del carrito y el
total debe actualizarse.

**Resultado obtenido:** Pendiente

**Estado:** ⏳ Not Run

---

### TC-008 — Actualizar cantidad del producto

| Campo | Detalle |
|---|---|
| Prioridad | Media |
| Tipo | Funcional |
| Precondición | Producto agregado al carrito |

**Pasos:**

1. Acceder al carrito.
2. Modificar la cantidad del producto.
3. Actualizar el carrito.

**Resultado esperado:**

La cantidad debe actualizarse correctamente y el subtotal y
total deben recalcularse.

**Resultado obtenido:** Pendiente

**Estado:** ⏳ Not Run

---

### TC-009 — Checkout con información válida

| Campo | Detalle |
|---|---|
| Prioridad | Crítica |
| Tipo | End-to-End / Positivo |
| Precondición | Producto disponible en carrito |
| Datos | Información válida de envío y pago |

**Pasos:**

1. Acceder al carrito.
2. Seleccionar "Checkout".
3. Ingresar información de envío.
4. Ingresar información requerida para el pago.
5. Confirmar la compra.

**Resultado esperado:**

La compra debe procesarse correctamente y el sistema debe
mostrar la confirmación del pedido.

**Resultado obtenido:** Pendiente

**Estado:** ⏳ Not Run

---

### TC-010 — Checkout con campos obligatorios vacíos

| Campo | Detalle |
|---|---|
| Prioridad | Alta |
| Tipo | Validación / Negativo |
| Precondición | Producto disponible en carrito |

**Pasos:**

1. Acceder al checkout.
2. Dejar uno o más campos obligatorios vacíos.
3. Intentar continuar.

**Resultado esperado:**

El sistema debe identificar los campos obligatorios y mostrar
los mensajes de validación correspondientes.

**Resultado obtenido:** Pendiente

**Estado:** ⏳ Not Run

---

### TC-011 — Confirmación de pedido

| Campo | Detalle |
|---|---|
| Prioridad | Crítica |
| Tipo | End-to-End |
| Precondición | Compra completada |

**Pasos:**

1. Completar correctamente el proceso de checkout.
2. Confirmar la compra.

**Resultado esperado:**

El sistema debe mostrar un número o identificador de pedido
y la información correspondiente a la compra.

**Resultado obtenido:** Pendiente

**Estado:** ⏳ Not Run

---

### TC-012 — Logout

| Campo | Detalle |
|---|---|
| Prioridad | Media |
| Tipo | Funcional |
| Precondición | Usuario autenticado |

**Pasos:**

1. Acceder al menú del usuario.
2. Seleccionar "Cerrar sesión".

**Resultado esperado:**

El usuario debe cerrar sesión y regresar a la pantalla de
acceso o página pública.

**Resultado obtenido:** Pendiente

**Estado:** ⏳ Not Run

---

# 📊 Resumen de casos

| ID | Escenario | Prioridad | Tipo | Estado |
|---|---|---|---|---|
| TC-001 | Login exitoso | Alta | Positivo | ⏳ |
| TC-002 | Login contraseña incorrecta | Alta | Negativo | ⏳ |
| TC-003 | Login campos vacíos | Alta | Validación | ⏳ |
| TC-004 | Búsqueda producto existente | Alta | Positivo | ⏳ |
| TC-005 | Búsqueda producto inexistente | Media | Negativo | ⏳ |
| TC-006 | Agregar producto | Alta | Positivo | ⏳ |
| TC-007 | Eliminar producto | Alta | Funcional | ⏳ |
| TC-008 | Actualizar cantidad | Media | Funcional | ⏳ |
| TC-009 | Checkout válido | Crítica | E2E | ⏳ |
| TC-010 | Checkout inválido | Alta | Negativo | ⏳ |
| TC-011 | Confirmación pedido | Crítica | E2E | ⏳ |
| TC-012 | Logout | Media | Funcional | ⏳ |

---

## 🧠 Técnicas de diseño aplicadas

Los casos fueron diseñados considerando:

- Partición de equivalencias
- Valores límite
- Escenarios positivos
- Escenarios negativos
- Validaciones de campos
- Priorización basada en riesgo
- Flujos End-to-End
- Reglas de negocio
