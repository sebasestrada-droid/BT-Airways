# ✈️ Modelo Entidad-Relación — Línea Aérea

<p align="center">
  <strong>Proyecto de Modelamiento de Bases de Datos</strong><br>
  Duoc UC
</p>

---

## 📌 Sobre el proyecto

Este proyecto presenta el diseño de un **Modelo Entidad-Relación (MER)** para una línea aérea.

El modelo permite representar y relacionar información sobre:

- ✈️ Aviones
- 🛫 Vuelos
- 👨‍💼 Empleados
- 👨‍✈️ Pilotos
- 🧑‍💼 Administrativos
- 👤 Pasajeros
- 📋 Reservas
- 🧳 Equipaje

---

## 🔗 Relaciones entre entidades

Las principales relaciones representadas en el modelo son:

| Entidades | Relación |
|---|---|
| **Avión — Vuelo** | Un avión puede realizar uno o varios vuelos. |
| **Empleado — Piloto** | Un empleado puede corresponder a un piloto. |
| **Empleado — Administrativo** | Un empleado puede corresponder a un administrativo. |
| **Vuelo — Reserva** | Un vuelo puede tener una o varias reservas. |
| **Pasajero — Reserva** | Un pasajero puede realizar una o varias reservas. |
| **Pasajero — Equipaje** | Un pasajero puede tener uno o varios equipajes. |
| **Empleado — Reserva** | Un empleado puede gestionar una o varias reservas. |

Las relaciones se representan mediante **claves foráneas y cardinalidades** dentro del modelo.

---

## 🛠️ Herramienta utilizada

**Oracle SQL Data Modeler**

---

## 📐 Modelo Entidad-Relación
<img width="1600" height="1208" alt="WhatsApp Image 2026-08-21 at 12 01 35" src="https://github.com/user-attachments/assets/5c2805bf-702a-42f0-9038-2089f4941b4b" />

---

## 🔑 Elementos principales

- **PK:** Claves primarias para identificar registros.
- **FK:** Claves foráneas para establecer relaciones.
- **Cardinalidad:** Define la cantidad de elementos que pueden relacionarse.
- **Atributos:** Representan las características de cada entidad.
- **Tipos de datos:** Definen el formato de la información almacenada.

---


**Duoc UC — Modelamiento de Bases de Datos**
