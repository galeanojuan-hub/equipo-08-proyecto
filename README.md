# Proyecto LaTeX — Metodología de la Investigación

Documento académico (UPTC, Ingeniería de Sistemas y Computación) sobre la relación
entre arquitectura de software (monolítica/modular) y consumo/eficiencia energética.

## Estructura

```
proyecto/
├── main.tex
├── referencias.bib
├── README.md
└── capitulos/
    ├── introduccion.tex
    ├── idea_investigacion.tex
    ├── problema.tex
    ├── sintomas_causas_consecuencias.tex
    ├── narrativa.tex
    ├── antecedentes.tex
    └── formulacion.tex
```

## Compilación

Compila en Overleaf o localmente con `pdflatex` + `bibtex`:

```
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

Se incluye `texstyles/IEEEtran.bst` como respaldo por si el entorno de
compilación no trae preinstalado el estilo IEEEtran (Overleaf sí lo trae
por defecto, así que normalmente no hace falta). Si `bibtex` no encuentra
`IEEEtran.bst`, compila con:

```
BSTINPUTS=./texstyles: bibtex main
```

El proyecto ya fue compilado y verificado en este entorno (pdflatex + bibtex,
13 referencias, sin citas indefinidas, sin errores). Se incluye `main.pdf`
como vista previa del resultado.

## Estado del documento — pendientes

Marcadores que el equipo debe completar antes de la entrega final:

- `[TÍTULO DEFINITIVO POR CONFIRMAR]` — portada y subtítulo propuesto.
- `[NOMBRE DEL INTEGRANTE 1]` a `[NOMBRE DEL INTEGRANTE 4]` — portada.
- `[CIUDAD]` — portada.
- `[DATO PRISMA POR COMPLETAR]` — cifras exactas de identificación, cribado,
  elegibilidad e inclusión del proceso PRISMA (capítulo de antecedentes,
  sección "Metodología PRISMA aplicada a la búsqueda de antecedentes").
  El proceso descrito en el documento es exploratorio; una revisión
  sistemática formal con registro numérico completo queda pendiente
  para una fase posterior del proyecto.

## Referencias

Las 13 referencias incluidas en `referencias.bib` fueron verificadas mediante
búsqueda bibliográfica real (autores, título, año, venue/editorial y DOI cuando
está disponible). No se inventó ninguna referencia. La entrada `araujo2024energy`
tiene autoría parcialmente incompleta en la fuente consultada ("Araújo, G. et al.")
y debe completarse con la lista completa de autores al acceder al artículo
original en IEEE Access antes de la entrega final.

## Alcance de este entregable

Este documento cubre, según lo solicitado: introducción, idea de investigación,
problema de investigación, síntomas/causas/consecuencias, narrativa del problema,
antecedentes (con tabla de 13 estudios), formulación del problema (diagnóstico,
pronóstico, control del pronóstico) y pregunta de investigación. No se desarrollan
objetivos, hipótesis, variables, operacionalización ni diseño experimental, por no
haber sido solicitados en esta fase.
