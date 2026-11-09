# Actividad: FORM-FB-01
 
- **Universidad:** Universidad Técnica Estatal de Quevedo
- **Facultad:** Facultad de Ciencias de la Computación
- **Carrera:** Carrera de Software
- **Asignatura:** Aplicaciones Distribuidas
- **Nivel y paralelo:** Séptimo nivel, paralelo B
- **Docente:** Gleiston Guerrero Ulloa, PhD
- **Fecha de entrega:** 8 de noviembre de 2026
## Integrantes y ramas de entrega
 
Cada trabajo individual se encuentra en su respectiva rama. Para verlo, usa el enlace de la tabla o elige la rama en el desplegable de ramas de GitHub.
 
| N° | Integrante | Rama | Contenido | Enlace |
|:-:|---|---|---|---|
| 1 | Benites Pérez Dariem Alberto | `main` | Carátula del grupo y fichas bibliográficas (LaTeX, BibTeX y PDF) | [Ver rama](https://github.com/DALBEZ-ROG/AD-FORM-FB-01-ABZ/tree/main) |
| 2 | Apunte Pazmiño Washington German | `apunte-washington` | Fichas bibliográficas (LaTeX, BibTeX y PDF), los cinco artículos citados en `referencias-pdf/` y su propio README con las instrucciones de compilación | [Ver rama](https://github.com/DALBEZ-ROG/AD-FORM-FB-01-ABZ/tree/apunte-washington) |
| 3 | Zambrano Triviño Leonel Leonidas | `zambrano-leonel` | Fichas bibliográficas en la carpeta `documento/` y su propio README | [Ver rama](https://github.com/DALBEZ-ROG/AD-FORM-FB-01-ABZ/tree/zambrano-leonel) |
 
## Cómo compilar (rama `main`)
 
- **Compilador:** pdfLaTeX con Biber.
- **Archivo principal:** `main.tex`.
- **Dependencias:** MiKTeX o TeX Live, con los paquetes biblatex y biblatex-ieee.
```
cd documento
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```
 
## Archivos de la rama `main`
 
- `documento/main.tex`: el código LaTeX de las fichas.
- `documento/referencias.bib`: las referencias en formato BibTeX.
- `documento/main.pdf`: el PDF ya compilado.
- `caratula.tex` y `caratula.pdf`: la carátula con el repositorio.
La carátula se compila aparte, desde la carpeta principal:
 
```
pdflatex caratula.tex
```
