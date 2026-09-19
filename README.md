# 🚗 Sistema de Reservas de Autos

Sistema web desarrollado con **Laravel** para la gestión de reservas de vehículos.

El proyecto está desarrollado como trabajo grupal y utiliza **Laravel 13**, **PHP 8.3+**, **PostgreSQL** y **Vite**.

---

## 📋 Tecnologías utilizadas

* **Laravel:** 13.32.0
* **PHP:** 8.3+
* **Base de datos:** PostgreSQL 18
* **Node.js:** 18+
* **NPM**
* **Composer**
* **Vite**
* **Git / GitHub**

---

## 📁 Estructura de ramas

El proyecto utiliza dos ramas principales:

```text
main
└── Versión estable del proyecto

develop
└── Rama principal de desarrollo
```

### Flujo de trabajo

Cada integrante debe crear su propia rama a partir de `develop`.

Ejemplo:

```bash
git checkout develop
git pull origin develop

git checkout -b feature/nombre-de-la-funcionalidad
```

Después de realizar los cambios:

```bash
git add .
git commit -m "Descripción del cambio"
git push origin feature/nombre-de-la-funcionalidad
```

Posteriormente se debe crear un **Pull Request hacia `develop`** para revisar e integrar los cambios.

---

# ⚙️ Instalación del proyecto

## 1. Clonar el repositorio

```bash
git clone https://github.com/Nicks555/sistema-reservas-de-autos.git
```

Ingresar a la carpeta:

```bash
cd sistema-reservas-de-autos
```

---

## 2. Instalar dependencias de PHP

```bash
composer install
```

---

## 3. Instalar dependencias de Node.js

```bash
npm install
```

---

## 4. Configurar el archivo `.env`

Copiar el archivo de configuración:

### Windows

```bash
copy .env.example .env
```

### Linux / macOS

```bash
cp .env.example .env
```

---

## 5. Configurar PostgreSQL

Crear una base de datos llamada:

```text
sistema_reservas
```

En el archivo `.env`, configurar:

```env
DB_CONNECTION=pgsql
DB_HOST=127.0.0.1
DB_PORT=5432
DB_DATABASE=sistema_reservas
DB_USERNAME=postgres
DB_PASSWORD=
```

⚠️ **No subir el archivo `.env` a GitHub.**

Cada integrante debe colocar sus propias credenciales de PostgreSQL en su archivo `.env`.

---

## 6. Generar la clave de Laravel

Ejecutar:

```bash
php artisan key:generate
```

---

## 7. Ejecutar las migraciones

```bash
php artisan migrate
```

Esto creará las tablas necesarias en la base de datos.

---

## 8. Ejecutar el proyecto

En una terminal:

```bash
php artisan serve
```

Laravel estará disponible normalmente en:

```text
http://127.0.0.1:8000
```

En otra terminal ejecutar Vite:

```bash
npm run dev
```

---

# 🔄 Actualizar el proyecto

Antes de comenzar a trabajar, siempre actualizar la rama `develop`:

```bash
git checkout develop
git pull origin develop
```

Después crear la rama correspondiente a la tarea:

```bash
git checkout -b feature/nombre-de-la-tarea
```

---

# 🧑‍💻 Reglas de trabajo del equipo

Para evitar conflictos entre integrantes:

* No trabajar directamente sobre `main`.
* Evitar trabajar directamente sobre `develop` salvo tareas coordinadas.
* Cada funcionalidad debe realizarse en una rama propia.
* Hacer commits pequeños y descriptivos.
* Antes de comenzar una tarea, actualizar `develop`.
* Antes de crear un Pull Request, verificar que el proyecto funcione correctamente.
* Los cambios deben integrarse mediante Pull Request hacia `develop`.
* `main` debe mantenerse como versión estable.

---

# 📝 Ejemplos de nombres de ramas

Para nuevas funcionalidades:

```text
feature/reservas
feature/clientes
feature/vehiculos
feature/pagos
```

Para correcciones:

```text
fix/error-reservas
fix/error-login
fix/error-validacion
```

---

# 💾 Ejemplos de commits

Se recomienda utilizar mensajes claros:

```bash
git commit -m "Agregar CRUD de vehículos"
```

```bash
git commit -m "Implementar módulo de reservas"
```

```bash
git commit -m "Corregir validación de clientes"
```

---

# 🔐 Información importante

Los siguientes archivos y datos **no deben subirse al repositorio**:

```text
.env
/vendor
/node_modules
```

Las credenciales de la base de datos son personales y cada integrante debe configurar su propio archivo `.env`.

---

# 👥 Trabajo colaborativo

Repositorio oficial:

**Sistema de Reservas de Autos**

```text
https://github.com/Nicks555/sistema-reservas-de-autos
```

Los integrantes del equipo deben ser agregados como colaboradores del repositorio de GitHub.

---

# 📌 Estado del proyecto

Actualmente el proyecto se encuentra en etapa de desarrollo.

**Rama principal de desarrollo:**

```text
develop
```

**Rama estable:**

```text
main
```
