# 🐞 Bug Reports — E-commerce Web Application

## 📌 Información general

| Campo | Información |
|---|---|
| Proyecto | E-commerce Web Application |
| QA | Irving Quezada |
| Tipo de pruebas | Functional Testing |
| Ambiente | QA / Test |
| Gestión | Jira (simulado) |

---

# BUG-001 — El sistema permite continuar el checkout sin seleccionar método de pago

## 📋 Información del defecto

| Campo | Detalle |
|---|---|
| ID | BUG-001 |
| Módulo | Checkout |
| Severidad | Alta |
| Prioridad | Alta |
| Tipo | Funcional |
| Estado | Abierto |
| Ambiente | QA |
| Detectado por | Irving Quezada |

---

## 📝 Descripción

El sistema permite al usuario continuar con el proceso de
checkout sin seleccionar un método de pago.

El comportamiento esperado es que el sistema valide que
exista un método de pago seleccionado antes de permitir
continuar con la compra.

---

## 🔄 Precondiciones

- Usuario autenticado.
- Existe al menos un producto disponible.
- El producto fue agregado al carrito.
- El usuario se encuentra en el proceso de checkout.

---

## 🧪 Pasos para reproducir

1. Iniciar sesión con un usuario válido.
2. Seleccionar un producto disponible.
3. Agregar el producto al carrito.
4. Acceder al carrito.
5. Seleccionar "Checkout".
6. Completar la información de envío.
7. No seleccionar ningún método de pago.
8. Seleccionar "Continuar" o "Confirmar compra".

---

## ❌ Resultado actual

El sistema permite continuar con el proceso de compra sin
tener un método de pago seleccionado.

---

## ✅ Resultado esperado

El sistema debe impedir continuar con la compra y mostrar un
mensaje indicando que es necesario seleccionar un método de
pago.

---

## ⚠️ Impacto

El defecto puede permitir que una orden avance a un estado
inconsistente o incompleto.

Esto puede afectar el proceso de compra y generar problemas
en procesos posteriores relacionados con el pedido.

---

## 📊 Severidad vs Prioridad

**Severidad:** Alta

El defecto afecta una funcionalidad importante del proceso
de compra.

**Prioridad:** Alta

Debe ser corregido antes de liberar la funcionalidad a
producción.

---

## 📎 Evidencia

La evidencia de ejecución será agregada en la carpeta:

```text
evidence/


BUG-002 — Mensaje incorrecto al ingresar credenciales inválidas
📋 Información del defecto
Campo	Detalle
ID	BUG-002
Módulo	Login
Severidad	Media
Prioridad	Media
Tipo	Funcional
Estado	Abierto
Ambiente	QA
Detectado por	Irving Quezada
📝 Descripción

Cuando el usuario intenta iniciar sesión con credenciales
incorrectas, el sistema muestra un mensaje que no corresponde
con la situación presentada.

🔄 Precondiciones
Usuario registrado.
Aplicación disponible.
Usuario ubicado en la pantalla de Login.
🧪 Pasos para reproducir
Acceder a la pantalla de Login.
Introducir un usuario válido.
Introducir una contraseña incorrecta.
Seleccionar "Iniciar sesión".
❌ Resultado actual

El sistema muestra un mensaje incorrecto o poco claro para
el usuario.

✅ Resultado esperado

El sistema debe mostrar un mensaje claro indicando que las
credenciales proporcionadas no son válidas.

📊 Severidad

Media

La funcionalidad de autenticación continúa operando, pero
el mensaje afecta la experiencia y comprensión del usuario.

📊 Resumen de defectos
ID	Módulo	Severidad	Prioridad	Estado
BUG-001	Checkout	Alta	Alta	🔴 Abierto
BUG-002	Login	Media	Media	🟠 Abierto
🧠 Información documentada

Cada defecto contiene:

Identificador
Módulo afectado
Descripción
Precondiciones
Pasos para reproducir
Resultado actual
Resultado esperado
Severidad
Prioridad
Impacto
Evidencia
Estado
