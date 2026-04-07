# BD_PROYECTO — Repositorio del Equipo

Este repositorio será utilizado para desarrollar el proyecto entre Entrega 2 y Entrega 3 utilizando Git como herramienta de seguimiento del progreso.

Durante **las semanas indicadas** el equipo deberá trabajar en tareas específicas registrando su progreso mediante:

- commits
- ramas
- pull requests
- registro semanal en el **CHANGELOG.md**

El objetivo es que el repositorio refleje claramente **cómo evolucionó el proyecto a lo largo del tiempo**, cumpliendo con los entregables semanalmente.

---

## 🛠️ Metodología de Trabajo

Durante el desarrollo del proyecto se deben seguir las siguientes reglas:

### 1. Trabajo por Ramas

Cada tarea debe realizarse en **una rama diferente**.

**Nombre sugerido:**
```
feature/<descripcion>
```

**Ejemplos:**
```
feature/consulta-votos-candidato
feature/modelo-fisico
feature/modelo-logico
```

#### Flujo recomendado:

**1. Crear la rama desde `main`**
```bash
git checkout main
git pull
git checkout -b feature/nombre-tarea
```

**2.** Realizar commits del progreso.
```bash
git add .
git commit -m "Mensaje de commit"
```

**3. Subir la rama al repositorio:**
```bash
git push origin feature/nombre-tarea
```

**4.** Crear un **Pull Request** para integrar los cambios en `main`.

---

### 2. Registro del Progreso

Cada semana se debe actualizar el archivo:
```
CHANGELOG.md
```

En este archivo deben registrar:

| Campo | Descripción |
|-------|-------------|
| 🎯 Objetivos | Metas de la semana |
| ✅ Tareas realizadas | Lo que se completó |
| 👤 Responsables | Integrantes a cargo |
| 🌿 Ramas utilizadas | Nombres de las ramas |
| ⚠️ Problemas | Inconvenientes encontrados |

Esto permitirá evaluar el **progreso del equipo durante el desarrollo del proyecto**.

---

# 📋 Planificación de Entregas — Proyecto Base de Datos Electoral

---

## 🗂️ ENTREGA 2

### ✅ Entregables

#### 1. Consultas Avanzadas

**Uso obligatorio de:**
- JOINs múltiples
- Subconsultas
- CTE (si el motor lo permite)
- Funciones de agregación

**Agregaciones por nivel territorial:**
- Mesa
- Puesto
- Municipio
- Departamento
- Nacional

> **Mínimo 6–10 consultas orientadas a transparencia y análisis electoral.**

---

#### 2. Perfección del Modelo

- Modelo Lógico
- Modelo Físico
- Normalización hasta **3FN**

---

#### 3. Roles y Privilegios

**Definición de roles:**
- Administrador
- Analista
- Auditor / Consulta

> **Restricciones de acceso por rol.**

---

#### 4. Pruebas

- Casos de prueba **exitosos** (escenarios válidos)
- Casos de prueba **fallidos** (violaciones de reglas)

---

### 📅 Calendario — Entrega 2

#### Semana 1 · 16–22 marzo · `[Semana 8 académica]`

| # | Tarea | Notas |
|---|-------|-------|
| 1 | Taller de Git | ⭐ Opcional — bono |
| 2 | Subir documentos de la 1ª entrega al repositorio | |
| 3 | Ajustes de observaciones | |
| 4 | Definir consultas a realizar | |

#### Semana 2 · 23–29 marzo · `[Semana 9 académica]`

| # | Tarea |
|---|-------|
| 1 | Modelo Lógico |
| 2 | Consultas Avanzadas |

#### Semana 3 · 6–12 abril · `[Semana 10 académica]`

| # | Tarea |
|---|-------|
| 1 | Modelo Físico |
| 2 | Definición de roles: Administrador, Analista, Auditor/Consulta |
| 3 | Restricciones de acceso por rol |

#### Semana 4 · 13–22 abril · `[Semanas 11–12 académica]`

| # | Tarea |
|---|-------|
| 1 | Normalización hasta 3FN |
| 2 | Pruebas |

---

## 🗂️ ENTREGA 3

### ✅ Entregables

#### 1. Programación en Base de Datos

**Funciones — Ejemplos esperados:**
- Cálculo automático de participación
- Ranking por territorio
- Validaciones lógicas

**Procedimientos Almacenados — Ejemplos esperados:**
- Carga masiva controlada de resultados
- Consolidación automática por nivel territorial
- Cierre de jornada electoral

**Triggers — Obligatorios:**

| Trigger | Descripción |
|---------|-------------|
| Auditoría | Modificaciones en actas/resultados |
| Validación de rangos | No votos negativos |
| Anti-duplicidad | Prevención de duplicidad de actas |
| Consistencia | Votos totales vs. suma de detalle |

---

#### 2. Aplicación Funcional (Web o Escritorio)

**Debe permitir:**

- **Administración de catálogos:**
  - Proceso electoral
  - Territorio
  - Puestos
  - Mesas
  - Opciones de voto (candidatos/listas)
- **Registro** de actas y resultados
- **Consulta** de resultados consolidados
- **Consulta** de incidencias y reportes

---

#### 3. Reportes

- Panel de visualización con filtros
- Resultados agregados por nivel territorial
- Indicadores básicos:
  - Participación
  - Top candidatos
  - Incidencias

---

### 📅 Calendario — Entrega 3

#### Semana 1 · 27 abril – 3 mayo · `[Semana 13 académica]`

| # | Tarea                                  |
| - | -------------------------------------- |
| 1 | Funciones |
| 2 | Procedimientos almacenados |

#### Semana 2 · 4–10 mayo · `[Semana 14 académica]`

| # | Tarea                                  |
| - | -------------------------------------- |
| 1 | Triggers |
| 2 | Aplicación funcional (conexión a BD) |

#### Semana 3 · 11–20 mayo · `[Semanas 15–16 académica]`

| # | Tarea                                  |
| - | -------------------------------------- |
| 1 | Desarrollo de la aplicación |
| 2 | Reportes |

---

## 📁 Estructura de Carpetas del Proyecto

```text
BD_PROYECTO/
│
├── app/                    ---> 3ra Entrega
├── docs/                   ---> Documentos, Modelos, Imágenes
│
├── sql/
│   ├── consultas/
│   ├── ddl/
│   ├── funciones/          ---> 3ra Entrega
│   ├── procedimientos/     ---> 3ra Entrega
│   ├── roles/
│   └── triggers/           ---> 3ra Entrega
│
├── tests/
│
├── .gitignore
├── CHANGELOG.md
└── README.md
```

---

## 💬 Contacto

De presentar alguna inquietud con respecto al proyecto, uso de git para este o los parámetros planteados, contactar a la monitora:

**Viviana Gómez**  
📧 Teams o Correo: [gomezlv@javeriana.edu.co](mailto:gomezlv@javeriana.edu.co)
