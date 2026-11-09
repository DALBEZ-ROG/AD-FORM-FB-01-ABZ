# Actividad: FORM-FB-01
Universidad Técnica Estatal de Quevedo

Facultad de Ciencias de la Computación

Carrera de Software

Cada trabajo individual se encuentra en su respectiva rama.

Integrantes: 

- BENITES PÉREZ DARIEM ALBERTO
- APUNTE PAZMIÑO WASHINGTON GERMAN
- ZAMBRANO TRIVIÑO LEONEL LEONIDAS

Aplicaciones Distribuidas

Séptimo nivel paralelo B

Docente: Gleiston Guerrero Ulloa, PhD

Fecha de entrega: 8 de noviembre de 2026

Cómo compilar:

Compilador: pdfLaTeX con Biber.

Archivo principal: main.tex.

Dependencias: MiKTeX o TeX Live, con los paquetes biblatex y biblatex-ieee.

```
cd documento
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

# Archivos

- documento/main.tex: el código LaTeX de las fichas.
- documento/referencias.bib: las referencias en formato BibTeX.
- documento/main.pdf: el PDF ya compilado.
- caratula.tex y caratula.pdf: la carátula con el repositorio.

La carátula se compila aparte, desde la carpeta principal:
```
pdflatex caratula.tex
```
