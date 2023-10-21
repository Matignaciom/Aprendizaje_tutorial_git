Git es un sistema de control de versiones distribuido ampliamente utilizado para el seguimiento de cambios en proyectos de software.

A continuación, te proporcionaré una guía básica de Git:

# Introducción a Git

## ¿Qué es Git?
Git es un sistema de control de versiones que permite rastrear los cambios en archivos y colaborar en proyectos de software. Cada cambio se registra en un "commit", lo que permite un seguimiento detallado de la historia de un proyecto.

## Configuración Inicial
Antes de empezar, configura tu nombre y dirección de correo electrónico en Git:

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"
```

## Comandos Básicos

### Iniciar un Repositorio
Para comenzar a usar Git en un directorio:

```bash
git init
```

### Agregar Archivos
Agrega archivos al área de preparación (staging) antes de hacer un commit:

```bash
git add archivo.txt  # Agregar un archivo específico
git add .            # Agregar todos los archivos
```

### Realizar Commit
Crea un commit con los archivos en el área de preparación:

```bash
git commit -m "Mensaje descriptivo"
```

### Ver Historial
Muestra el historial de commits:

```bash
git log
```

## Ramas

### Crear una Rama
Crea una nueva rama para desarrollar una función o corrección:

```bash
git branch nombre_de_rama
```

### Cambiar de Rama
Cambia a una rama específica:

```bash
git checkout nombre_de_rama
```

### Fusionar Ramas
Combina los cambios de una rama en otra:

```bash
git merge nombre_de_rama
```

## Ignorar Archivos

Crea un archivo `.gitignore` en el repositorio para especificar archivos o patrones que deben ser ignorados por Git. Por ejemplo, para ignorar archivos `.log` y la carpeta `node_modules`:

```
*.log
node_modules/
```

## Repositorios Remotos

### Clonar un Repositorio Remoto
Copia un repositorio remoto a tu máquina:

```bash
git clone URL_del_repositorio
```

### Agregar un Repositorio Remoto
Conecta tu repositorio local a uno remoto:

```bash
git remote add nombre_remoto URL_del_repositorio
```

### Subir Cambios
Sube tus cambios al repositorio remoto:

```bash
git push nombre_remoto nombre_de_rama
```

### Descargar Cambios
Obtiene los cambios del repositorio remoto:

```bash
git pull nombre_remoto nombre_de_rama
```

## Funcionalidades Adicionales

### Etiquetas (Tags)
Crea etiquetas para versiones específicas del proyecto:

```bash
git tag -a v1.0 -m "Versión 1.0"
```

### Submódulos
Incluye subproyectos como submódulos en tu repositorio:

```bash
git submodule add URL_del_submodulo
```

## Comandos Avanzados

### Stash
Guarda cambios temporales sin hacer commit:

```bash
git stash
git stash pop
```

### Rebase
Reorganiza y combina commits en una rama:

```bash
git rebase nombre_de_rama
```

### Bisect
Ayuda a encontrar el commit que introdujo un problema:

```bash
git bisect start
git bisect bad
git bisect good
```

## Referencias

- Documentación oficial de Git: https://git-scm.com/doc
- GitHub Guides: https://guides.github.com/
- Pro Git Book: https://git-scm.com/book/en/v2

Esta es una introducción básica a Git. Puedes encontrar más información y funcionalidades avanzadas en los recursos proporcionados. Recuerda que la práctica es esencial para aprender Git con éxito.

## Agradecimientos

Hecho con ❤️ por Matias Ignacio - https://github.com/Matignaciom
