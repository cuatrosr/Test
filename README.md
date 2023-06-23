<h1 align="center"><strong>Guía de Aprendizaje de Git y GitHub</strong></h1>

<p align="justify">¡Bienvenido a esta guía de aprendizaje de Git y GitHub! En este documento, te proporcionaremos una introducción básica a las principales funcionalidades de Git y cómo utilizar GitHub para colaborar en proyectos de desarrollo de software. A lo largo del documento, exploraremos conceptos clave y te mostraremos ejemplos prácticos para que puedas familiarizarte con el flujo de trabajo de Git y GitHub.</p>

## **Tabla de Contenido** 📁

1. [Introducción a Git y GitHub](#introducción-a-git-y-github-%EF%B8%8F)
   1. [¿Qué es Git?](#qué-es-git)
   2. [¿Qué es GitHub?](#qué-es-github)
2. [Configuración inicial](#configuración-inicial-%EF%B8%8F)
   1. [Instalación de Git](#instalación-de-git)
   2. [Configuración de Git](#configuración-de-git)
3. [Conceptos básicos de Git](#conceptos-básicos-de-git-)
   1. [Inicializar un repositorio](#inicializar-un-repositorio)
   2. [Realizar un commit](#realizar-un-commit)
   3. [Enviar cambios a un repositorio remoto (push)](#enviar-cambios-a-un-repositorio-remoto-push)
   4. [Obtener cambios del repositorio remoto (pull)](#obtener-cambios-del-repositorio-remoto-pull)
   5. [Cambiar de rama (checkout)](#cambiar-de-rama-checkout)
   6. [Fusionar ramas (merge)](#fusionar-ramas-merge)

## **Introducción a Git y GitHub** 💻️

### **¿Qué es Git?**

<div style="text-align: left">
    <a href="https://git-scm.com/" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/2ae2a900d2f041da66e950e4d48052658d850630/icons/git/git-original.svg" height="60" width = "60" alt="Git"></a>
</div>

<p align="justify">
    Git es un sistema de control de versiones distribuido que permite realizar un seguimiento de los cambios realizados en archivos y coordinar el trabajo en equipo. Proporciona una forma eficiente de manejar proyectos, realizar seguimiento de modificaciones, revertir cambios y colaborar con otros desarrolladores.
</p>

> **"Guardar archivos binarios** en el repositorio de git **es una mala práctica"**

### **¿Qué es GitHub?**

<div style="text-align: left">
    <a href="https://github.com/" target="_blank"> <img src="https://img.icons8.com/fluency-systems-filled/344/ffffff/github.png" height="60" width = "60" alt="GitHub"></a>
</div>

<p align="justify">
    GitHub es una plataforma basada en la web que utiliza Git para alojar repositorios de código. Además de las funcionalidades de Git, GitHub ofrece características adicionales, como la posibilidad de colaborar en proyectos de código abierto, realizar seguimiento de problemas y solicitar fusiones de código.
</p>

## **Configuración inicial** ⚙️

<p align="justify">
    Antes de comenzar a utilizar Git y GitHub, es necesario realizar una configuración inicial. A continuación, se detallan los pasos básicos:
</p>

### **Instalación de Git**

<p align="justify">
    Descarga Git desde <a href="https://git-scm.com/downloads">https://git-scm.com/downloads</a> e instálalo en tu sistema operativo.
</p>

<div style="text-align: left">
   <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/linux/linux-original.svg" height="60" width = "60" alt="Linux">
   <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/apple/apple-original.svg" height="60" width = "60" alt="MacOS">
   <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/windows8/windows8-original.svg" height="60" width = "60" alt="Windows">
</div>

### **Instalación de GitHub Desktop**

<p align="justify">
   Descargar GitHub Desktop desde <a href="https://desktop.github.com">https://desktop.github.com</a> e instálalo en tu sistema operativo.
</p>

<div style="text-align: left">
   <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/apple/apple-original.svg" height="60" width = "60" alt="MacOS">
   <img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/windows8/windows8-original.svg" height="60" width = "60" alt="Windows">
</div>

### **Configuración de Git**

#### Desde Consola

<p align="justify">
   Abre una terminal o línea de comandos y ejecuta los siguientes comandos para configurar tu nombre de usuario y dirección de correo electrónico:
</p>

```bash
$ git config --global user.name "Tu Nombre"
$ git config --global user.email "tu@email.com"
```

#### Desde GitHub Desktop

<p align="justify">
   Seleccione el menu de opciones en su apartado Git para configurar tu nombre de usuario y dirección de correo electrónico:
</p>

<div align="center">
   <img style="height: 400px" src="https://i.imgur.com/wFw2jQA.png" alt="Configuracion">
</div>

## **Estados de un Archivo** 📂️

- **Untracked:** Archivo que no está siendo rastreado por Git.
- **Modified:** Archivo que ha sido modificado desde el último commit.
- **Staged:** Archivo que ha sido modificado y añadido al área de preparación.
- **Committed:** Archivo que ha sido modificado, añadido al área de preparación y confirmado en el repositorio.
- **Pushed:** Archivo que ha sido modificado, añadido al área de preparación, confirmado en el repositorio y enviado al repositorio remoto.

<div align="center">
   <img style="height: 200px" src="https://i.imgur.com/Za8NF7S.png" alt="file-status">
</div>

## **Conceptos básicos de Git** 📝

<p align="justify">
   En esta sección, aprenderemos los conceptos básicos de Git y cómo utilizarlos.
</p>

### **Inicializar un repositorio**

<p align="justify">
   Para comenzar a utilizar Git en un proyecto existente o en uno nuevo, debemos inicializar un repositorio.
</p>

#### Desde Consola

<p align="justify">
   Ejecuta el siguiente comando en la terminal en la ubicación de tu proyecto:
</p>

```bash
$ git init
```

#### Desde GitHub Desktop

<p align="justify">
   Deberas de elegir la opcion de "Crear un nuevo repositorio en tu disco duro..." donde deberas llenar todos los campos correspondientes:
</p>

<div align="center">
   <img style="height: 400px" src="https://i.imgur.com/SoYyaQK.png" alt="Repositorio">
</div>

### **Realizar un commit**

<p align="justify">
   Un commit es una confirmación de cambios en el repositorio. Para realizar un commit, debemos seguir estos pasos:
</p>

<div align="center">
   <img style="height: 180px" src="https://i.imgur.com/VGdb7NE.png" alt="GitFlow">
</div>

> No puedes usar **commit** si antes no has añadido los archivos con **add**.

#### Desde Consola

1. Agrega los archivos modificados al área de preparación:

```bash
$ git add nombre_archivo
```

2. Realiza el commit con un mensaje descriptivo:

```bash
$ git commit -m "Mensaje descriptivo del commit"
```

#### Desde GitHub Desktop

1. Selecciona los archivos modificados:

<div align="center">
   <img style="height: 100px" src="https://i.imgur.com/IZJoC7W.png" alt="Add">
</div>

2. Realiza el commit con un mensaje descriptivo y opcionalmente agregale una descripción:

<div align="center">
   <img style="height: 200px" src="https://i.imgur.com/pJZgnmU.png" alt="Commit">
</div>

### **Crear una rama (branch)**

<p align="justify">
   Las ramas te permiten realizar cambios sin afectar la rama principal (Main). Un ejemplo de esto es al encontrar bugs en alguna versión entras a Hotfix, entonces se crea una nueva rama donde realias los cambios y los pruebas con la versión actual del Main.
</p>

#### En Consola

<p align="justify">
   Si deseas crear una rama, ejecuta el siguiente comando:
</p>

```bash
$ git branch nombre_rama
```

#### En GitHub Desktop

<p align="justify">
   Deberas de elegir la opcion "New Branch" dentro del dropdown de "Current Branch" llenando el campo requerido de nombre:
</p>

<div align="center">
   <img style="height: 200px" src="https://i.imgur.com/MmoCo1T.png" alt="Branch">
</div>

### **Cambiar de rama (checkout)**

<p align="justify">
   El comando checkout se utiliza para cambiar entre ramas existentes.
</p>

#### En Consola

<p align="justify">
   Si deseas cambiar a una rama específica, ejecuta el siguiente comando:
</p>

```bash
$ git checkout nombre_rama
```

#### En GitHub Desktop

<p align="justify">
   Deberas de seleccionar el dropdown de "Current Branch" para ver el listado de ramas de tu proyecto. Luego, darle click a la rama que quieres cambiar y elegir la opcion de tu preferencia:
</p>

<div align="center">
   <img style="height: 200px" src=https://i.imgur.com/yNuM6dT.png" alt="Branch">
</div>

<div align="right">
   <img style="height: 200px" src=https://i.imgur.com/yNuM6dT.png" alt="Branch">
</div>

### **Fusionar ramas (merge)**

<p align="justify">
   La funcionalidad de fusionar ramas permite combinar los cambios de una rama con otra. Utiliza el siguiente comando para fusionar una rama en la rama actual:
</p>

```bash
$ git merge nombre_rama
```

<div align="center">
   <img style="height: 180px" src="https://i.imgur.com/ldv7Qv4.png" alt="Merge">
</div>

## **Trabajando con GitHub** 🤝

En esta sección, aprenderemos cómo utilizar GitHub para colaborar en proyectos y aprovechar sus características
adicionales.

### **Crear un repositorio en GitHub**

1. Inicia sesión en tu cuenta de GitHub.
2. Haz clic en el botón **"New"** para crear un nuevo repositorio.
3. Completa los detalles del repositorio, como nombre, descripción y configuración adicional.
4. Haz clic en **"Create repository"** para crear el repositorio.

### **Conectar repositorio local con repositorio remoto**

Para conectar tu repositorio local con el repositorio remoto en GitHub, utiliza el siguiente comando:

```bash
$ git remote add nombre_remoto url_remoto
```

### **Enviar cambios a un repositorio remoto (push)**

<p align="justify">
   Para enviar tus cambios locales a un repositorio remoto, utiliza el comando push:
</p>

```bash
$ git push nombre_remoto nombre_rama
```

### **Obtener cambios del repositorio remoto (pull)**

<p align="justify">
   Si otros colaboradores han realizado cambios en el repositorio remoto, puedes obtener esos cambios y fusionarlos con tu rama local utilizando el comando pull:
</p>

```bash
$ git pull nombre_remoto nombre_rama
```

### **Enviar cambios a GitHub (push)**

Una vez que hayas realizado los commits locales, puedes enviar tus cambios al repositorio remoto en GitHub utilizando el
comando push:

```bash
$ git push nombre_remoto nombre_rama
```

### **Solicitar una fusión de código (pull request)**

Si deseas contribuir a un proyecto en GitHub, puedes enviar una solicitud de fusión de código (pull request) para que
los propietarios del repositorio revisen tus cambios y los incorporen al proyecto principal.

---

¡Felicidades! Ahora tienes una base sólida para comenzar a utilizar Git y GitHub. Este documento solo proporciona una
introducción básica, pero te animamos a explorar más a fondo cada uno de los temas mencionados y a utilizar las
numerosas características adicionales que ofrecen estas herramientas.

Happy coding! 🚀
----------------

[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com)
[![forthebadge](https://forthebadge.com/images/badges/for-you.svg)](https://forthebadge.com)
