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
├── LICENSE
├── README.md
│
└── css/
    └── global.css
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
      ├── html
      └── css
```

### `main`

Es la rama principal del proyecto. Contendrá las versiones estables y terminadas del sitio web.

### `develop`

Es la rama de desarrollo. Se utilizará como base para integrar los cambios realizados en las ramas de trabajo antes de llevar el proyecto a `main`.

### Rama `html`

Esta rama estará destinada al desarrollo y modificación de la estructura HTML del proyecto, principalmente del archivo:

```text
index.html
```

En esta rama se trabajará la estructura y el contenido de la página web.

### Rama `css`

Esta rama estará destinada al desarrollo de los estilos personalizados del proyecto, principalmente del archivo:

```text
css/global.css
```

En esta rama se trabajará la apariencia visual de la página.

---

## Flujo de trabajo

El flujo de trabajo recomendado será:

1. Clonar el repositorio.
2. Actualizar la información del repositorio local.
3. Crear o utilizar la rama correspondiente.
4. Realizar los cambios necesarios.
5. Agregar los archivos modificados.
6. Crear un commit con los cambios.
7. Subir los cambios a GitHub.
8. Integrar las ramas `html` y `css` en `develop`.
9. Una vez que el proyecto esté terminado y estable, integrar `develop` en `main`.

El flujo general será:

```text
main
  │
  └── develop
       ├── html
       │
       └── css
```

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
git branch html
```

Las ramas permiten separar el trabajo y desarrollar diferentes partes del proyecto sin modificar directamente la rama principal.

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
git commit -m "Agrega estructura HTML"
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

Para trabajar en la parte HTML, se puede utilizar la rama `html`:

```bash
git checkout html
```

Se realizan los cambios necesarios en `index.html`.

Después se agregan los cambios:

```bash
git add .
```

Se crea un commit:

```bash
git commit -m "Agrega estructura de la página"
```

Finalmente, se envían los cambios a GitHub:

```bash
git push origin html
```

Para trabajar en los estilos CSS, se utiliza la rama `css`:

```bash
git checkout css
```

Se realizan los cambios en:

```text
css/global.css
```

Después:

```bash
git add .
git commit -m "Agrega estilos globales"
git push origin css
```

Posteriormente, las ramas `html` y `css` se integrarán en `develop`.

---

# Finalidad del ejercicio

Este ejercicio tiene como finalidad practicar el uso de Git y GitHub dentro de un flujo de trabajo colaborativo.

Durante el desarrollo del proyecto se busca reforzar especialmente el uso de:

* `git clone` — Clonar un repositorio.
* `git branch` — Crear y administrar ramas.
* `git add` — Preparar cambios para un commit.
* `git commit` — Registrar cambios en el historial.
* `git pull` — Obtener los cambios del repositorio remoto.

Además, se busca comprender cómo organizar un proyecto utilizando una rama principal (`main`), una rama de desarrollo (`develop`) y ramas específicas para trabajar en diferentes partes del proyecto (`html` y `css`).

---

## Ramas del proyecto

| Rama      | Función                          |
| --------- | -------------------------------- |
| `main`    | Rama principal y versión estable |
| `develop` | Rama de desarrollo e integración |
| `html`    | Desarrollo de la estructura HTML |
| `css`     | Desarrollo de los estilos CSS    |

---

## Proyecto

**Nombre:** Music
**Tema:** Bandas de rock
**Tecnologías:** HTML5, CSS3, Bootstrap 5, Git y GitHub

---

## Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo [LICENSE](LICENSE) para conocer los términos y condiciones de uso, modificación y distribución del proyecto.



