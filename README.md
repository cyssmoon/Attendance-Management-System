# 📋 Sistema de Gestión de Asistencias

> Aplicación web para registrar y consultar asistencias de alumnos por curso y materia.

-----

## 📁 Estructura

```
tp/
├── server.js
├── bd.sql
└── public/
    ├── index.html
    ├── style.css
    └── main.js
```

-----

## ✨ Funcionalidades

- 👤 Crear alumnos y asignarlos a un curso
- ✅ Registrar asistencia por alumno, materia y tipo
- 🔍 Consultar asistencias filtrando por curso, materia y fecha
- ✏️ Editar registros existentes
- 🗑️ Eliminar registros con confirmación

-----

## 🗄️ Base de datos

Tablas: `cursos`, `alumnos`, `materias`, `registros`

Tipos de asistencia: `A` (ausente) · `P` (presente) · `T` (tarde) · `RA` (retiro anticipado) · `AP` (ausente con permiso)

-----

## 🌐 Endpoints API

|Método|Ruta                |Descripción          |
|------|--------------------|---------------------|
|GET   |`/cursos`           |Listar cursos        |
|GET   |`/materias/:cursoId`|Materias de un curso |
|GET   |`/alumnos/:cursoId` |Alumnos de un curso  |
|POST  |`/alumnos`          |Crear alumno         |
|POST  |`/asistencias`      |Registrar asistencia |
|GET   |`/asistencias`      |Consultar asistencias|
|PUT   |`/asistencias/:id`  |Editar asistencia    |
|DELETE|`/asistencias/:id`  |Eliminar asistencia  |

-----

## 🚀 Cómo correrlo

```bash
# 1. Importar la base de datos
mysql -u root -p < bd.sql

# 2. Instalar dependencias
npm install

# 3. Iniciar el servidor
node server.js
```

Abrí `http://localhost:3000` en el navegador.

-----

## 🛠️ Stack

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat&logo=express&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)

-----

## 👩‍💻 Autora

**Luna Estanga** 