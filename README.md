<div align="center">

# Programación de Scripts en Linux (Bash Scripting)

![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Shell](https://img.shields.io/badge/Shell-Scripting-FF6B35?style=for-the-badge)

> Automatización de tareas de administración del sistema con Bash scripting en entorno Linux.

## Descripción

</div>

---

Laboratorio de programación de scripts en **Bash** para Linux: automatización de tareas del sistema operativo, gestión de archivos y directorios, procesamiento de texto con herramientas POSIX (`grep`, `awk`, `sed`), control de flujo, manejo de procesos en background y scripts de administración del sistema.

## Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `archivosdelinux.zip` | Scripts Bash del laboratorio |
| `*.pdf` | Informe con scripts, ejecuciones y resultados |

## Arquitectura

```mermaid
flowchart TD
    A[Programacion_De_Scripts_En_Linux] --> B[archivosdelinux.zip]
    A --> C[Informe PDF]
    B --> D[Variables y Sustitucion de Comandos]
    B --> E[Condicionales if/case]
    B --> F[Bucles for/while]
    B --> G[Funciones Bash]
    B --> H[Gestion de Procesos - ps / kill / background jobs]
    B --> I[Procesamiento de Texto - grep / awk / sed]
```

## Scripts implementados

```bash
#!/bin/bash
# Ejemplos de conceptos implementados:

# Variables y sustitución de comandos
fecha=$(date +%Y-%m-%d)

# Condicionales
if [ -f "$archivo" ]; then chmod 755 "$archivo"; fi

# Bucles
for f in *.log; do gzip "$f"; done

# Funciones
backup() { tar -czf "$1.tar.gz" "$1" && echo "Backup: $1 OK"; }

# Gestión de procesos
ps aux | grep nginx | awk '{print $2}' | xargs kill -9
```

## Contexto académico

**Asignatura:** Programación bajo Unix · **Institución:** Ingeniería Informática
**Autor:** Alejandro De Mendoza — Ingeniero Informático · Especialista Ingeniería de Software

---

## Autor

**Alejandro De Mendoza**  
Ingeniero Informático · Especialista en IA · Especialista en Ingeniería de Software · Máster en Arquitectura de Software

[![GitHub](https://img.shields.io/badge/GitHub-AlejoTechEngineer-181717?style=for-the-badge&logo=github)](https://github.com/AlejoTechEngineer)
