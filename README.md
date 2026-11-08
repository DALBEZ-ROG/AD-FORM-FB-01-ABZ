# FORM-FB-01 · Fichas bibliográficas de sistemas distribuidos

> Rama de **Leonel Leonidas Zambrano Triviño**: cinco fichas bibliográficas sobre sistemas distribuidos y microservicios, base del informe TA-IND-01.

| Dato | Detalle |
|---|---|
| Institución | Universidad Técnica Estatal de Quevedo |
| Facultad | Ciencias de la Computación |
| Carrera | Software |
| Asignatura | Aplicaciones Distribuidas |
| Nivel | Séptimo, paralelo A |
| Docente | Gleiston Guerrero Ulloa, PhD |
| Entrega | 8 de noviembre de 2026 |

## Estructura de la rama

```
documento/
├── main.tex          # documento LaTeX con las 5 fichas
├── referencias.bib   # base bibliográfica (biblatex)
└── main.pdf          # versión compilada
```

## Compilación

Se necesita una distribución de LaTeX (**TeX Live** o **MiKTeX**) que incluya:

- `biblatex` y el estilo `biblatex-ieee`, para las referencias en formato IEEE
- `biber`, que procesa la bibliografía (no se usa BibTeX)
- `babel` con español e inglés, y `csquotes`

El archivo principal es `documento/main.tex` y se compila con **pdfLaTeX**. Hay que correr biber entre dos pasadas de pdfLaTeX para que aparezcan las citas:

```bash
cd documento
pdflatex main
biber main
pdflatex main
pdflatex main
```

En Overleaf basta con subir `main.tex` y `referencias.bib` y compilar con pdfLaTeX; Overleaf ejecuta biber automáticamente.

## Artículos revisados

Todos son de acceso abierto en IEEE Xplore:

| # | Tema | Revista | Año | DOI |
|---|---|---|---|---|
| 1 | Algoritmos de consenso en blockchain | IEEE Access | 2023 | [10.1109/ACCESS.2023.3267047](https://doi.org/10.1109/ACCESS.2023.3267047) |
| 2 | Descomposición de monolitos en microservicios | IEEE Trans. Softw. Eng. | 2023 | [10.1109/TSE.2023.3287297](https://doi.org/10.1109/TSE.2023.3287297) |
| 3 | Consumo energético en microservicios | IEEE Access | 2024 | [10.1109/ACCESS.2024.3389064](https://doi.org/10.1109/ACCESS.2024.3389064) |
| 4 | Seguridad entre servicios | IEEE Access | 2024 | [10.1109/ACCESS.2024.3406500](https://doi.org/10.1109/ACCESS.2024.3406500) |
| 5 | Observabilidad en microservicios | IEEE Access | 2025 | [10.1109/ACCESS.2025.3562125](https://doi.org/10.1109/ACCESS.2025.3562125) |

## Sobre el uso de IA

Usé **Claude (Anthropic)** como asistente en tres tareas: localizar artículos recientes en IEEE Xplore y comprobar sus DOI, armar `referencias.bib` y la plantilla LaTeX, y ubicar dentro de cada artículo datos concretos con su página o sección. A partir de eso redacté los resúmenes y las notas personales.

Revisé cada DOI a mano, confirmando autores, año, título, revista, volumen y páginas contra la publicación original. El detalle completo está en la declaración al final de `main.pdf`.
