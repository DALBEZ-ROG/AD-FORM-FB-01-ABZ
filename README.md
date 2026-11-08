# FORM-FB-01: Fichas bibliográficas

Trabajo individual de **Apunte Pazmiño Washington German** para Aplicaciones Distribuidas (ISR-701), séptimo nivel, paralelo B, Universidad Técnica Estatal de Quevedo. Docente: Gleiston Guerrero Ulloa, PhD. Semana 2 (2 al 8 de noviembre de 2026).

La actividad es individual, pero en el SGA figura como tarea del grupo ABZ (Apunte, Benites, Zambrano). Por eso mi trabajo está en la rama `apunte-washington` del repositorio del grupo, `AD-FORM-FB-01-ABZ`: la rama `main` contiene el trabajo de mi compañero Benites, esta rama contiene solo el mío, y ninguna de mis cinco referencias coincide con las suyas.

Son cinco fichas bibliográficas sobre fundamentos de sistemas distribuidos y arquitecturas distribuidas. Las usaré como base del informe TA-IND-01.

## Archivos

- `documento/main.tex`: código LaTeX de las fichas (archivo principal).
- `documento/referencias.bib`: las cinco referencias en BibTeX.
- `documento/main.pdf`: PDF compilado.
- `documento/ieee.bbx` y `documento/ieee.cbx`: estilo biblatex-ieee v1.4g (licencia LPPL 1.3c), sin cambios. Están junto al documento para que las referencias salgan con el mismo formato en cualquier computadora.

## Compilación

- Compilador: pdfLaTeX.
- Bibliografía: biblatex con Biber, estilo IEEE.
- Archivo principal: `documento/main.tex`.

Orden de comandos, desde la carpeta principal de esta rama:

```
cd documento
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

El primer `pdflatex` crea el archivo que lee Biber, Biber arma la bibliografía y las dos últimas pasadas completan citas e índice. También se puede usar `latexmk -pdf main.tex` dentro de `documento`.

En Overleaf: subir el contenido de esta rama, compilador pdfLaTeX y documento principal `documento/main.tex`. Overleaf ejecuta Biber solo.

## Dependencias

- TeX Live 2023 o posterior, o MiKTeX actualizado.
- Biber de la versión que corresponde a biblatex. El PDF se compiló con biblatex 3.19 y Biber 2.19.
- Paquetes: inputenc, fontenc, lmodern, babel (spanish y american), geometry, microtype, csquotes, array, booktabs, xltabular, enumitem, biblatex y hyperref. MiKTeX los instala la primera vez que se compila.

## Fuentes

Las cinco son de acceso abierto (licencias Creative Commons) y su PDF se descarga gratis desde el sitio del editor.

1. Pournazari *et al.*, *Cluster Computing*, 2025. DOI: [10.1007/s10586-025-05577-6](https://doi.org/10.1007/s10586-025-05577-6) · [PDF](https://link.springer.com/content/pdf/10.1007/s10586-025-05577-6.pdf)
2. Landau *et al.*, *Journal of Parallel and Distributed Computing*, 2025. DOI: [10.1016/j.jpdc.2025.105071](https://doi.org/10.1016/j.jpdc.2025.105071) · [PDF en ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0743731525000383) (botón *View PDF*)
3. Ferreira *et al.*, *Journal of Cloud Computing*, 2024. DOI: [10.1186/s13677-024-00716-7](https://doi.org/10.1186/s13677-024-00716-7) · [PDF](https://link.springer.com/content/pdf/10.1186/s13677-024-00716-7.pdf)
4. Al-Said Ahmad *et al.*, *Computing*, 2024. DOI: [10.1007/s00607-024-01292-z](https://doi.org/10.1007/s00607-024-01292-z) · [PDF](https://link.springer.com/content/pdf/10.1007/s00607-024-01292-z.pdf)
5. Barata *et al.*, *Cluster Computing*, 2026. DOI: [10.1007/s10586-026-06095-9](https://doi.org/10.1007/s10586-026-06095-9) · [PDF](https://link.springer.com/content/pdf/10.1007/s10586-026-06095-9.pdf)

Los cinco DOI llevan a la página del editor de cada artículo. Autores, año, título, revista, volumen, número y páginas o número de artículo se compararon con esa página y con el registro Crossref de cada DOI.

## Uso de inteligencia artificial

Usé Claude (Anthropic), modelo Claude Opus 5.5, para buscar artículos candidatos y revisar sus metadatos en Crossref, comprobar que el PDF de cada uno es de libre acceso, extraer cada dato concreto y redactarlo con su página o sección, redactar la introducción y la tabla de uso previsto, generar el código LaTeX, el archivo `.bib` y este README, y preparar un primer borrador de los resúmenes y las notas personales, que después reescribí con mis propias palabras; la IA solo revisó la ortografía y la gramática de la versión final y recortó algunas palabras para ajustar los resúmenes a la extensión pedida. Cada DOI se abrió en https://doi.org, los datos de cada referencia se cotejaron con la página de la revista y con Crossref, y cada dato concreto se buscó en el texto completo del artículo para confirmar su sección o página. La declaración completa está en la sección 4 de `documento/main.pdf`.
