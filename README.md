<h1 align="center">Guía de Aprendizaje de Git y GitHub para Dummies</h1>

<p align="justify">¡Bienvenido a esta guía de aprendizaje de Git y GitHub! En este documento, te proporcionaremos una introducción básica a las principales funcionalidades de Git y cómo utilizar GitHub para colaborar en proyectos de desarrollo de software. A lo largo del documento, exploraremos conceptos clave y te mostraremos ejemplos prácticos para que puedas familiarizarte con el flujo de trabajo de Git y GitHub.</p>

## Introducción a Git y GitHub

### ¿Qué es Git?

<div style="width: 100%;position: relative;display: flex;align-items: center">
    <img align="left" width="120px" alt="git" src="https://media0.giphy.com/media/kH1DBkPNyZPOk0BxrM/giphy.gif?cid=ecf05e47t5u2xixvb21ps80wmwtjscc7lbkyewgxe51khdov&ep=v1_gifs_related&rid=giphy.gif&ct=s"/>
    <p align="justify">
        Git es un sistema de control de versiones distribuido que permite realizar un seguimiento de los cambios realizados en archivos y coordinar el trabajo en equipo. Proporciona una forma eficiente de manejar proyectos, realizar seguimiento de modificaciones, revertir cambios y colaborar con otros desarrolladores.
    </p>
</div>

### ¿Qué es GitHub?

<div style="width: 100%;position: relative;display: flex; align-items: center">
    <img align="left" width="120px" alt="github" src="https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExcDRucWZmeHo5dTQ1OXlocGd2MXRmbDE1emc4NDVlczh0NzF4cjc5OCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/KzJkzjggfGN5Py6nkT/giphy.gif"/>
    <p align="justify">
        GitHub es una plataforma basada en la web que utiliza Git para alojar repositorios de código. Además de las funcionalidades de Git, GitHub ofrece características adicionales, como la posibilidad de colaborar en proyectos de código abierto, realizar seguimiento de problemas y solicitar fusiones de código.
    </p>
</div>

## Configuración inicial

Antes de comenzar a utilizar Git y GitHub, es necesario realizar una configuración inicial. A continuación, se detallan
los pasos básicos:

### Instalación de Git

Descarga Git desde https://git-scm.com/downloads e instálalo en tu sistema operativo.

### Configuración de Git

Abre una terminal o línea de comandos y ejecuta los siguientes comandos para configurar tu nombre de usuario y dirección
de correo electrónico:

```bash
$ git config --global user.name "Tu Nombre"
$ git config --global user.email "tu@email.com"
```

## Conceptos básicos de Git

En esta sección, aprenderemos los conceptos básicos de Git y cómo utilizarlos.

### Inicializar un repositorio

Para comenzar a utilizar Git en un proyecto existente o en uno nuevo, debemos inicializar un repositorio. Ejecuta el
siguiente comando en la terminal en la ubicación de tu proyecto:

```bash
$ git init
```

### Realizar un commit

Un commit es una confirmación de cambios en el repositorio. Para realizar un commit, debemos seguir estos pasos:

1. Agrega los archivos modificados al área de preparación:

```bash
$ git add nombre_archivo
```

2. Realiza el commit con un mensaje descriptivo:

```bash
$ git commit -m "Mensaje descriptivo del commit"
```

### Fusionar ramas (merge)

La funcionalidad de fusionar ramas permite combinar los cambios de una rama con otra. Utiliza el siguiente comando para
fusionar una rama en la rama actual:

```bash
$ git merge nombre_rama
```

### Cambiar de rama (checkout)

El comando checkout se utiliza para cambiar entre ramas existentes. Si deseas cambiar a una rama específica, ejecuta el
siguiente comando:

```bash
$ git checkout nombre_rama
```

### Enviar cambios a un repositorio remoto (push)

Para enviar tus cambios locales a un repositorio remoto, utiliza el comando push:

```bash
$ git push nombre_remoto nombre_rama
```

### Obtener cambios del repositorio remoto (pull)

Si otros colaboradores han realizado cambios en el repositorio remoto, puedes obtener esos cambios y fusionarlos con tu
rama local utilizando el comando pull:

```bash
$ git pull nombre_remoto nombre_rama
```

## Trabajando con GitHub

En esta sección, aprenderemos cómo utilizar GitHub para colaborar en proyectos y aprovechar sus características
adicionales.

### Crear un repositorio en GitHub

1. Inicia sesión en tu cuenta de GitHub.
2. Haz clic en el botón "New" para crear un nuevo repositorio.
3. Completa los detalles del repositorio, como nombre, descripción y configuración adicional.
4. Haz clic en "Create repository" para crear el repositorio.

### Conectar repositorio local con repositorio remoto

Para conectar tu repositorio local con el repositorio remoto en GitHub, utiliza el siguiente comando:

```bash
$ git remote add nombre_remoto url_remoto
```

### Enviar cambios a GitHub (push)

Una vez que hayas realizado los commits locales, puedes enviar tus cambios al repositorio remoto en GitHub utilizando el
comando push:

```bash
$ git push nombre_remoto nombre_rama
```

### Solicitar una fusión de código (pull request)

Si deseas contribuir a un proyecto en GitHub, puedes enviar una solicitud de fusión de código (pull request) para que
los propietarios del repositorio revisen tus cambios y los incorporen al proyecto principal.

¡Felicidades! Ahora tienes una base sólida para comenzar a utilizar Git y GitHub. Este documento solo proporciona una
introducción básica, pero te animamos a explorar más a fondo cada uno de los temas mencionados y a utilizar las
numerosas características adicionales que ofrecen estas herramientas.

Happy coding!
