# ✈️ BT Airways — Modelo de Base de Datos

![Oracle](https://img.shields.io/badge/Oracle-Database-red)
![SQL](https://img.shields.io/badge/SQL-Database-blue)
![Data%20Modeler](https://img.shields.io/badge/Oracle%20SQL%20Developer%20Data%20Modeler-orange)
![Status](https://img.shields.io/badge/Estado-Completado-success)

## 📌 Descripción

**BT Airways** es un proyecto académico de diseño de una base de datos para una compañía aérea.

El modelo fue desarrollado utilizando **Oracle SQL Developer Data Modeler**, permitiendo representar y organizar la información relacionada con pasajeros, empleados, vuelos y reservas.

El proyecto contempla un **modelo lógico** y un **modelo relacional**, incorporando claves primarias, claves foráneas y relaciones entre las distintas entidades.

---

## 🎯 Objetivo del proyecto

El objetivo es diseñar una estructura de base de datos que permita gestionar de manera organizada la información principal de una aerolínea.

El modelo permite representar:

- 👤 Pasajeros.
- 👨‍💼 Empleados.
- ✈️ Vuelos.
- 🎫 Reservas.
- 🔑 Claves primarias.
- 🔗 Claves foráneas.
- 📊 Relaciones entre las entidades.

---

# 🗂️ Modelo de datos

El sistema está compuesto por cuatro entidades principales:

```text
                    ┌───────────────┐
                    │   PASAJERO    │
                    │───────────────│
                    │ num_pasaporte │
                    │ nombre        │
                    │ fecha_nac.    │
                    │ nacionalidad  │
                    │ teléfono      │
                    └───────┬───────┘
                            │
                            │
                            ▼
                    ┌───────────────┐
                    │    RESERVA    │
                    │───────────────│
                    │ num_reserva   │
                    │ fecha_reserva │
                    │ fecha_viaje   │
                    │ estado        │
                    │ num_pasaporte │
                    │ rut           │
                    │ num_vuelo     │
                    └───────┬───────┘
                            ▲
                            │
              ┌─────────────┴─────────────┐
              │                           │
              │                           │
      ┌───────┴────────┐          ┌───────┴───────┐
      │    EMPLEADO    │          │     VUELO     │
      │────────────────│          │───────────────│
      │ rut            │          │ num_vuelo     │
      │ nombre         │          │ fecha_salida  │
      │ dirección      │          │ fecha_llegada │
      │ sueldo_base    │          │ hora_salida   │
      │ fecha_ingreso  │          └───────────────┘
      │ género         │
      │ teléfono móvil │
      │ teléfono       │
      └────────────────┘
