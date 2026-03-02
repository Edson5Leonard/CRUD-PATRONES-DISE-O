# CRUD-PATRONES-DISE-O
Se va realizar un Crud con 3 patrones de diseño.



# 📊 Base de Datos – Gestión de Empleados

## 📁 Tabla: tipos_empleado

Campos:
- id (INT, PK, AUTO_INCREMENT)
- nombre (CHAR)

Datos iniciales:

1 - Administrativo  
2 - Operativo  
3 - Supervisor  

---

## 📁 Tabla: areas

Campos:
- id (INT, PK, AUTO_INCREMENT)
- nombre (CHAR)

Datos iniciales:

1 - Sistemas  
2 - Recursos Humanos  
3 - Logística  

---

## 📁 Tabla: empleados

Campos:
- id (INT, PK, AUTO_INCREMENT)
- nombre (CHAR)
- email (CHAR, UNIQUE)
- salario (DECIMAL)
- fecha_ingreso (DATE)
- tipo_id (INT, FK)
- area_id (INT, FK)

---

## 🔗 Relaciones

- `empleados.tipo_id` → referencia a `tipos_empleado.id`
- `empleados.area_id` → referencia a `areas.id`

---

## 🧠 Descripción del Modelo

Cada empleado pertenece a:
- Un tipo de empleado
- Un área

La base de datos está diseñada bajo principios de normalización y modelo relacional,
permitiendo escalabilidad y mantenimiento profesional.

