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


/evidence


