# Music — Ejercicio GitHub

## Objetivo

Reforzar los conocimientos adquiridos en las sesiones de Git y GitHub mediante la creación y gestión colaborativa de una página web sencilla.

El proyecto se llama **Music** y presenta información relacionada con diferentes bandas de rock.

---

## Descripción del ejercicio

Construir una página web sencilla que incluya los elementos descritos a continuación:

* Una página de inicio llamada `index.html`.
* Integración de Bootstrap 5 mediante CDN.
* Una carpeta `css/` que contenga el archivo `global.css`.
* Contenido relacionado con bandas de rock.
* Uso de Git y GitHub para trabajar de manera colaborativa mediante ramas.

---

## Estructura del proyecto

La estructura básica del proyecto será:

```text
music/
│
├── index.html
│
├── css/
│   └── global.css
│
└── README.md
```

### `index.html`

Es la página principal del proyecto. En ella se mostrará la información sobre las bandas de rock.

### Bootstrap 5

El proyecto debe incluir Bootstrap 5 mediante CDN para utilizar sus componentes y clases de estilos.

Ejemplo:

```html
<link
  href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css"
  rel="stylesheet"
>
```

### `css/global.css`

Contendrá los estilos personalizados de nuestra página web, complementando los estilos proporcionados por Bootstrap.

---

## Flujo de trabajo con ramas

Para organizar el trabajo colaborativo se utilizará la siguiente estructura de ramas:

```text
main
 │
 └── develop
      ├── mario
      ├── alma
      └── angelica
```

### `main`

Es la rama principal del proyecto. Contendrá las versiones estables del sitio web.

### `develop`

Es la rama de desarrollo. Se utilizará como base para integrar los cambios realizados por los integrantes del equipo antes de llevarlos a `main`.

### Ramas individuales

Dentro de `develop`, cada integrante tendrá su propia rama para trabajar de manera independiente:

* `mario`
* `alma`
* `angelica`

Cada integrante deberá realizar sus cambios en su propia rama y posteriormente integrarlos a `develop`.

---

## Flujo de trabajo

El flujo de trabajo recomendado será:

1. Clonar el repositorio.
2. Obtener o actualizar las ramas existentes.
3. Trabajar sobre la rama correspondiente.
4. Realizar los cambios necesarios.
5. Agregar los archivos modificados.
6. Crear un commit con los cambios.
7. Actualizar la rama antes de integrar cambios.
8. Subir los cambios al repositorio remoto.
9. Integrar las modificaciones en `develop`.
10. Una vez que el proyecto esté listo y estable, integrar `develop` en `main`.

---

# Comandos de Git y Bash

El ejercicio tiene como finalidad practicar los principales comandos utilizados durante el trabajo con Git y GitHub.

## `git clone`

Permite copiar un repositorio remoto de GitHub a nuestra computadora.

```bash
git clone URL_DEL_REPOSITORIO
```

Por ejemplo:

```bash
git clone https://github.com/usuario/music.git
```

Este comando crea una copia local del proyecto para poder trabajar con él.

---

## `git branch`

Permite crear, consultar y administrar ramas dentro de un repositorio.

Para consultar las ramas existentes:

```bash
git branch
```

Para crear una nueva rama:

```bash
git branch mario
```

Las ramas permiten que diferentes integrantes trabajen en funcionalidades independientes sin modificar directamente la rama principal.

---

## `git add`

Permite agregar archivos modificados al área de preparación (*staging area*) antes de realizar un commit.

Para agregar un archivo específico:

```bash
git add index.html
```

Para agregar todos los archivos modificados:

```bash
git add .
```

---

## `git commit`

Guarda los cambios preparados en el historial local del repositorio.

```bash
git commit -m "Agrega contenido de bandas de rock"
```

Es recomendable utilizar mensajes de commit claros y descriptivos para identificar fácilmente qué cambios se realizaron.

---

## `git pull`

Permite descargar los cambios más recientes del repositorio remoto y actualizar nuestra copia local.

```bash
git pull
```

También podemos especificar una rama:

```bash
git pull origin develop
```

Este comando es importante para mantener nuestro trabajo actualizado antes de realizar nuevas modificaciones o integrar cambios.

---

# Ejemplo de flujo de trabajo

Un integrante puede comenzar su trabajo de la siguiente manera:

```bash
git clone URL_DEL_REPOSITORIO

cd music

git branch
```

Después puede cambiar a su rama de trabajo:

```bash
git checkout mario
```

Realiza sus modificaciones en `index.html` o `css/global.css`.

Posteriormente agrega los cambios:

```bash
git add .
```

Crea un commit:

```bash
git commit -m "Agrega información de bandas de rock"
```

Antes de continuar trabajando, puede actualizar su repositorio:

```bash
git pull
```

Finalmente, los cambios pueden ser enviados al repositorio remoto y posteriormente integrados en la rama `develop`.

---

# Finalidad del ejercicio

Este ejercicio tiene como finalidad practicar el uso de Git y GitHub dentro de un flujo de trabajo colaborativo.

Durante el desarrollo del proyecto se busca reforzar especialmente el uso de:

* `git clone` — Clonar un repositorio.
* `git branch` — Crear y administrar ramas.
* `git add` — Preparar cambios para un commit.
* `git commit` — Registrar cambios en el historial.
* `git pull` — Obtener los cambios del repositorio remoto.

Además, se busca comprender cómo organizar un proyecto utilizando una rama principal (`main`), una rama de desarrollo (`develop`) y ramas individuales para cada integrante del equipo.

---

## Equipo

| Integrante | Rama       |
| ---------- | ---------- |
| Mario      | `mario`    |
| Alma       | `alma`     |
| Angelica   | `angelica` |

---

## Proyecto

**Nombre:** Music
**Tema:** Bandas de rock
**Tecnologías:** HTML5, CSS3, Bootstrap 5, Git y GitHub
