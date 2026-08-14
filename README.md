# ✈️ BT Airways

## 📌 Descripción

BT Airways es un proyecto de modelamiento de una base de datos para una aerolínea.

El proyecto permite organizar la información de pasajeros, empleados, vuelos y reservas, estableciendo las relaciones entre ellos.

## 🎯 Objetivo

Diseñar una base de datos organizada para gestionar la información principal de una aerolínea.

## 🗂️ Entidades

### PASAJERO

- num_pasaporte (PK)
- nombre_completo
- fecha_nacimiento
- nacionalidad
- telefono_correo

### EMPLEADO

- rut (PK)
- nombre_completo
- direccion
- sueldo_base
- fecha_ingreso
- genero
- telefono_movil
- telefono_contacto

### VUELO

- num_vuelo (PK)
- fecha_salida
- fecha_llegada
- hora_salida

### RESERVA

- num_reserva (PK)
- fecha_reserva
- fecha_viaje
- estado
- num_pasaporte (FK)
- rut (FK)
- num_vuelo (FK)

## 🔗 Relaciones

La tabla RESERVA se relaciona con:

- PASAJERO mediante num_pasaporte.
- EMPLEADO mediante rut.
- VUELO mediante num_vuelo.



Proyecto académico — BT Airways
