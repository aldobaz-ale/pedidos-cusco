# Pedidos Cusco 🍲

Sistema web para gestionar pedidos de comida local, desarrollado para una startup en Cusco.

> Laboratorio 1 – Ingeniería de Software: Introducción al entorno de desarrollo y Git.

## Objetivo

Organizar el código del proyecto desde el inicio usando control de versiones con **Git** y alojarlo en **GitHub**, para facilitar el trabajo colaborativo, la trazabilidad de cambios y la recuperación de versiones.

## Herramientas

| Herramienta | Uso |
|---|---|
| Visual Studio Code / IntelliJ | Editor / IDE de desarrollo |
| Git | Control de versiones local |
| GitHub | Repositorio remoto y colaboración |

## Configuración del entorno

```bash
git --version
git config --global user.name "Aldo Yaranga Achahui"
git config --global user.email 103179@unsaac.edu.pe
```

## Flujo de trabajo seguido

```bash
mkdir pedidos-cusco && cd pedidos-cusco
git init                              # Inicializar repositorio
git add .                             # Preparar cambios
git commit -m "Primer commit"         # Guardar versión
git remote add origin https://github.com/aldobaz-ale/pedidos-cusco.git
git push -u origin main               # Subir al remoto
```

## Estructura del proyecto

```
pedidos-cusco/
├── README.md      # Documentación del proyecto
├── INFORME.md     # Informe del Laboratorio 1
└── .gitignore     # Archivos excluidos del control de versiones
```

## Funcionalidades previstas

- Catálogo de platos típicos locales
- Registro y seguimiento de pedidos
- Gestión de clientes y restaurantes

## Convención de commits

Mensajes cortos, en español y en imperativo (ej.: `Agregar .gitignore`, `Agregar informe del laboratorio`).

## Autor

- Aldo Yaranga Achahui
- GitHub: [aldobaz-ale](https://github.com/aldobaz-ale)
- Correo: 103179@unsaac.edu.pe
