# 🏋️‍♂️ Frontend Gym – Angular

Este proyecto corresponde al **frontend** de una aplicación de gestión para un gimnasio, desarrollada con **Angular** y pensada para integrarse con un backend en **Spring Boot** mediante **JWT**.

El objetivo del proyecto es mantener una **estructura profesional, escalable y fácil de mantener**, siguiendo buenas prácticas usadas en proyectos reales.

---

## 📁 Estructura general del proyecto

```text
frontend-gym/
├── src/
│   ├── app/
│   ├── assets/
│   ├── environments/
│   ├── styles.scss
│   └── index.html
├── angular.json
├── package.json
├── tsconfig.json
└── README.md
```

---

## 📂 src/app

Aquí vive **toda la lógica de la aplicación Angular**.

```text
app/
├── auth/
├── core/
├── shared/
├── app-routing.module.ts
├── app.component.ts
└── app.module.ts
```

---

## 🔐 auth/

Módulo encargado de **autenticación y autorización**.
Actualmente contiene el **login**, y a futuro puede incluir:

* Registro
* Recuperación de contraseña

```text
auth/
├── login/
│   ├── login.component.ts
│   ├── login.component.html
│   ├── login.component.scss
│   └── login.component.spec.ts
├── auth-routing.module.ts
└── auth.module.ts
```

### 📌 ¿Qué va aquí?

* Pantallas relacionadas con autenticación
* Formularios de acceso
* Flujo de login/logout

---

## 🧠 core/

Contiene **servicios y configuraciones centrales** que se usan en toda la aplicación.

```text
core/
├── services/
│   └── auth.service.ts
├── guards/
│   └── auth.guard.ts
├── interceptors/
│   └── auth.interceptor.ts
└── core.module.ts
```

### 📌 ¿Para qué sirve core?

* Comunicación con el backend (HTTP)
* Protección de rutas
* Manejo del token JWT
* Funcionalidades globales

⚠️ Nada visual va aquí.

---

## ♻️ shared/

Componentes, modelos y utilidades **reutilizables**.

```text
shared/
├── components/
│   ├── button/
│   └── input/
├── models/
│   └── user.model.ts
└── shared.module.ts
```

### 📌 ¿Qué va aquí?

* Componentes genéricos (botones, inputs)
* Modelos de datos
* Pipes y directivas reutilizables

---

## 🌍 app-routing.module.ts

Define las **rutas principales** del proyecto.

Ejemplo:

* `/login`
* `/dashboard`

También permite **lazy loading** de módulos.

---

## 🧩 app.module.ts

Es el **módulo raíz** de la aplicación.

Aquí se:

* Importan módulos principales
* Declaran componentes globales
* Configura la app al iniciar

---

## 📂 src/assets

Archivos estáticos del proyecto.

```text
assets/
├── images/
│   └── gym.jpg
├── icons/
└── styles/
```

### 📌 ¿Qué va aquí?

* Imágenes
* Íconos
* Fuentes
* Archivos CSS/SCSS compartidos

---

## 🌎 environments/

Configuración por entorno.

```text
environments/
├── environment.ts
└── environment.prod.ts
```

### 📌 Uso

* URLs del backend
* Flags de producción

Ejemplo:

```ts
apiUrl: 'http://localhost:8080'
```

---

## 🎨 styles.scss

Archivo global de estilos.

Aquí se definen:

* Colores del sistema
* Tipografías
* Estilos generales

---

## 📦 package.json

Define:

* Dependencias
* Scripts (`ng serve`, `ng build`)

---

## ⚙️ angular.json

Configuración del proyecto Angular:

* Build
* Assets
* Estilos
* Producción

⚠️ Normalmente no se modifica mucho.

---

## 🚀 Buenas prácticas aplicadas

* Arquitectura modular
* Lazy loading
* Separación de responsabilidades
* Escalable para proyectos empresariales

---

## 🔮 Próximos pasos

* Conectar con Spring Boot
* Implementar JWT
* Crear dashboard
* Proteger rutas

---

✍️ **Autor:** Jofre Zambrano
🎓 Proyecto académico / profesional

