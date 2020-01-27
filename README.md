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
