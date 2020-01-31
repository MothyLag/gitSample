# Repositorio de prueba

Este repositorio fué creado por motivos didacticos

## Instalación de git

para llevar a cabo el control de versiónes
se necesita del programa "git" en el sistema

### windows

para instalar git en windows solo tienes que ir al sitio de descarga en la
[web de git](https://git-scm.com/download/win,")

### MacOS

para instalar en MacOS,
puedes hacerlo desde el xcode command, solo corriendo

```
$ git --help

```

que ejectuara git en la terminal, o si no lo tienes instalado te enviara el prompt para hacerlo.

### Linux

#### Debian Based

para sistemas basados en debian solo se necesita correr en terminal:

```bash
$ sudo apt-get install git

```

para sistemas basados en arch solo se necesita correr en terminal:

#### Arch Based

```bash
$ yum install git

```

## Configuración de usuario

para utilizar git y que los cambios realizados se vean reflejados por usuario, se requiere configurar en el sistema el usuario con el que utilizara git, ya sea de manera individual para ese proyecto, o de manera global para todos los proyectos.

### Configuración global

```bash
$ git config --global user.name "UserName"
$ git config --global user.email email@example.com
```

### Configuración individual

no me acuerdo :p, pero existe XD

## Crear repositorio

esto viene en dos partes que llamaremos, crear repositorio desde la aplicación, e inicializar repositorio desde el proyecto.

### Crear repositorio desde la aplicación

para este apartado utilizaremos como ejemplo la plataforma de github aunque es bastante parecido en otras plataformas de repositorios.

solo debes dar click en el enorme boton verde que tiene la leyenda "New"

![git image](https://github.com/MothyLag/gitSample/blob/master/src/img/newRepo.png)

y finalmente rellenar el formulario con los siguientes datos:
nombre del repositorio, descripción y seleccionar si el repositorio será privado o público

![git image](https://github.com/MothyLag/gitSample/blob/master/src/img/newRepoForm.png)

### Inicializar repositorio desde el proyecto

#### inicialización desde cero

Para inicializar un proyecto en git desde cero primero debemos incluir los archivos necesarios para llevar acabo el control de versiones, para esto correremos la instrucción:

```bash
$ git init
```

después de esto pasaremos a clonar el repositorio en nuestro proyecto

```bash
$ git remote add git@github.com:MothyLag/gitSample.git
```

donde:

- **origin** es un alias para el workspace local, por lo general se define como origin,
- **MothyLag** es el owner del proyecto
- **gitSample** es el nombre del repositorio

finalmente para subir el proyecto al repositorio se ejecutan las siguientes instrucciónes

```bash
$ git add .
$ git commit -m"cualquier mensaje"
$ git push -u origin master
```

### inicialización desde un proyecto ya comenzado

si un proyecto ya está comenzado desde el repositorio de github, y desesas bajarlo a tu terminal para trabajar, tienes que hacer algo llamado "clonar el repositorio", que es obtener una copia esacta del proyecto que se encuentra en el repositorio, para esto ejecutaremos la siguiente instrucción.

```bash
git clone git@github.com:MothyLag/gitSample.git
```

donde:

- **MothyLag** es el owner del proyecto
- **gitSample** es el nombre del repositorio

e inmediatamente tendremos el proyecto en nuestro equipo.

## Subir cambios

para subir cambios a la rama actual de tu repositorio se necesitan hacer 3 pasos:

- agregar los cambiós al stage
- hacer un commit de los cambios en el stage
- subir el commit al repositorio

primero agregamos los archivos al stage:

```bash
$ git add .
```

el punto es para indicar que se agregaran todos los archivos que se han modificado,
pero también se pueden agregar cada uno de los archivos de manera individual

```bash
$ git add package.json
```

después procedemos a hacer un commit del cambio que estamos realizando

```bash
$ git commit -m"mensaje"
```

donde:

- **-m** es para indicar el parametro del mensaje que aparecerá en el commit

y finalmente subimos los cambios a la rama actual del repositorio

```bash
$ git push
```

#### Nota: para subir cambios necesitas tener actualizado tu espacio de trabajo.

## Descargar Cambios

```bash
$ git pull
```

## Crear rama y cambiar rama

para cambiar a una rama ya existente se utiliza el comando

```bash
$ git checkout <nombre_de_la_rama>
```

en cazó de que la rama aun no exista se utiliza el el comando

```git
$ git checkout -b <nombre_de_la rama>
```
