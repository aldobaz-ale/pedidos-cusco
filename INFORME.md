# Laboratorio 1: Introducción al entorno de desarrollo y Git

**Curso:** Ingeniería de Software
**Estudiante:** Aldo Yaranga Achahui (103179@unsaac.edu.pe)
**GitHub:** https://github.com/aldobaz-ale
**Caso:** Sistema web de pedidos de comida local para una startup en Cusco

## 1. Objetivo

Configurar un entorno de desarrollo y aplicar control de versiones con Git en un proyecto básico.

## 2. Parte 1: Configuración

```bash
$ git --version
git version 2.43.0

$ git config --global user.name "Aldo Yaranga Achahui"
$ git config --global user.email 103179@unsaac.edu.pe
$ git config --global --list
user.name=Aldo Yaranga Achahui
user.email=103179@unsaac.edu.pe
```

## 3. Parte 2: Proyecto inicial

```bash
$ mkdir pedidos-cusco
$ cd pedidos-cusco
$ git init
Initialized empty Git repository in .../pedidos-cusco/.git/
```

## 4. Parte 3: Versionamiento

Se creó el `README.md` documentado y un `.gitignore`.

```bash
$ git add .
$ git commit -m "Primer commit"
```

## 5. Parte 4: Repositorio remoto

Repositorio creado en GitHub: https://github.com/aldobaz-ale/pedidos-cusco

```bash
git remote add origin https://github.com/aldobaz-ale/pedidos-cusco.git
git push -u origin main
```

## 6. Entregables

| Entregable | Ubicación |
|---|---|
| URL del repositorio | https://github.com/aldobaz-ale/pedidos-cusco |
| Evidencias de commits | https://github.com/aldobaz-ale/pedidos-cusco/commits/main |
| README documentado | `README.md` en la raíz del repositorio |

## 7. Reflexión

**¿Por qué Git es crítico en proyectos colaborativos?**
Porque permite que varias personas trabajen en paralelo sobre el mismo código sin pisarse: cada quien trabaja en su rama y luego integra sus cambios (merge / pull request). Además deja un historial completo de quién cambió qué, cuándo y por qué (trazabilidad), y permite volver a cualquier versión anterior si algo falla. GitHub añade revisión de código, seguimiento de incidencias y un respaldo remoto del proyecto.

**¿Qué problemas evita?**
- Pérdida de código o de trabajo por borrados o fallos del equipo.
- Sobrescritura de cambios entre compañeros.
- Archivos duplicados tipo `proyecto_final_v2_FINAL.zip` y confusión sobre cuál es la versión vigente.
- No saber quién introdujo un error ni cuándo (se resuelve con `git log` y `git blame`).
- Dificultad para revertir un cambio que rompió el sistema (`git revert`, `git checkout`).
- Falta de un respaldo centralizado y de un flujo ordenado de revisión antes de publicar.
